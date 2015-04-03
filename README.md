# SQL Engine

The simple SQL engine which have the reduced functionality than the real SQL. Within it you can parse such query
operations:
* simple SELECT from the a table;
* it is possibly to specify columns (tableName.columnName) or select all of them (*);
* cross-join queries (by putting tables and separated them by a comma in the FROM block);
* WHERE queries with such operators in conditions: ['=', '<=', '>=', '>', '<', '!=']. It is possible to put in condition some columns to filter them by some conditions for instance (tableName1.columnName = tableName2.columnName).
Also you may put more than one WHERE condition: you can compound them only by 'AND' or 'OR' operators but not by them together in one query;
* JOIN and multi-JOIN queries;

### Tests

There are tests for parser.

To run them in console you must run such commands:

```sh
$ npm i
$ bower i
to run jasmine test you need to run:
$ karma start
to run protractor tests you need to run:
$ npm i protractor -g
$ npm  webdriver-manager update
$ npm  webdriver-manager start
  open new console and run
$ protractor  protractor.config.js
```


### Version
1.0.0