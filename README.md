mvn compile flyway:migrate
mvn spring-boot:run
INSERT INTO ACCOUNT (ID, NAME, CREATED_ON) VALUES ('ROOT', 'ROOT', CURRENT_TIMESTAMP());
INSERT INTO ACCOUNT_CLOSURE (ANCESTOR_ACCOUNT_ID, DESCENDANT_ACCOUNT_ID) VALUES ('ROOT', 'ROOT');