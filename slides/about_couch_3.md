## Map/reduce

CoffeeScript
```
(doc) ->
  if doc.title? and doc.date?
    emit doc.title, [doc.date, doc._id]
```

JavaScript
```
function(doc) {
  if(doc.title && doc.date) {
    emit(doc.title, [doc.date, doc._id]);
  }
}
```

results in:
```
{
   "_id": "_design/blog",
   "_rev": "1-67072284f987db058a4bcf02a57288a2",
   "language": "coffeescript",
   "views": {
       "title_date_id": {
           "map": "(doc) ->\n  if doc.title? and doc.date?\n    emit doc.title, [doc.date, doc._id]\n"
       }
   }
}
```