pouchdb-adapter-node-sql
======

Based on PouchDB adapter using Node-based SQLite (via [node-websql](https://github.com/nolanlawson/node-websql)) as its data store. Designed to run in Node.js. Its adapter name is `'websql'`.

### Usage

```bash
npm install github:liederivative/pouchdb-adapter-node-sql
```
or 

```bash
yarn add pouchdb-adapter-node-sql
```

```js
PouchDB.plugin(require('pouchdb-adapter-node-node-sql'));
var db = new PouchDB('mydb', {adapter: 'websql'});
```

Also the query interface has been changed as follows: 
```js
db.query('name-or-id-for-query', {selector: {name: "Hi"}, limit: 1})
```
This interface has partial support of query mango (couchdb).  

For full API documentation and guides on PouchDB, see [PouchDB.com](http://pouchdb.com/). For details on PouchDB sub-packages, see the [Custom Builds documentation](http://pouchdb.com/custom.html).

### Source

PouchDB and its sub-packages are distributed as a [monorepo](https://github.com/babel/babel/blob/master/doc/design/monorepo.md).

For a full list of packages, see [the GitHub source](https://github.com/pouchdb/pouchdb/tree/master/packages).


