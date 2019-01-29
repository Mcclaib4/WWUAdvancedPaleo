1.  **Conduct a GPA on your data and examine the plot. What information does it visualize?**
The GPA plots all the collected data and provides an averaged location for each landmark.

2.  **What does this information tell you about the original set of Osteostracan skulls?**
The data indicates that specimen dimensions vary considerably.

3.  **According to the plot, which two specimens are LEAST similar in terms of PC 1?**
Specimens 8 and 29 are the least similar in terms of PC1.

4.  **Embed the ````R .png ```` files for these two specimens in your MarkDown file and describe the visual differences between them. What factor does PC 1 seem to describe?**

![Osteo8](https://github.com/Mcclaib4/Osteostracans/blob/master/osteostracans/Boreaspis_ceratops.png)
![Osteo29](https://github.com/Mcclaib4/Osteostracans/blob/master/osteostracans/Zychiaspis_siemiradzkii.png)

The rostral extension of *Boreaspis ceratops* is prolonged with near parallel lateral margins where as *Zychiaspis siemiradzkii* has no rostral extension. The Posterolateral margin of the shield of both specimens are relatively equal in length however the curvature direction  is quite different. *Boreaspis ceratops* has no curve, while *Zychiaspis siemiradzkii* has a medial curve. In *Boreaspis ceratops*, lateral fields extend onto the abdominal division posterior to the pectoral sinus and the pectoral sinus is anterior in relation to the level of orbits. In *Zychiaspis siemiradzkii*, lateral fields' extend to cornua and the pectoral sinus is posterior in relation to the level of orbits. PC1 describes **?**

5.  **According to the plot, which two specimens are least similar in terms of PC 2?**
*Belonaspis puella* & *Benneviaspis anglica* are least similar in terms of PC2.

6.  **Embed these images in your MarkDown file and describe the visual differences between them. What factor does PC 2 seem to describe?**

![Osteo3](https://github.com/Mcclaib4/Osteostracans/blob/master/osteostracans/Belonaspis_puella.png)
![Osteo4](https://github.com/Mcclaib4/Osteostracans/blob/master/osteostracans/Benneviaspis_anglica.png)

**?**

7.  **Create a simple bar plot of the proportion of variance and embed the figure in your Markdown file.**

![BarPlot](https://github.com/Mcclaib4/Osteostracans/blob/master/osteostracans/PropVar_barplot.png)

8.  **Try plotting PC 1 and PC 18. Include the code that you used in your MarkDown file, and embed the resuting plot. Why does it look like all the specimens fall almost perfectly along a single line parallel to the major axis?**

````R
> osteoPCA <- plotTangentSpace(osteoGPA$coords, axis1 = 1, axis2 = 18, label = TRUE)
````

![PC1/PC18_Osteo](https://github.com/Mcclaib4/Osteostracans/blob/master/osteostracans/PC1_PC18_Osteo.png)

