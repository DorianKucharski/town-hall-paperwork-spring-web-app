# Town Hall Paperwork Spring Web App

## Description

Simple Spring Boot web app created as part of my Spring learning.
The theme is a town hall management system focused on forms and applications
(the UI and sample forms are in Polish).

### Used technologies

- Java
- Spring
- PostgreSQL
- Flyway
- Thymeleaf
- iTextPDF
- Bootstrap

### Features

- creating new users
- managing user roles
- creating, editing and deleting forms
- filling in, editing, deleting and submitting applications
- reviewing applications by clerks, who can accept or reject them
- generating PDFs of applications and forms
- simple statistics

## Build and run

Requirements: Java 11 and a running PostgreSQL server. Maven is provided through the wrapper.

Database connection settings are in `src/main/resources/application.properties`
(`spring.datasource.*` for the app and `spring.flyway.*` for migrations). By default they point at
a local PostgreSQL on port 5432; adjust the database names and credentials to your setup.

```bash
./mvnw spring-boot:run      # run the app (Windows: mvnw.cmd spring-boot:run)
./mvnw package              # build a jar into target/
```

On the first visit to the home page with an empty `users` table, the app seeds a test user, a
test admin/clerk account and a sample form (see `FirstRunService.java`).

## Preview

![1](https://user-images.githubusercontent.com/54181425/131108599-50896955-6c29-4df6-933c-7bbc101df882.png)
![2](https://user-images.githubusercontent.com/54181425/131108600-c7c908b6-fb5f-4ff1-bf9c-007e98d031a3.png)
![3](https://user-images.githubusercontent.com/54181425/131108602-966b1fe2-3460-49ad-9300-7ccd6cb457e0.png)
![4](https://user-images.githubusercontent.com/54181425/131108604-1fd06256-91d4-45e0-b859-5047b89ae39f.png)
![5](https://user-images.githubusercontent.com/54181425/131108606-18433f4e-e168-45ed-b016-a1f0e0126e53.png)
![6](https://user-images.githubusercontent.com/54181425/131108609-052c7865-4601-4850-8100-64be8951c500.png)
![7](https://user-images.githubusercontent.com/54181425/131108614-c4b1b028-b6f0-472e-b1d0-a5c12b132714.png)
![8](https://user-images.githubusercontent.com/54181425/131108616-ef7019ad-8ec6-4eca-b99c-49776d7bbd81.png)
![9](https://user-images.githubusercontent.com/54181425/131108619-79c75679-b836-475a-b641-1dddbfed102e.png)
![10](https://user-images.githubusercontent.com/54181425/131108623-7caa4837-e6fc-4b3d-8172-993fca35acac.png)
![11](https://user-images.githubusercontent.com/54181425/131108624-9503afe0-7a33-4b95-a0b2-a548cd6a75b6.png)
