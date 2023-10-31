
## create read update in mongo
```bash
use employee
```


```bash
db.createCollection('employees')
```


```bash
db.employees.insertMany([{name:'ram',role:'backend',salary:50000},{name:'sanjay',role:'frontend',salary:40000}])
```


```bash
 db.employees.find()
```

```bash
db.employees.updateOne({name:'sanjay'},{$set:{role:'backend'}})
```


```bash
db.employees.find()
```


```bash
db.employees.updateMany({role:'backend'},{$set:{salary:100000}})
```



## create and delete read delete
```bash
db.createCollection('student')
```
```bash
db.student.insertOne({name:'affan',age:22,grade:'O'})
```
```bash
db.student.insertMany([{name:'kaab',age:21,grade:'A'},{name:'talha',age:21,grade:'B'}])
```
```bash
db.student.find()
```
```bash
db.student.deleteOne({grade:'A'})
```
```bash
db.student.find()
```
```bash
db.student.deleteMany({})
```
```bash
db.student.find()
```

