**Problem Set I**

**1.**

Earliest and latest occurences respectively of that species within the specified peiod of time.

**2.**
````R
> tapply(DataPBDB[,"max_ma"],DataPBDB[,"genus"],max)
````

**3.**
````R
> tapply(DataPBDB[,"min_ma"],DataPBDB[,"genus"],min)
````

**4.**
````R
> names(which.max(table(PBDB_occ)))
[1] "Anadara"
````

**5.**
````R
> Anadara<-DataPBDB[which(DataPBDB[,"genus"]=="Anadara"),]
> max(Anadara[,"max_ma"])
[1] 66
> min(Anadara[,"min_ma"])
[1] 0
````

**Problem Set II**

**6.**

The first line isolates the paleolongitude data, while also omitting any entries with missing data.
The second line randomly resamples the occurrences of Lucina, then finds the mean longitude of that resample.

**7.**
````R
> plot(density(ResampledMeans))
````
The distribution looks quite similar to a Gaussian distribution.

**8.**
````R
> mean(ResampledMeans)
[1] 24.27991
````
It is very similar to the original mean.

**9.**
````R
> sort(ResampledMeans,decreasing = FALSE)
````

**10.**
````R
