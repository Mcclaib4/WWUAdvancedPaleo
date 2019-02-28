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
Beyond this point is when the graph didn't look right, but I haven't figured out how to fix it.
