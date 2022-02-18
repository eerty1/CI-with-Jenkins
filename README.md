# CI-with-Jenkins

For the whole period of working with this module the [only thing](https://www.youtube.com/watch?v=_DimZ1upYMU&ab_channel=Kurogan) was repeating in my head.

They are divided into 4 difficulty levels :face_with_head_bandage:

* I Can Win

* Bring It On

* Hurt Me Plenty

* Hardcore

## I Can Win requirements

1. Install Jenkins

2. Create a task that will do the following:
 
* Clone a project from [here](https://github.com/vitalliuss/helloci)

* Run tests from a project in the Java directory using the mvn test target

3. Configure the build triggers so that the task executes once every 5 minutes

## Bring It On requirements

1. Install Jenkins

2. Create a task that will do the following:

* Clone a project from [here](https://github.com/vitalliuss/helloci)

3. Configure build triggers:

* Run tests in 5 minutes after the commit to git

* Also run test every weekday at midnight

4. Publish the file "Java\target\surefire-reports\com.github.vitalliuss.damn it.AppTest.txt " like an artifact

## Hurt Me Plenty requirements

This task performance is based on the **Bring It On task**.

1. Change the server port to 8081

2. Create a node and configure the server so that the job is performed only on the slave node

3. Configure JobConfigHistory and thinBackup

## Hardcore requirements

This task performance is based on the **Hurt me plenty**.

1. Create a user and give him the rights to see the Jenkins job, but without the ability to record or change settings

2. Create a parameterized "Hello User job" that will ask the username as a parameter and write "Hello, username!" to the console.

3. Use the mvn cobertura:cobertura goal to measure the code coverage with unit tests (code coverage) and publish it on the jobs page as a graph

## Installation

It is essential to say about correct Maven version.

![This is an image](https://i.ibb.co/kSLL33z/image.png)

There're the steps to unpack my project: 

* git clone CI-with-Jenkins

* Unzip the file inside

## Other
 
All the materials were taken from the [EPAM Automated Testing course](https://training.epam.com/#!/Training/3044?lang=en). :test_tube:

The backup of the tasks could be found [there](https://github.com/vitalliuss/automation-training.git), in file "backup.md". :file_folder:

Unfortunately they provided only RU verion of the requirements.