# JComSkeleton
Skeleton for developing Joomla! Components

## INTRO

Tool to create a custom skeleton of a Joomla! component.  
Starting point to start developing.
You can even roll out changes to your test environment as you develop.

## RESTRICTIONS
* need sudo rights
* build by copying files

## INSTALL PHING FROM COMPOSER
`composer install`

## EXECUTION
`php ./vendor/bin/phing`

### EXAMPLE > HELLO WORLD !
`php ./vendor/bin/phing -f ./buildfiles/build.xml`

`php ./vendor/bin/phing -f ./buildfiles/build.xml another_hello`

`php ./vendor/bin/phing -f ./buildfiles/build.xml build.01_Introduction`

### EXAMPLE > Delete Skeleton Folder
`php ./vendor/bin/phing -f ./buildfiles/build.xml delete.skeletons`

### EXAMPLE > Create a component skeleton with name JumerCom

In the web page [Developing an MVC Component](https://docs.joomla.org/J3.x:Developing_an_MVC_Component), you will find a series of articles explaining how to develop a compenent HelloWold for Joomla 3 from scratch. Each article add a new feature to the component HelloWorld. This command, creates a installable copy, with the name you want, for the HelloWorld version you choose:
`php ./vendor/bin/phing -f ./buildfiles/build.from.helloworld.xml create -Dtemplate=01_Introduction -Dcomponent.name=jumer`

Set the property **component.name** to give the name to the new component:

`php ./vendor/bin/phing -f ./buildfiles/build.xml create.from.template -Dtemplate=helloworld -Dcomponent.name=JumerCom1`

### EXAMPLE > Zip Skeleton Folder
`php ./vendor/bin/phing -f ./buildfiles/build.xml zip -Dcomponent.name=JumerCom1`
Install
sudo chmod g+w ~/Documentos/dev/joomla/labs_democracia_online/joomla-lab1/ -R

### EXAMPLE > BUILD
Change some files & build
`php ./vendor/bin/phing -f ./buildfiles/build.xml build -Dcomponent.name=JumerCom1`

### INSTALL COMPONENT IN JOOMLA FROM FOLDER
You will need to clone JComSkeleton in the "tmp" folder of your Joomla installation for this.
`/var/www/html/tmp/JComSkeleton/skeletons/JumerCom1`