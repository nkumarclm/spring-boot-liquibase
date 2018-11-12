Build:
mvn clean package

Run:
mvn spring-boot:run

Access liquibase change log:
http://localhost:8080/liquibase


#Create local oracle schema

User Schema:
    create user PALM_LOCAL identified by PALM_LOCAL;
    
Grants:    
    GRANT create session TO PALM_LOCAL;
    Grant Resource to PALM_LOCAL;
    GRANT CREATE TABLE to PALM_LOCAL;
    GRANT CREATE VIEW TO PALM_LOCAL;
    GRANT CREATE SYNONYM TO PALM_LOCAL;
    GRANT CREATE ANY MATERIALIZED VIEW TO PALM_LOCAL;
    GRANT ALTER ANY MATERIALIZED VIEW TO PALM_LOCAL;
