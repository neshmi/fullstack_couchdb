# Oh, one more thing...

The philosophy (read: _my_ phiolosophy) emphasizes that documents be self contained.  Some of the Couch adapters that let you work with ActiveModel (Rails) like objects create different documents when really they should be self contained.

<br/>
JSON Document
```
{
  "_id": "my-house",
  "_rev": "blahblahblah",
  "pets": [
    {"type": "cat", "name": "Fluffy"},
    {"type": "cat", "name": "Whiskers"}
  ]
}
```

