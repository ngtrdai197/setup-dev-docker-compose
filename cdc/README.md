## CDC demo for performing data migration to new system

```curl
curl --location 'http://localhost:8083/connectors' \
--header 'Content-Type: application/json' \
--data '{
    "name": "account-service-connector",
    "config": {
        "connector.class": "io.debezium.connector.postgresql.PostgresConnector",
        "database.hostname": "postgres_db",
        "database.port": "5432",
        "database.user": "postgres",
        "database.password": "postgres",
        "database.dbname": "postgres_local",
        "database.server.name": "fullfillment",
        "table.include.list": "public.user_profile,public.supplier_profile",
        "topic.prefix": "cdc_account_service",
        "publication.autocreate.mode": "filtered",
        "value.converter.schemas.enable": false,
        "plugin.name": "pgoutput"
    }
}'
```