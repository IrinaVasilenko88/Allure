# Allure

# Обучение в Нетологии.

## Домашнее задание по курсу Автоматизированное тестирование

## Тема: Репортинг: Report Portal

- Настройка Allure, интегрированного с Selenide


# Инструкция по настройке Allure
1. В проекте в build.gradle прописать  

``` plugins{id'java'id'io.qameta.allure'version'2.8.1'}
...
allure{autoconfigure=true
version='2.13.0'//LatestAllureVersion
useJUnit5{version='2.13.0'//LatestAllureVersion
 }
}
repositories{
jcenter()
mavenCentral()
 }
 ```
 
**Для запуска использовать команду**
```
gradlew clean test allureReport
```
``` 
gradlew allureServe
```

**Для запуска проекта:**
1. Склонировать проект из репозитория командой 

```
git clone https://github.com/IrinaVasilenko88/Allure.git
``` 
2. Открыть склонированный проект в Intellij IDEA
3. Открыть в терминале каталог ```artifacts```
4. Для запуска приложения ввести команду ```java -jar app-card-delivery.jar```
5. Для запуска в браузере ввести ссылку http://localhost:9999/
6. Запустить команду
```
gradlew clean test allureReport
```
``` 
gradlew allureServe
```
