# TrialDockerSpring

Instructions to evaluate the work done and explain the deliverables
-	Added git Configuration management…
-	docker run -p 3306:3306 --name rdb -e MYSQL_ROOT_PASSWORD=admin -d mysql:5.7
docker run --name myweb2 -p 8081:8080 --link rdb:rdb -e SPRING_DATASOURCE_URL=jdbc:mysql://rdb:3306/journals?createDatabaseIfNotExist=true serkan/journals
