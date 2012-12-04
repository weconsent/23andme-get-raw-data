23andme-get-raw-data
====================

Gets the raw data from 23andme and provides it for download. That's it!

This is a simple app to:

* get authorization from a user
* then quickly construct a downloadable package of his/her genome
* provide a download link to this data
* provide a mechanism to push over to the PLC site
* provide a mechanism to delete this data uponc completion


Documentation on Genome
=======================

Check out:

* http://snpedia.com/index.php/23andMe
* https://api.23andme.com/docs/ 23andme API


Setup 
=====

* Create an apache web server instance
* Clone this repository
* Test out the site
* Set a cron job to clean out the constructed package folder every 3 hours
* Example crontab to add:

     14 */3 * * * USERNAME rm -Rf /path/to/packages/*
