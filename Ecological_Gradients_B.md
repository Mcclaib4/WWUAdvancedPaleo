**1.**
````R
> Ordovician <- velociraptr::downloadPBDB(Taxa=c("Animalia"),StartInterval="Ordovician",StopInterval="Ordovician")
````

**2.**
````R
> Ordovician <- velociraptr::cleanTaxonomy(Ordovician,"genus")
````

**3.**
