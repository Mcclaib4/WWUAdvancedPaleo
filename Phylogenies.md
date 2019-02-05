**Part I**

**1.** 

Based on my observations, I would divide the specimens into the following species:

Sp 1) 1,8,21

Sp 2) 2,4,5,14,25

Sp 3) 3,7,9,10,13,15,17,19,23

Sp 4) 6,12,18

Sp 5) 11,20

Sp 6) 16,24

Sp 7) 22

**2.**

1) evolute coiling, distinct ridges, 
2) involute coiling, 
3) evolute coiling, 
4) involute coiling, 
5) involute coiling, 
6) involute coiling, knobby, distinct ridges, 
7) evolute coiling, 
8) evolute coiling, distinct ridges, 
9) evolute coiling, 
10) evolute coiling, 
11) evolute coiling, distinct ridges, widely spaced ridges, suture lines (ceratitic), 
12) evolute coiling, knobby, distinct ridges, 
13) evolute coiling, 
14) involute coiling, 
15) evolute coiling, 
16) evolute coiling, suture lines (goniatic), 
17) evolute coiling, 
18) evolute coiling, knobby, distinct ridges, 
19) evolute coiling, 
20) evolute coiling, distinct ridges, widely spaced ridges,
21) evolute coiling, distinct ridges, 
22) involute coiling, suture lines (goniatic), 
23) evolute coiling, 
24) evolute coiling, suture lines (goniatic), 
25) involute coiling,

**3.**

**?**

**4.**

**?**

**Part II**

**Sub.1**

**1.**

````R
> attributes(plethodon)
$names
[1] "land"    "links"   "species" "site"   
[5] "outline"
````

**2.**

````R
> typeof(plethodon)
[1] "list"
````

**3.**

````R
> plethodon$land
, , 1

          [,1]     [,2]
 [1,]  8.89372 53.77644
 [2,]  9.26840 52.77072
 [3,]  5.56104 54.21028
 [4,]  1.87340 52.75100
 [5,]  1.28180 53.18484
 [6,]  1.24236 53.32288
 [7,]  0.84796 54.70328
 [8,]  3.35240 55.76816
 [9,]  6.29068 55.70900
[10,]  8.87400 55.25544
[11,] 10.74740 55.43292
[12,] 14.39560 52.75100
````
**Sub2**

**1.**
````R
"land"
````

**2.**
````R
> ProcrustesHummingbirds<-gpagen(hummingbirds$land)
````

**3.**
````R
plotTangentSpace(ProcrustesHummingbirds$coords, warpgrids = FALSE, verbose = FALSE)
````

**4.**
3 species
