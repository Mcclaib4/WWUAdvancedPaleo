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
> quantile(ResampledMeans, c(.025, .975))
    2.5%    97.5% 
21.71473 26.69090 
````

**11.**

The numbers are the upper and lower confidence intervals because
the probability that the mean from any given sample will be closer
to the actual mean than these numbers is 97.5.

**Problem Set III**

**12.**

It is highly likely that *Lucina* is extant.

**13.**
````R
> estimateExtinction(Dallarca[,"min_ma"],0.95)
Earliest   Latest 
 2.58800 -3.88749
 ````
 
 **14.**
 
 There is a 95% liklihood that *Dallarca* is extant.
 
 **15.**
 
 Statistical analysis indicates that *Dallarca* is likely to be extant and with it being a bivalve it is not absurd to think that it is a Lazarus taxa.
 
 **Problem Set IV**
 
 **16.**
 
 Taxa are, generally, relatively rare early and late in their period of existence, with a period of relative abundance somewhere in the middle. It is not randomly distributed throughout.
 
 **17.**
 
 Likelihood of preservation can change drastically through a stratigraphic section depending on the erossional and depositional conditions of the region during the time period in question.
 
 **Problem Set V**
 
 **18.**
````R
> nrow(ExtantData)
[1] 62114
> nrow(DataPBDB)
[1] 71215
> nrow(DataPBDB)-nrow(ExtantData)
[1] 9101
````

**19.**
````R
> length(unique(DataPBDB[,"genus"]))
[1] 1075
> length(unique(ExtantData[,"genus"]))
[1] 544
> length(unique(DataPBDB[,"genus"]))-length(unique(ExtantData[,"genus"]))
[1] 531
````
