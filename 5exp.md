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
