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
> with(mtcars, tapply(mpg, cyl, mean))
       4        6        8 
26.66364 19.74286 15.10000
````

5.
````R
> PbD<-function(NumDraw)
+ {DrawMatrix<-matrix(NA,nrow=NumDraw,ncol=6)
+ for (draw in 1:NumDraw)
+ {DrawMatrix[draw,1:5]<-sample(c(1:69),5,replace=FALSE)
+ DrawMatrix[draw,6]<-sample(c(1:26),1,replace=FALSE)}
+ return(DrawMatrix)}
> PbD(1000000)
````

6.
````R
> PbD<-function(MyNum)
+ {DrawMatrix<-matrix(NA,nrow=1000000,ncol=6)
+ for (draw in 1:1000000)
+ {DrawMatrix[draw,1:5]<-sample(c(1:69),5,replace=FALSE)
+ DrawMatrix[draw,6]<-sample(c(1:26),1,replace=FALSE)}
+ MatchTest<-array(NA,dim=1000000)
+ for (test in 1:1000000)
+ {MatchTest[test]<-all(DrawMatrix[test,]==MyNum)}
+ Result<-any(MatchTest)
+ return(Result)}
> print(PbD(c(1,16,21,43,69,17)))
[1] FALSE
````
