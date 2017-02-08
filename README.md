# survos-documentation
RST and Generated HTML for Survos Platform (using Sphinx)

##Installation

First, install sphinx
```
sudo pip install sphinx sphinx-autobuild sphinxcontrib-httpdomain
```
In case of pip error
```
sudo apt-get install python-pip python-setuptools
```

##Workflow

Module and Survey Types rst files are generated from the Survos 6 Platform, and 

```
cd /var/www/survos
bin/console adhoc:generate-rst
cd /var/www/survos-documentation
```

The rst files outside of the /modules and /survey-type directories are coded manually.  In particular, we need to make sure that they are properly linked to each other and that the toctree is properly set.

Generate docs
```
make html
```

After the files are committed and push, they will automatically be republished on readthedocs.

http://survos-documentation.readthedocs.io/en/latest/index.html

They are also available on Survos

http://l.stagingsurvos.com/docs/

(Note: auto-publish is not yet set up on StagingSurvos)`
