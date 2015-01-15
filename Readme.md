## Setting up grunt with jasmine as Front End testing framework

###To setup the Grunt-testing framework follow the next steps:

1. Npm/bower for package installation:(ensure grunt and grunt-cli are installed globally)

- npm install grunt-contrib-jshint —> installing jshint for code quality standards

- npm install grunt-contrib-watch —> for watching file changes on you project

- npm install grunt-contrib-jasmine —> install the jasmine testing framework

2. Next step create the gruntile: touch Gruntfile.js

3. Copy the contents of the Gruntfile in this repo to your grunfile.

4. Create the same directory structure:
    
    public
        - js
            - spec
            * your js files

    If you want to use a different file structure make sure you update the following lines in your gruntfile:
        files: [ 'public/js/*.js','public/js/spec/*.js'] //line 8 in the gruntfile

5. Run grunt jasmine and you should see the tests
    If you want to ensure your code is meeting the jshint quality standars just run grunt watch, after you save any change in your js files you will see the errors or the lack of them.

6. If you have any doubt I don't mind to give you a hand if you email me your github url repo at galicians@gmail.com    


### Jasmine matchers:

The Jasmine testing framework from Pivotal Labs comes with this default set of matchers:

- expect(fn).toThrow(e);

- expect(instance).toBe(instance);

- expect(mixed).toBeDefined();

- expect(mixed).toBeFalsy();

- expect(number).toBeGreaterThan(number);

- expect(number).toBeLessThan(number);

- expect(mixed).toBeNull();

- expect(mixed).toBeTruthy();

- expect(mixed).toBeUndefined();

- expect(array).toContain(member);

- expect(string).toContain(substring);

- expect(mixed).toEqual(mixed);

- expect(mixed).toMatch(pattern);

In case you want to user additional matchers, you can use Jaime Mason package, just by running:

npm install jasmine-expect --save-dev

Here the url to his repo:
https://github.com/JamieMason/Jasmine-Matchers