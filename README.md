# JComSkeleton
Skeleton for developing Joomla! Components

## INTRO

Tool to create a custom skeleton of a Joomla! component.  
Starting point to start developing.
You can even roll out changes to your test environment as you develop.

## INSTALL PHING FROM COMPOSER
`composer install`

## EXECUTION
`php ./vendor/phing/phing/bin/phing`

### EXAMPLE > HELLO WORLD !
`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml`

`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml another_hello`

`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml build.01_Introduction`

### EXAMPLE > Delete Skeleton Folder
`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml delete.skeletons`

### EXAMPLE > Create a component skeleton with name JumerCom
Set the property **component.name** to give the name to the new component:

`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml create.from.template -Dtemplate=helloworld -Dcomponent.name=JumerCom1`

### EXAMPLE > Zip Skeleton Folder
`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml zip -Dcomponent.name=JumerCom1`
Install
sudo chmod g+w ~/Documentos/dev/joomla/labs_democracia_online/joomla-lab1/ -R

### EXAMPLE > BUILD
Change some files & build
`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml build -Dcomponent.name=JumerCom1`

### INSTALL COMPONENT IN JOOMLA FROM FOLDER
You will need to clone JComSkeleton in the "tmp" folder of your Joomla installation for this.
`/var/www/html/tmp/JComSkeleton/skeletons/JumerCom1`