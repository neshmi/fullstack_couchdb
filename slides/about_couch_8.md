### Then...

Map:
```
function(doc){emit([doc.field, doc.square], doc.field);};
```

Reduce
```
function(keys,values){return true;};
```

RESTful Query
```
GET opendig-development/_design/OpenDigRails/_view/squares_by_field?group=true&startkey=["A"]&endkey=["A"]
```

JSON Result
```
{"rows":[

]}
```
 