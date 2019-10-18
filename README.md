# Columbia SQL Workshop

[Slide Deck](https://github.com/learning-analytics-curriculum-teaching/sql-workshop/blob/master/sql_workshop.pdf)

## Create MySQL Instance on Amazon Web Services

* Log into your [AWS Management Console](https://console.aws.amazon.com)
* Locate `RDS` under the `Databases` heading
* Within Amazon RDS click `Create database`
* Under `Choose a database creation method` click `Standard Create`
* Under `Engine options` choose `MySQL`
* Under `Templates` choose `Free tier`
* Under `Settings` name your `DB instance identifier` as `sqltest`
* Under `Credential settings` create a username and password combination and write it down (you will need it later)
* Under `Connectivity` expand `Additional connectivity configuration` to show additional menu items and make sure that `Publicly accessible` is checked `Yes`
* Expand the `Additional configuration` menu
* Under `Initial database name` write `testdb`
* Uncheck `Automatic backups`
* Click `Create database`

## Modify Security Group

* Under `Security Groups` click `Inbound` and then `Edit`
* Add the rule `SQL/Aurora` on `Port 3306` with the `Connection` of `MyIP`
