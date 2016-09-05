Publishing Turk HITs
====================

To publish HITs into a local (development) database, do the following, which assumes you're working in /var/www/demo, using demo.l.survos.com

Load the Initial Data
--------------------------


Load the PATH hits via Import Spreadsheet.  This gives a variety of jobs

1. Go to the Import Pilot job, by selecting it from under the Jobs sidebar menu

    http://demo.l.survos.com/app_dev.php/job/path-import_pilot

2. Check to make sure there's data and images by clicking on the Data Mapping tab

    http://demo.l.survos.com/app_dev.php/job/path-import_pilot/input_data
 
<img src="images/dataMapping.png" width="600" />
<!--- was
![dataMapping.png](/home/tac/Survos/docs/images/dataMapping.png "")
--->

3. Import some tasks by clicking on the button at the bottom of that page.

4. You should make sure there's a dedicated SQS queue to handle messages from Amazon if you're using a local database, and
set it in parameters.yml

    aws_sqs_url: 'https://sqs.us-east-1.amazonaws.com/279530343417/demo-tac'

Otherwise, the queue will end up with HITs that aren't processed by the 'notifications' process.

4. To actually import the photos, go to the status screen and click on publish, then open a terminal and run

   wiki/turk-background-jobs demo.l.survos.com 5 --publish --sync-tasks --sync-hits --sync-images --verbose

This will run a set of background jobs (some refactoring is needed here eventually) that move data around, publish
images to S3, and set up the Data Object database, which other HITs use as their datasource.

5. Finally we have some data to create other HITs.  Go to the 'basic' job:

   http://demo.l.survos.com/app_dev.php/job/path-basic

and click "Queue and Publish" (with Sandbox selected).  The background jobs will publish the HITs, which you can see on
sandbox and on the HITs tab.

6. In another terminal (or even in 'screen'), run app/console turk:notifications, which will sync the incoming messages from
the SQS turk queue with your local database.  This will be rewritten in NodeJS when we get an internal API working to update
our database.

