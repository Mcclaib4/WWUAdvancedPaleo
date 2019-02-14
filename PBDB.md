**Part 1**

**1.**

704

**2.**

24429

**3.**

Strophomenata, Strophomenidae, *Strophomena planumbona*

**4.**

United States

**5.**

Ordovician

**6.**

Liberty

**Part II**

**1.**

The different colors represent different periods of geologic time.

**2.**

Abra is found in the United States, the United Kingdom, and Belgium.

**3.**

Cincinnati, OH.

**4.**

Ordovician

**5.**

Parallel

**6.**

Myalinida

**Part III**

**1.**

https://paleobiodb.org/data1.2/occs/list.json?
datainfo&rowcount&base_name=Ambonychia&strat=LexingtonLimestone

**2.**

https://paleobiodb.org/data1.2/occs/list.csv?
datainfo&rowcount&base_name=Mammalia&interval=Paleocene,Oligocene

**3.**

https://paleobiodb.org/data1.2/occs/opinions.csv?
datainfo&rowcount&base_name=Testudines&interval=Mesozoic&op_type=all

**4.**

https://paleobiodb.org/data1.2/occs/opinions.csv?
datainfo&rowcount&base_name=Aves,Marsupialia,Sirenia&cc=US&op_type=all

**5.**

https://paleobiodb.org/data1.2/taxa/opinions.csv?
datainfo&rowcount&base_name=ficus&rank=genus&op_type=all

**6.**

Gastrocoptidae

**7.**

125-113 Ma.

**8.**

50.3 - 46.2 Ma

**9.**

Tropics

**10.**

Kotodzha Fm. and Raiga Fm.

**Part IV**

**1.**
````R
> Mammut<-fread('https://paleobiodb.org/data1.2/colls/
list.csv?base_name=Mammut&interval=Pliocene')
````

**2.**
````R
> dim(Mammut)
[1] 70 14
````

**3.**

collections

**4.**

*Mammut*, Mastadon, Pliocene

**5.**
````R
> Mammut<-fread('https://paleobiodb.org/data1.2/colls/list.csv?
base_name=Mammut&interval=Miocene,Pleistocene')
````

**6.**
````R
> Mammut<-fread('https://paleobiodb.org/data1.2/colls/list.csv?
base_name=Mammut&interval=Miocene,Pleistocene&show=paleoloc')
````
**Part V**

````R
downloadPBDB<-function(taxon="",interval=""){
return(fread(paste('https://paleobiodb.org/data1.2/occs/list.csv?
base_name=',taxon,'&interval=',interval,sep="")))}
````
