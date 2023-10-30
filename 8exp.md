```bash
titanic = read.csv("C:/Users/affan/Desktop/BDA CODE/7/titanic_dataset.csv")
head(titanic)

sapply(titanic, class)

titanic$Survived = as.factor(titanic$Survived)

summary(titanic)

sum(is.na(titanic))
dropnull_train = titanic[rowSums(is.na(titanic)) <= 0,]
survivedlist = dropnull_train[dropnull_train$Survived == 1,] 
notsurvivedlist = dropnull_train[dropnull_train$Survived == 0,]

mytable <- table(titanic$Survived) 
lbls <- paste(names(mytable), "\n", mytable, sep="")
pie(mytable, labels = lbls, main = "Pie Chart of Survived column data\n (with sample sizes)")

hist(survivedlist$Age, xlab = "Age", ylab = "frequency")

temp <- density(table(titanic$Fare)) 
plot(temp, type = "n", main = "Fare charged from Passengers") 
polygon(temp, col = "lightgray", border = "gray")


```
