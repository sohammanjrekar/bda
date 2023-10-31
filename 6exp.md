## index and aggregate
```bash
db.createCollection('student')
```

```bash
db.student.insertOne({name:'affan',class:'BE COMP',marks:95})
```
```bash
db.student.insertMany([{name:'kaab',class:'BE AIDS',marks:85},{name:'talha',class:'BE COMP',marks:80},{name:'wael',class:'BE COMP',marks:75}])
```
```bash
db.student.find()
```
```bash
db.student.createIndex({name:1})
```
```bash
db.student.getIndexes()
```
```bash
db.student.aggregate([{$group:{_id:'$class',average:{$avg:'$marks'}}}])
```
```bash
db.student.aggregate([{$sort:{marks:-1}},{$limit:1}])
```






## limit and sort
```bash
db.createCollection('Book')
``````bash
db.Book.insertOne({name:'BDA', author:'abc',published:1990,price:100})
``````bash
db.Book.insertMany([{name:'ML', author:'affu',published:2010,price:200},{name:'BC',author:'kaab',published:2022,price:300},{name:'DMMM',author:'wael',published:2023,price:350}])
``````bash
db.Book.find()
``````bash
db.Book.find().limit(2)
``````bash
db.Book.find().sort({price:1})
















