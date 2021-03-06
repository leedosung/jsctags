```js
function Base() {}
Base.prototype = {};

Base.prototype; //: Base.prototype
new Base; //: Base

function Sub1() {}
Sub1.prototype = new Base();
new Sub1(); //: Sub1

function Sub2() {}
Sub2.prototype = Object.create(Base.prototype);
new Sub2(); //: Sub2

function Base2() {}

function Sub3() {}
Sub3.prototype = new Base2();

new Sub3(); //: Sub3
```
```json
[
  {
    "id": "19d3eb70-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "Base",
    "addr": "/Base/",
    "kind": "f",
    "type": "void function()",
    "lineno": 1,
    "origin": {
      "!span": "9[0:9]-13[0:13]",
      "!type": "fn()",
      "!data": {
        "isConstructor": true,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  },
  {
    "id": "19d43990-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "prototype",
    "addr": "/prototype/",
    "kind": "v",
    "lineno": 2,
    "namespace": "Base",
    "parent": "19d3eb70-7aef-11e6-b7ac-3b6df8d5ccc7",
    "origin": {
      "!span": "24[1:5]-33[1:14]",
      "!data": {
        "isConstructor": false,
        "scoped": false,
        "isArg": false,
        "type": "Object.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  },
  {
    "id": "19d43991-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "Sub1",
    "addr": "/Sub1/",
    "kind": "f",
    "type": "void function()",
    "lineno": 7,
    "origin": {
      "!span": "105[6:9]-109[6:13]",
      "!type": "fn()",
      "!data": {
        "isConstructor": true,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  },
  {
    "id": "19d43992-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "prototype",
    "addr": "/prototype/",
    "kind": "v",
    "lineno": 8,
    "namespace": "Sub1",
    "parent": "19d43991-7aef-11e6-b7ac-3b6df8d5ccc7",
    "origin": {
      "!span": "120[7:5]-129[7:14]",
      "!data": {
        "isConstructor": false,
        "scoped": false,
        "isArg": false,
        "type": "Base.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  },
  {
    "id": "19d43993-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "Sub2",
    "addr": "/Sub2/",
    "kind": "f",
    "type": "void function()",
    "lineno": 11,
    "origin": {
      "!span": "175[10:9]-179[10:13]",
      "!type": "fn()",
      "!data": {
        "isConstructor": true,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  },
  {
    "id": "19d43994-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "prototype",
    "addr": "/prototype/",
    "kind": "v",
    "lineno": 12,
    "namespace": "Sub2",
    "parent": "19d43993-7aef-11e6-b7ac-3b6df8d5ccc7",
    "origin": {
      "!span": "190[11:5]-199[11:14]",
      "!data": {
        "isConstructor": false,
        "scoped": false,
        "isArg": false,
        "type": "Base.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  },
  {
    "id": "19d43995-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "Base2",
    "addr": "/Base2/",
    "kind": "f",
    "type": "void function()",
    "lineno": 15,
    "origin": {
      "!span": "264[14:9]-269[14:14]",
      "!type": "fn()",
      "!data": {
        "isConstructor": true,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  },
  {
    "id": "19d460a0-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "Sub3",
    "addr": "/Sub3/",
    "kind": "f",
    "type": "void function()",
    "lineno": 17,
    "origin": {
      "!span": "285[16:9]-289[16:13]",
      "!type": "fn()",
      "!data": {
        "isConstructor": true,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  },
  {
    "id": "19d460a1-7aef-11e6-b7ac-3b6df8d5ccc7",
    "name": "prototype",
    "addr": "/prototype/",
    "kind": "v",
    "lineno": 18,
    "namespace": "Sub3",
    "parent": "19d460a0-7aef-11e6-b7ac-3b6df8d5ccc7",
    "origin": {
      "!span": "300[17:5]-309[17:14]",
      "!data": {
        "isConstructor": false,
        "scoped": false,
        "isArg": false,
        "type": "Base2.prototype"
      }
    },
    "tagfile": "__DIR__/protoname.js"
  }
]
```
```ctags
Base	__DIR__/protoname.js	/Base/;"	f	lineno:1	type:void function()
prototype	__DIR__/protoname.js	/prototype/;"	v	lineno:2	namespace:Base
Sub1	__DIR__/protoname.js	/Sub1/;"	f	lineno:7	type:void function()
prototype	__DIR__/protoname.js	/prototype/;"	v	lineno:8	namespace:Sub1
Sub2	__DIR__/protoname.js	/Sub2/;"	f	lineno:11	type:void function()
prototype	__DIR__/protoname.js	/prototype/;"	v	lineno:12	namespace:Sub2
Base2	__DIR__/protoname.js	/Base2/;"	f	lineno:15	type:void function()
Sub3	__DIR__/protoname.js	/Sub3/;"	f	lineno:17	type:void function()
prototype	__DIR__/protoname.js	/prototype/;"	v	lineno:18	namespace:Sub3
```
