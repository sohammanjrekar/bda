
```bash
hdfs dfs -ls/
```


```bash
hdfs dfs - mkdir /test1
```


```bash
hdfs dfs -ls/
```

I will copy a text file named ‘hello’ from my local file system to this folder that 
```bash
hdfs dfs -copyFromLocal C:\Users\hp\Downloads\hello.txt /test1
```

```bash
hdfs dfs -ls/test1
```

To view the contents of the file we copied, I will use cat command
```bash
hdfs dfs –cat /test1/hello.txt
```

To Copy file from hdfs to local directory, I will use get command 
```bash
hdfs dfs -get /test1/hello.txt C:\Users\hp\Desktop\priyanka
```

remove a file 
```bash
hdfs dfs -rm /test1/hello.txt
```
