# ACSEO REST Generator using SensioGeneratorBundle

This bundle provide Twig template to generate CRUD REST applications with SensioGeneratorBundle in your Symfony2 application

## Requirements
- A Symfony 2 Project with SensioGeneratorBundle (embeded by default in the Symfony Standard Distribution)
- FOSRestBundle (https://github.com/FriendsOfSymfony/FOSRestBundle)
- NelmioApiDocBundle (https://github.com/nelmio/NelmioApiDocBundle) 

## How to use it

### Step 1 : Get the code
Get the code using ``git submodule`` command :
````
cd /path/to/my/sf2project
git submodule add https://github.com/acseo/RESTGenerator app/Resources/SensioGeneratorBundle
```` 
Now you should see a directory called 'skeleton' in app/Resources/SensioGeneratorBundle

### Step 2 : Generate the CRUD for an Entity
CRUD creation is just the same as the original ``app/console doctrine:generate:crud`` command.

````
 cd /path/to/my/sf2project
php app/console doctrine:generate:crud
````
And follow the guidelines.
Your REST controller should be generated now ! **But we must configure it**
### Step 3 : Configure POST and PUT actions
You will see that ``TODO`` insctruction have been generated in your Controller.
For now, we are not able to generate some usefull code to describe the attributes that the POST and PUT methods are waiting for.

Simply edit your Controller file to make it work as you expect.