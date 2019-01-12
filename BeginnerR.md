**Problemset 1**

1.
````R
typeof(mtcars)
[1] "list"
````
2.
````R
is(islands)
[1] "numeric" "vector"
````
3.
````R
> as.matrix(beaver1)
> beaver1.mtx<-as.matrix(beaver1)
> beaver1.mtx
> is(beaver1.mtx,"matrix")
[1] TRUE
````
4.
````R
> islands[8]
Borneo 
   280 
````
5.
````R
> mylist<-list(islands,beaver1,mtcars)
> mylist
````
6.
````R
> is(islands,"numeric")
[1] TRUE
````
7.
````R
> mtcars[2,7]
[1] 17.02
> mtcars[2,"qsec"]
[1] 17.02
> mtcars["Mazda RX4 Wag",7]
[1] 17.02
> mtcars[,"qsec"][2]
[1] 17.02
````
8.
````R
> islands[21][1]=83
> islands[24][1]=21
> islands[45][1]=10
````
9.
````R
> beaver1[3]
````
10.
````R
> ValueA<-sum(beaver1[3])
> ValueB<-sum(mtcars[6,])
> ValueC<-sum(islands[1:7])
> (ValueC/ValueB)+ValueA
[1] 4298.739
````
