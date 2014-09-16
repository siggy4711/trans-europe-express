---
title       : Trans Europe Express
subtitle    : Traveling Sales Man application using GoogleMaps
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

The days of lowcost fuels are behind us due to increasing demand and increasing complexity of mining. As a logical result travel costs are also increasing and therefore reducing these cost bears more weight in improving business profits.

Trans Europe Express(TEE) will help businesses in reducing car travel costs by determining the shortest route of a trip to multiple cities.

The traveler can select the cities that have to be visited and the starting point, TEE will then show the shortest roundtrip in a table including distances. We will show the information displayed by TEE in the following demonstration.

An online prototype is available at [Trans Europe Express](https://siggy4711.shinyapps.io/project/)

--- .class #id 

## Demonstration

Assume that the cities to be visited are

```r
cities
```

```
## [1] "Brussel"  "Berlin"   "London"   "Paris"    "Madrid"   "Lissabon"
## [7] "Prague"
```
and the trip starts in 

```
## [1] "Madrid"
```
Then TEE will derive the shortest route and for this route the sequence is

```r
cities[tour]
```

```
## [1] "Brussel"  "Paris"    "London"   "Berlin"   "Prague"   "Madrid"  
## [7] "Lissabon"
```


--- .class #id 

### Demonstration, City to City output
The roundtrip from city to city is orderly displayed in a table, the last line of the table shows the total trip length



|From     |To       |Distance |
|:--------|:--------|:--------|
|Brussel  |Paris    |308.304  |
|Paris    |London   |456.301  |
|London   |Berlin   |1090.811 |
|Berlin   |Prague   |350.614  |
|Prague   |Madrid   |2235.864 |
|Madrid   |Lissabon |628.275  |
|Lissabon |Brussel  |2036.991 |
|Brussel  |Brussel  |7107.16  |

--- .class #id 

### Demonstration, map output
A clear picture shows the roadtrip on a map.
![plot of chunk unnamed-chunk-6](assets/fig/unnamed-chunk-6.png) 









