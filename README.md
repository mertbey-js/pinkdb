# Pink DB



## Example

```js
const Database = require("pink-db");
const db = new Database("./database.json");

// Set data
db.set("Hello", "World");

// Get data
db.get("Hello"); // World

// Delete data
db.delete("Hello");

db.get("Hello"); // undefined
db.has("Hello"); // false
db.fetch("Hello"); // undefined

db.set("age", 10);
db.add("age", 1); // 11
db.subtract("age", 9); // 2

db.set("array", [ "apple" ]);
db.push("array", "orange"); // [ "apple", "orange" ]

// Clear data
db.clear();
```
#
