## Create npm library and publish to npm repository
1. Create js script with your name what you want, but in this article i use <strong>index.js</strong>. On this file you put your library process in here
2. Push into your git repository, this is important because npm repository will read the syntax from here.
3. Generate your <strong>package.json</strong> using command ```npm init``` and follow the step.
```
### Input your package name, if you put blank as default will set name as your folder project name
package name: (nodejs-hello-world-library)

### Input your version, if you put blank as default will set version as in display
version: (1.0.1)

### Input your description, if you put blank it will blank description
description:

### Input your entry point, it will set your root js 
entry point: (index.js)

### Git repository, it just show your repository
git repository: (https://github.com/fascalsj/nodejs-hello-world-library.git)

### Information about the author 
author:
```
4. Add npm user using ```npm adduser```
5. Publish your npm library using ```npm publish```
6. Install the library on your project ```npm install nodejs-hello-world-library@1.0.1 ``` 
7. Test it in your npm project

```
var test = require('nodejs-hello-world-library');

test.helloWorld;
test.doSomethingAwesome;
test.doSomethingElse;
test.doSomethinNew("ok");

```