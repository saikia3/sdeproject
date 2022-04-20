#Comparison of effectiveness & accuracy of Text-to-SQL Systems


## Contents

* [discover/](discover/) -> `Discover: Keyword Search in Relational Databases`
* [discoverIR/](discoverIR/) -> `EfficientIR-style Keyword Search over Relational Databases`
* [expressq2/](expressq2/) ->`Constructing an Interactive Natural Language Interface for Relational Databases`
* [sharedlib/](sharedlib/) -> A library shared by all systems (except `NaLIR`) used for database management and utility functions. This folder also contains the [query generator](sharedlib/src/main/java/shared/benchmark/Generator.java)

## Prerequisites
For the above mentioned systems to run, gradle build system is required and added to system path. Primarily Java 8.0 is the minimum requirement and bin set to JAVA_HOME within system path. A MySQL database or PostgreSql database without any preprocessing steps is required. MOreover, MySQL database must have some `FULLTEXT` indexes to enable the systems to search terms in the database. 

## Use
After the prerequisites are met, changing into a directory and then typing 'gradlew run' will execute the system

The system will prompt for 3 inputs:
* The query
* The database to search
* The number of results

Inserting each one of the above followed by an `enter` and post results are displayed, the system will ask for input. This can be interrupted with ctrl + c
