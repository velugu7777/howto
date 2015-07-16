##How to install ember-cli
    Before installing ember-cli install node.js
    After installing go to command
    Type this syntax npm ember-cli -g
##Getting started
###How to install bower
    npm install bower -g
###how to  other static assets via Brocfile.js  
      bower install bootstrap --save  // it will save a reference in bower.json file

###how to see version
    ember -v
###how to create new app
          ember new myapp //app name
          cd myapp // app name

          // this will serve on http://localhost:4200
          // auto reloads whenever there is change in "app" folder
          // for any changes outside "app" folder we need to restart the server
          ember server

###How to crete object code in ember model
    1.open the  project
    2.After open the project
    3.Type in git [ember g model name(user)]
    4.After installing ember g model user
    5.it will be create app/models/user.js

    after finishing this open user.js-app/models
```js
      import DS from 'ember-data';
      import Ember from 'ember';
      To create object model
      export default DS.model.extend({
        name.DS.attr('string'),
        age.DS.attr('number'),
        isMarried.DS.attr('boolean'),
        });
```
###How to genrate Routes
    go to git type this ember g route user

###How to write code in routes
```js
    syntax:
    import Ember from 'ember';
    export default Ember.Route.extend({
      model:functon{
        return[
        {name:'anji',age:25},
        {name:koti,age:32},
        ];
      }
      });
    <--- To be continued >  
```
###How to write a code in templates

###How to genrate controoler
    go to git type this ember g controoler user
###How to write code in controller
```js
    Syntax:
        import Ember from 'ember';

        export default Ember.controller.extend({

          });
        <--- To be contiued >
```  
###How to set LocalStorage Adapter
      1.go to the application folder
      2.open the git bash and
      3.ember g adapter application (todo)
      4.after that ember install ember-localstorage-adapter
      4.after that go to the application.js and set the following in your application.js
        export default DS.LSAdapter.extend({
        namespace: 'api',
      5.after  that go the app.js and set the following in your app
        import DS from 'ember-data';
        App.ApplicationSerializer = DS.LSSerializer.extend();
###How to run ember app in github
     1.go to the git and type....ember build --environment production
     2.open the dist in your project and copy the files to your app
     3.open the index.html and set the following options
        set <base href="/appname/" />//vtodoapp
        Set the full path for following...(http://velugu7777.github.io/vtodoapp/)
        <link rel="stylesheet" href="http://velugu7777.github.io/vtodoapp/assets/vendor-a3a549a3c1534001dbc79026aaf213c4.css">
        <link rel="stylesheet" href="http://velugu7777.github.io/vtodoapp/assets/atodo-4e08dd69f47f73fc8ac91de7e9868dca.css">

       <script src="http://velugu7777.github.io/vtodoapp/assets/vendor-4b14358b7a4d1760f54b91c322283000.js"></script>
       <script src="http://velugu7777.github.io/vtodoapp/assets/atodo-e4eface054dc1df8b4cbe9e58f9a9f97.js"></script>
