# Columbia SQL Workshop

## Create MySQL Instance on Amazon Web Services

* Log into your [AWS Management Console](https://console.aws.amazon.com)
* Locate RDS under the Databases heading
* Within Amazon RDS click `Create database`
* Under `Choose a database creation method` click `Standard Create`
* Under `Engine options` choose `MySQL`
* Under `Templates` choose `Free tier`
* Under `Settings` name your `DB instance identifier` as `sqltest`
* Under `Credential settings` create a username and password combination that you will remember (you will need it)
* Under `Connectivity` expand `Additional connectivity configuration` to show additional menu items and make sure that `Publicly accessible` is `yes`
* Expand the `Additional configuration` menu
* Name the database `testdb`
* Uncheck `Automatic backups`
* Click `Create database`
