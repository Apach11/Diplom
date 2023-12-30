# Дипломный проект по професии "Тестировщик"
## Для выполнения работы необходимо:
1. Установить Google Chrome;
2. Установить IntelliJ IDEA;
3. Установить Github;
4. Установить Docker Desktop.
## Запуск тестов
1. Запустить:  _InetelliJ IDEA_
2. Запустить: _Docker Desktop_
3. В терминале: _InetelliJ IDEA_ набрать команду _docker-compose up_ и нажать _Enter_
### Для проверки MySQL
1. Запустить  _jar_  файл командой:  _java "-Dspring.datasource.url=jdbc:mysql://185.119.57.126:3306/app" -jar artifacts/aqa-shop.jar_
2. После запуска _jar_ файла запустить тесты командой: _.\gradlew clean test "-Ddb.url=jdbc:postgresql://185.119.57.126:5432/app"_
3. Создание отчета командой: _./gradlew allureReport_
### Для проверки PostgreSQL
1. В новой вкладке терминала запустить приложение командой: _java "-Dspring.datasource.url=jdbc:postgresql://185.119.57.126:5432/app" -jar artifacts/aqa-shop.jar_
2. Запустить тесты командой: _.\gradlew clean test "-Ddb.url=jdbc:postgresql://185.119.57.126:5432/app"_
3. Создание отчета командой: _./gradlew allureReport_

