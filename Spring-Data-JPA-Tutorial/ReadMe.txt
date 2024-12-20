One Step project in understanding spring application -> Database connection.

1. Support for multiple databases.
2. Add ER Diagram for better relation understanding.
3. Add docker compose for setting up different DBs, Also add instructions in running them.


Setting up postgresDB:

    1. cmd: docker-compose up -d
    2. It'll start both PostgreSQL & PgAdmin
    3. Connecting PgAdmin to PostgresDB:
        1. Open http://localhost:5050 in your browser
        2. Email: admin@pgadmin.com
        3. Password: admin
        4. Create -> Server
        5. {"Name":"PostgresDB", "Host":"postgres-db", "Port":"5432", "Username":"admin", "Password":"password"} (HostName = ContainerName & port number is container port number i.e. 5432)
        6. Save & test the connection
    4. cmd: docker-compose down -d (stopping DB)

Setting up H2Console DB:
    1. Uncomment the H2Console properties
    
ER Diagram:

About Code: