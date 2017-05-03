---
layout: blog
tags: open data, housing, planning, rwc, harker
author: robert_harker
published: false
title:  "Using Open Data to calculate Redwood City's upcoming housing shortfall"
date:   2016-05-23 12:00:00
---

## Using Open Data To Calculate Redwood City's Upcoming Housing Shortfall

San Mateo County is in the midst of the largest housing crisis in its history.  The crisis is a direct result of planning choices over the last 5 years.  Building office space for new employees at a much-much faster rate than building the new housing units needed to house these new employees.  County wide the ratio is 5-9 times office space to housing units for the last 5 years (I need to fact check).  I have been talking with Michelle Littlefield, our brigade captain about this.  Her day job is a city planner for Redwood City.  In our conversations I realized people are not talking about the housing shortage in the most useful way.  The conversation is about high rents, below market rate units and housing for teachers, police and fire crews.

I think a different and more useful approach is to figure out how many new housing units need to be built to support the new office space that is currently being planned or being built.  If we know how many housing units are needed and how many units are actually planned, then we can figure out the shortfall.

I did this and the numbers are scary:  
* 3 million square feet (sq ft) of new office space.  
  Which will dd over 10,000 people to the city's workforce.

* These 10,000 employees will need over 6,800 new housing units.  

* Only 3226 housing units are planned.  

* This leaves a shortfall of almost 3,600 units.

In other words, Redwood City is building less than half the needed housing for workers who will be added to the city's workforce in the next 5 years.  This does not take into account any existing shortfall for completed projects.

### Calculating workforce growth and housing requirements using government public data

I was able to accurately calculate workforce numbers and housing unit needs using Redwood City's government public data.  Using Redwood City's excellent [public GIS (Global Information System) web site](http://webgis.redwoodcity.org) I was able to find the actual square footage of new office space and number of hosing units currently planned or being built.  Using the City GIS website's Planning Projects feature I could see the current project information in a nice, easy to understand format.

* There are 9 commercial and 3 mixed use projects with new office space.  
  The combined total new office space is '3,068,000 sq ft'.  
  New retail space and hotel or remodel only projects are ignored.

* There are 18 residential and 3 mixed use projects with new housing  
  with a total of '3226 housing units'.  
  90% of these units are high density rental apartments.

My two base assumptions are:
* For every 300 sq ft of office space  
  a new person will be added to city's workforce.
* A unit of housing will house 1.5 employees  
  or 3 employees per 2 housing units.

### The Calculations:
Commercial office space (from RWC Planning Projects page)
Total sq ft: 3,068K	300 sq ft per employee = 10,226 new employees

Assuming 1.5 employees per housing unit:
10,226 employees = 6,817 housing units needed

Housing totals: (from RWC Planning Projects page)
36 homes	169 townhomes	2930 apartments		91 condominiums
total 3226 housing units

If 6,817 housing units are needed, but only 3226 are planned, then the housing shortfall is 3500 units.

The sad fact is that the families and individuals that will be displaced will be low income people doing mundane work as receptionists, waitresses/waiters, janitors, cashiers, stock clerks or day laborers.

@@ The 2 to 1 ratio of housing to office space square footage ratio

To support office space with housing for employees you need to build twice as many sq ft of housing as office space.  
  Build a million sq ft of office space,  
  You need to build two million sq ft of housing.

*  10,000 new employees @ 300 sq ft per employee  
  = 3 million sq ft new office space.  
*  10,000 new employees @ 2/3 housing unit per employee (3 employee / 2 housing units)  
  = 6,666 housing units.
*  6,666 hosing units @ 900 sq ft per unit  
  = 6 million sq ft of new housing required.

The 1 to 2 ratio of new office to new housing verified:  
* 3 million sq ft of new office space requires six million sq ft of new housing.

## Public data but not government Open Data

The data is available in a very easy to use form on Redwood City's excellent GIS web portal.  But the data is locked into drop down data boxes.  Sometimes the data was in the actual plans.  I had to scrape (hand enter) the data to find my facts.

If the data was in a machine readable Open Data format accessible via a public http base API, I could have crafted an API query that would return the current results in realtime.  A simple web or mobile app could have a query form that with would generate the API query and display the results on a map, in a table or graph.

* Redwood City's public GIS portal:  
  [http://webgis.redwoodcity.org](http://webgis.redwoodcity.org)  
  The nicest Open Data portal I have seen.

## Fun fact about RWC's potential near term population growth:

* The estimated Redwood City Population in 2014: 83,000.

* Assuming 1.5 new residents per new employee (many have families)  
  10,000 new employees = 15,000 new residents.

Which is an 18% increase in the population of Redwood City.

