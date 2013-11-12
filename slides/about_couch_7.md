### To Generate that list

Map:
```
function(doc){if (doc.field) emit(doc.field,doc.field);};
```

Reduce
```
function(keys,values){return true;};
```

RESTful Query
```
GET opendig-development/_design/OpenDigRails/_view/fields?group=true
```

JSON Result
```
{"rows":[
{"key":"A","value":true},
{"key":"B","value":true},
{"key":"C","value":true},
{"key":"D","value":true},
{"key":"E","value":true},
{"key":"F","value":true},
{"key":"G","value":true},
{"key":"H","value":true},
{"key":"K","value":true},
{"key":"L","value":true},
{"key":"M","value":true},
{"key":"N","value":true},
{"key":"R","value":true},
{"key":"S","value":true}
]}
```
 