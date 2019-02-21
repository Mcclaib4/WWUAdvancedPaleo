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

**2.**
````R
> 1-(P_M/(P+M+P_M))
[1] 0.1649175
````

**3.**
````R
> vegdist(PresencePBDB,method="jaccard")
````

**4.**

(Pleistocene/Pliocene)=0.12933754, (Pleistocene/Miocene)=0.16491754,
(Pleistocene/Oligocene)=0.27575758, (Pleistocene/Eocene)=0.21428571,
(Pleistocene/Paleocene)=0.43750000, (Pliocene/Miocene)=0.09036145,
(Pliocene/Oligocene)=0.20091324, (Pliocene/Eocene)=0.14202050,
(Pliocene/Paleocene)=0.37826087, (Miocene/Oligocene)=0.16265060,
(Miocene/Eocene)=0.08918129, (Miocene/Paleocene)=0.32075472,
(Oligocene/Eocene)=0.18573551, (Oligocene/Paleocene)=0.40625000,
(Eocene/Paleocene)=0.32173913

Miocene and Eocene are the most dissimilar.
