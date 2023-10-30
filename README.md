# golang-web-api-dolt-pop

## Description
This returns a data dump of the table `pop`
as a JSON encoded string. An ORM is used to
create and seed the database.

## Tech stack
- bash
- dolt
- golang

## Docker stack
- ubuntu:latest
- dolthub/dolt-sql-server

## Build notes
The service takes about 1 min before callable.

## To run
`sudo ./install.sh -u`
Available at http://localhost:8080

## To stop
`sudo ./install.sh -d`

## To see help
`sudo ./install.sh -h`

## Credits
- https://tutorialedge.net/golang/golang-mysql-tutorial/
- https://levelup.gitconnected.com/build-a-rest-api-using-go-mysql-gorm-and-mux-a02e9a2865ee
