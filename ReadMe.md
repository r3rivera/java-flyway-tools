### Executing Flyway via command line
```
mvn flyway:migrate -Dflyway.configFile=<path>/config.properties
```

The command above will be executed by the jenkins pipeline.



#### Sample of the config.properties file content 
```
flyway.user=
flyway.password=
flyway.schemas=
flyway.url=jdbc:postgresql://amazon_rds_url
flyway.locations=filesystem:database/sear
flyway.sqlMigrationPrefix=ver
flyway.table=sear_flyway_db_history
#flyway.baselineOnMigrate=true
```