**1.**
````R
> Ordovician <- velociraptr::downloadPBDB(Taxa=c("Animalia"),StartInterval="Ordovician",StopInterval="Ordovician")
````

**2.**
````R
> Ordovician <- velociraptr::cleanTaxonomy(Ordovician,"genus")
````

**3.**
````R
> locationOrdovician <- velociraptr::presenceMatrix(Ordovician,Rows="genus",Columns = "geoplate")
> locationOrdovician<-velociraptr::cullMatrix(locationOrdovician,Rarity=2,Richness=25)
````
**4.** **???**
````R
> OrdovicianDCA<-vegan::decorana(locationOrdovician)
> plot(OrdovicianDCA,display="sites")
````
