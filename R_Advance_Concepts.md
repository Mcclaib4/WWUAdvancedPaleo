**Section 1**

1.
````R
> Greetings<-"Hello, World"
> Greetings
[1] "Hello, World"
````

2.
````R
> iris_split <- split(iris, iris$Species)
> new_names <- c("Setosa", "Versicolor", "Virginica")
> for (i in 1:length(iris_split))
+  {assign(new_names[i], iris_split[[i]])}
````

3.
````R **?**
> IrisFunction<-function(iris)
+     {AnswerVector<-array(NA,dim=dim(iris)[[1]])
+     for (index in 1:dim(iris)[[1]])
+     {if (iris[index,"Sepal.Width"]>3.1)
+             {AnswerVector[index]<-iris[index,"Petal.Length"]+iris[index,"Sepal.Length"]}
+         else if (iris[index,"Sepal.Width"]<3.1)
+         {AnswerVector[index]<-iris[index,"Sepal.Length"]-iris[index,"Petal.Length"]}}
+     return(AnswerVector)}
````

4.
````R

````
