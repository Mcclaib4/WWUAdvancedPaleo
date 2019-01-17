**Section 1**

1. **?**
````R
replace=
````
ensures that no element occurs twice

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

9. **?**
````R

````

10. **?**
````R
> which(apply(MyMatrix,1,sum)>70)
[1] 1 2 3 4 6 7 8

````
