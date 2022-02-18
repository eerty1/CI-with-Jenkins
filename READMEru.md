# CI-with-Jenkins

На протяжении всего времени, сколько я занимался этим модулем, в голове у меня звучала [одна вещь](https://www.youtube.com/watch?v=_DimZ1upYMU&ab_channel=Kurogan)

Модель можно назвать побежденным после выполнения следующих заданий, которые поделены на 4 уровня сложности: 

* I Can Win

* Bring It On

* Hurt Me Plenty

* Hardcore

## Условия I Can Win

1. Установите Jenkins

2. Создайте задачу, которая будет делать следующее:

* Клонировать проект [отсюда](https://github.com/vitalliuss/helloci)

* Запускать тесты из проекта в директори Java с помощью цели mvn test

3. Настройте билд триггеры таким образом, чтобы задача выполнялась раз в 5 минут

## Условия Bring It On

1. Установите Jenkins

2. Создайте задачу которая будет делать следующее:

* Клонировать проект [отсюда](https://github.com/vitalliuss/helloci)

* Запускать тесты из проекта в директори Java с помощью цели mvn test

3. Настройте билд триггеры:

* Запуск тестов не позднее чем через 5 минут после коммита в git

* Каждый будний день в полночь

4. Опубликуйте файл “Java\target\surefire-reports\com.github.vitalliuss.helloci.AppTest.txt” как артефакт

## Условия Hurt Me Plenty

Данное задание выполняется на основе *Bring It On* задачи.

1. Сменить порт сервера на 8081

2. Создать ноду и настроить сервер так, чтобы джоба выполнялась только на slave ноде

3. Настроить Job Config History и thinBackup

## Условия Hardcore

Данное задание выполняется на основе *Hurt Me Plenty*

1. Создать пользователя user и дать ему права на просмотр джоб Jenkins, но без возможности записи или смены настроек

2. Создать параметризованную джобу HelloUser, которая будет спрашивать в качестве параметра имя пользователя (username) и писать в консоль "Hello, username!".

3. С помощью цели  mvn cobertura:cobertura измерьте покрытие кода юнит-тестами (code coverage) и опубликуйте на странице джобы в виде графика

## Установка

Используйте правильную версию Maven.

![This is an image](https://i.ibb.co/kSLL33z/image.png)

Далее алгоритм действий прост:

* git clone CI-with-Jenkins

* Разархивируйте файл внутри

## Прочее

Все материалы были взяты из курса [EPAM Automated Testing course](https://training.epam.com/#!/Training/3044?lang=en). :test_tube:

Резервную копию заданий вы можете найти [тут](https://github.com/vitalliuss/automation-training.git), файл называется "backup.md". :file_folder: