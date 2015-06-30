##How to install ember-cli
    Before installing ember-cli install node.js
    After installing go to command
    Type this syntax npm ember-cli -g
##Getting started
###how to see version
    ember -v
###how to create new app
          ember new myapp //app name
          cd myapp // app name
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
    go to git type this ember g router user

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
###How to wrie code in router
        <--- to be continued >
