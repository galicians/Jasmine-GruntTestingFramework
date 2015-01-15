## Setting up grunt with jasmine as Front End testing framework

###To setup the Grunt-testing framework follow the next steps:

1. Npm/bower for package installation;

- npm install grunt-contrib-jshint —> installing jshint for code quality standards

- npm install grunt-contrib-watch —> for watching file changes on you project

- npm install grunt-contrib-jasmine —> install the jasmine testing framework

2. Next step create the gruntile: touch Gruntfile.js

3. Copy the contents of the Gruntfile in this repo to your grunfile.

4. Create the same directory structure:
    
    public
        - js
            - specs
            * your js files

    If you want to use a different file structure make sure you update the following lines in your gruntfile:
        files: [ 'public/js/*.js','public/js/specs/*.js'] //line 8 in the gruntfile

5. Run grunt jasmine and you should see the tests
    If you want to ensure your code is meeting the jshint quality standars just run grunt watch, after you save any change in your js files you will see the errors or the lack of them.

6. If you have any doubt I don't mind to give you a hand if you email me your github url repo at galicians@gmail.com    
