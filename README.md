<h1>Alita Automation</h1>

<h2>Build<h2/>

- Go to project root folder, ex: ```cd theAlita```
- Download composer: ```curl -sS https://getcomposer.org/installer | php```
- Install via composer: ```php composer.phar install```
- Init
    - Config database in ```application/config/database.php``` (See database.php.example)
      <h2>Build cronjob</h2
- Created folder job_logs, ex: ``mkdir job_logs``
- Run jobs, ex:
    - 1: ``*/5 * * * *  php index.php cronJob FixCompletedAudiencesJob``   or ``*/5 * * * *  php /var/www/theAlita/index.php cronJob FixCompletedAudiencesJob``
    - 2 : ``*/5 * * * *  php index.php cronJob FixDownloadJob``   or ``*/5 * * * *  php /var/www/theAlita/index.php cronJob FixDownloadJob``
    - 3 : ``*/5 * * * *  php index.php cronJob FixImportAudiencesJob``   or ``*/5 * * * *  php /var/www/theAlita/index.php cronJob FixImportAudiencesJob``
    - 4 : ``*/5 * * * *  php index.php cronJob FixSyncData``   or ``*/5 * * * *  php /var/www/theAlita/index.php cronJob FixSyncData``
    - 5 : ``*/5 * * * *  php index.php jobs FixMaintainingFee``   or ``*/5 * * * *  php /var/www/theAlita/index.php jobs FixMaintainingFee``