**Section 1**

1.

It designates whether or not the function should replace the current elements of the matrix with new ones.

2.
````R
> 1*MyMatrix
````

3.
````R
> all(MyMatrix==1)
[1] FALSE
````

**Section 2**

4.
````R
> which(MyMatrix==7)
[1] 17 32 37 48 53 60 71 83 91

> table(MyMatrix)
````
9

5.
````R
> apply(MyMatrix,2,sum)
 [1] 46 35 32 50 45 61 38 47 38 39 57 50
 ````
 
 6.
 ````R
 > apply(MyMatrix,2,prod)
 [1]  100000    9600    6804  840000  241920 7741440   12600  403200   70000   38880 4408992 1008000
````

7.
````R
> MyMatrix[which(MyMatrix==1)]<-11
````

8.
````R
> sum(MyMatrix>3 & MyMatrix<8)
[1] 34
````

9.
````R
> MyFrame<-as.data.frame(MyMatrix)
> MyFrame[,12]<-as(MyFrame[,12],"character")
> MyFrame
  V1 V2 V3 V4 V5 V6 V7 V8 V9 V10 V11 V12
1 10  6  7  3 11  8 11  4  5   8   6  10
2 11  2 11 10  6  9 10  3 10  11   8   5
3  5  5  2  8  6  8 11 10  5   6   7   7
4 11 11  3  5 10  8  5  7  2   3   6   9
5 10  2  9  5  7  3  7  3  5   5   3   2
6 10  8  3 10  4  8  9  2  2  11   9   4
7  4 10 11  2  3 10  4  8  7   9   9   8
8  5 11  6  7  8  7 11 10  2   6   9   5
````

10.
````R
> NewMatrix<-matrix(NA,nrow=8,ncol=13)
> NewFrame<-data.frame(NewMatrix)
> NewFrame[,1:12]<-MyMatrix
> NeFrame[,13]<-Sums>70
> NewFrame
  X1 X2 X3 X4 X5 X6 X7 X8 X9 X10 X11 X12   X13
1 10  6  7  3 11  8 11  4  5   8   6  10  TRUE
2 11  2 11 10  6  9 10  3 10  11   8   5  TRUE
3  5  5  2  8  6  8 11 10  5   6   7   7  TRUE
4 11 11  3  5 10  8  5  7  2   3   6   9  TRUE
5 10  2  9  5  7  3  7  3  5   5   3   2 FALSE
6 10  8  3 10  4  8  9  2  2  11   9   4  TRUE
7  4 10 11  2  3 10  4  8  7   9   9   8  TRUE
8  5 11  6  7  8  7 11 10  2   6   9   5  TRUE
````
