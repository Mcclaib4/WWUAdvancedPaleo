**Problem Set I**

**1.**

653, 177, 396, and 121 respectively.
````R
> apply(PresencePBDB,1,sum)
````

**2.**

29

**3.**
````R
> PresencePBDB[,"Mytilus"]
````
Early Devonian; Early, Middle, & Late Triassic; Early, Middle, & Late Jurassic; Early & Late Cretaceous; Paleocene; Eocene; Oligocene; Miocene; Pliocene; Pleistocene.

**4.**

Middle & Late Devonian, Mississippian, Pennsylvanian, Cisuralian, Guadalupian, and Lopingian can be infered to have *Mytilus* because there are members of *Mytilus* above and below this section in the fossil record.

**Problem Set II**

**1.**
````R
> P<-length(which(PresencePBDB["Pleistocene",] == 1 & PresencePBDB["Miocene",] == 0))
> M<-length(which(PresencePBDB["Miocene",] == 1 & PresencePBDB["Pleistocene",] == 0))
> P_M<-length(which(PresencePBDB["Miocene",] == 1 & PresencePBDB["Pleistocene",] == 1))
> P_M/(P+M+P_M)
[1] 0.8350825
````
