# java-cli-mill-h2-index

## Description
A java millbuild build, that connects to h2
database.

Creates a small database table
called `dog`. This table, `dog`, has been normalized to 3NF.
Two new tables have been added, `breedLookup` and `colorLookup`.
Creates a new table `dog_expanded` that joins
`dog`, `breedLookup` and `colorLookup`. Added nonclustered indexes on
`dog`.breedId and `dog`.colorId. All output normally
seen in a terminal will be in `java-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

H2 is a database written in `java`
and is best known for a `dev` only
use.

## Tech stack
- java
- millbuild
- h2 driver

## Docker stack
- nightscape/scala-mill

## To run
`sudo ./install.sh -u`

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`
