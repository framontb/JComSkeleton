# JComSkeleton
Skeleton for developing Joomla! Components

## INTRO

Tool to create a custom skeleton of a Joomla! component.  
Starting point to start developing.
You can even roll out changes to your test environment as you develop.

## EXECUTION

`php ./vendor/phing/phing/bin/phing`

### EXAMPLE > HELLO WORLD !

`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml`

`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml another_hello`

`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml build.01_Introduction`

### EXAMPLE > Create a component skeleton with name JumerCom
Set the property **component.name** to give the name to the new component:

`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml build.from.template -Dtemplate=helloworld -Dcomponent.name=JumerCom2`

### EXAMPLE > Delete Skeleton Folder

`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml delete.skeletons`

### EXAMPLE > Zip Skeleton Folder
`php ./vendor/phing/phing/bin/phing -f ./buildfiles/build.xml build.zip -Dcomponent.name=JumerCom1`