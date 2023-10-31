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
