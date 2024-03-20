These scripts are meant to perform the function of importing data from the Google Ad manager API, and exporting it into Google Cloud Storage. It then should transform and load that data into Bigquery. This process should then be automated via cron or a scheduler program. 

To do:

-Issues with how to tackle loading the data from Google Cloud Storage into BigQuery, primarily authentication via the Google CLI

-How to modify the initial API code script into exporting the data into an online directory rather than how it currently downloads to a local directory, remove the need for a local machine.

-Perhaps change how the scripts export the data into Google Cloud Storage, currently does so by taking the hour in which the data was processed and exports it accordingly, whilst the cron job being adjusted so that the scripts operate during the middle of the hour
and occuring in the appropriate order, I can see some potential for the script to break because of this approach.
