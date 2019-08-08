### pymongo
---
https://github.com/mher/pymongo

https://docs.mongodb.com/ecosystem/drivers/python/

```py
import pymongo
connection = pymongo.Connection("localhost", 27017)
db = connection.test
db.name()

db.my_collection
db.my_collection.save({"x": 10})
db.my_collection.save({"x": 8})
db.my_collection.save({"x": 11})
db.my_collection.find_one()
for item in db.my_collection.find():
  print item["x"]
for item in db.my_collection.find().sort("x", pymongo.ASCENDING):
  print item["x"]

```

```
```

```
```

