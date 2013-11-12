## Map/reduce

CoffeeScript
```
(doc) ->
  if doc.title? and doc.date?
    emit doc.title, [doc.date, doc._id]
```

RESTful Query
```
GET /blog/_design/blog/_view/title_date_id
```

JSON Result
```
{"total_rows":3,"offset":0,"rows":[
{"id":"couchdb-is-so-amazing","key":"CouchDB is so amazing","value":["2013/06/30 18:04:11","couchdb-is-so-amazing"]},
{"id":"my-final-post","key":"My final post","value":["2013/08/30 18:04:11","my-final-post"]},
{"id":"yay-for-archaeology","key":"Yay for Archaeology!!","value":["2013/07/30 18:04:11","yay-for-archaeology"]}
]}
```