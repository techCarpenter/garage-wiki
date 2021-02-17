# IndexedDB Tutorial

## Structure

```js
export default = {
DB1: {
  ObjectStore1: {
    Object1: {name: "", id: ""},
    Object2: {name: "", id: ""},
    Object3: {name: "", id: ""}
  },
  ObjectStore2: {
    Object1: {name: "", id: ""}
  }
},
DB2: {
  ObjectStore1: {
    Object1: {name: "", id: ""},
    Object2: {name: "", id: ""}
  },
  ObjectStore2: {
    Object1: {name: "", id: ""},
    Object2: {name: "", id: ""},
    Object3: {name: "", id: ""}
  }
};
```

## Actions

### Database

- `createObjectStore()`
- `deleteObjectStore()`

### Transaction

- `put()` - replaces value if key exists
- `add()` - throws error if key already exists

## Open Request

```js
const DB_NAME = "CRM";
const CONTACTS_STORE_NAME = "Contacts";
const DB_VERSION = 1;
let DB;

const request = window.indexedDB.open(DB_NAME, DB_VERSION);
```

## Define `onerror`

```js
request.onerror = function() {
  console.log("Database failed to open");
};
```

## Define `onsuccess`

```js
request.onsuccess = function () {
    console.log("Database opened successfully");

    // Store the opened database object in the db variable. This is used a lot below
    DB = request.result;
  };
```