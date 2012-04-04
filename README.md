Prerequisites
-------------

* All your Grails versions must be installed under the same base directory. Ex:

        /opt/grails-1.0.3
        /opt/grails-1.1.1
        /opt/grails-1.3.2

* `GRAILS_HOME` environment variable must be set and point to your "default" Grails installation
* This script was tested on Mac OS X (Snow Leopard), Linux (Ubuntu) and Windows (with cygwin)

Installation
------------

* Download the script: http://github.com/deluan/grails.sh/raw/master/grails
* Include the folder where it is installed in your `PATH`. 
* Exclude `$GRAILS_HOME/bin` from your `PATH`

Usage
-----

Using the script is as transparent as possible:

* If you invoke it from a project folder, it will detect the version used by the project and call the correct grails
	* If the required version does not exist locally, the script will attempt to download the version specified from grails amazon mirror
* If you invoke it from any other folder that does not contain a Grails project, it will call the "default" Grails installation
* If you want to call a specific Grails version (i.e. when doing an upgrade) you can specify the version you want in the first parameter. 
	* If the version you specified does not exist locally, it will also attempt to download the version specified.

	Ex: $ grails 1.3.3 upgrade

