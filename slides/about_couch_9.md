### It won't work unless...

RESTful Query
```
GET opendig-development/_design/OpenDigRails/_view/squares_by_field?group=true&startkey=["A"]&endkey=["A",{}]

OR

GET opendig-development/_design/OpenDigRails/_view/squares_by_field?group=true&startkey=["A"]&endkey=["A\uffff"]
```

JSON Result
```
{"rows":[
  {"key":["A","7J49"],"value":true},
  {"key":["A","7J59"],"value":true},
  {"key":["A","7J68"],"value":true},
  {"key":["A","7J69"],"value":true},
  {"key":["A","7J78"],"value":true},
  {"key":["A","7J79"],"value":true},
  {"key":["A","7K40"],"value":true},
  {"key":["A","7K41"],"value":true},
  {"key":["A","7K42"],"value":true},
  {"key":["A","7K50"],"value":true},
  {"key":["A","7K51"],"value":true},
  {"key":["A","7K52"],"value":true},
  {"key":["A","7K60"],"value":true},
  {"key":["A","7K61"],"value":true},
  {"key":["A","7K62"],"value":true},
  {"key":["A","7K70"],"value":true},
  {"key":["A","7K71"],"value":true},
  {"key":["A","7K72"],"value":true}
]}
```
 