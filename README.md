<h1 align="center">
  <a href="https://www.ndi.org/"><img src="https://www.ndi.org/sites/all/themes/ndi/images/NDI_logo_svg.svg" alt="NDI Logo" width="200"></a>
</h1>

<h1 align="center">
  Sample Lando Repo
</h1>

<p align="center">
  <a href="#documentation">Documentation</a> - 
  <a href="#installation">Installation</a> - 
  <a href="#contributing">Contributing</a> - 
  <a href="#license">License</a> - 
  <a href="#authors">Author(s)</a>
</p>

Sample Lando Repo, originally conceived @ NDI <br />
This is a Drupal 7 site. <br />
Local dev happens with Lando (https://docs.devwithlando.io)

## Documentation

* Install Lando for your system
    * https://docs.devwithlando.io/installation/installing.html
* Clone this repo     
* Check that .lando.yml has everthing you need
* Run "lando start" from the app root
* Import the DB: "lando db-import database.sql" 
  * (I removed the DB file as this is an anonymized version of a production site)
* Create a web/sites/default/settings.local.php
    * There is a template in web/sites/default/default.settings.local.php
* Update web/sites/default/settings.local.php
    * You can find the correct settings with "lando info"
    * You probably just need to set the DB name, user and pass. These are in "database->creds"
    * If you need to set the DB host and port, use the details in "database->internal_connection"
* Site should be available at the URLs in the "urls" sections from "lando info"    

## Useful commands
* lando start
* lando stop
* lando drush command
* lando php -v
( lando mysql

## Author(s)

<b>Dean Valentine</b>
> Website [https://dmv.tech](https://dmv.tech) &nbsp;&middot;&nbsp;
> GitHub [deanvalentine](https://github.com/deanvalentine) &nbsp;&middot;&nbsp;
> Twitter [@deanmv](https://twitter.com/deanmv) &nbsp;&middot;&nbsp;
> Drupal [deanvalentine](https://www.drupal.org/u/deanvalentine)
