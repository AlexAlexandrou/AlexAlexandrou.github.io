---
layout: post
title: Cyberthreat and Vulnerability awareness for Smart Cities
subtitle: Visualizations providing threat intelligence for Smart Cities
tags: [Splunk, Cybersecurity, Smart Cities]
thumbnail-img: /assets/img/smart-city.png
share-img: /assets/img/smart-city.PNG
comments: true
---

For this project, different datasets containing data on countries and their smart cities as well as the vulnerabilities that apply to them and their severity were used to create visualizations in Splunk.  
The visualizations vary from each other and are placed on different dashboards:
* Countries: Contains visualizations in regards to the countries contained in the datasets.
* Cities: Similarly to the Countries dashboard, it contains all the visualizations regarding the Smart Cities.
* Vulnerabilities: All the visualizations about the vulnerabilities are displayed such as their description, their attack methods, severity and the systems they can exploit.

Additionally, dashbaords containing visualizations about specific assets were also created:
* Selected City
* Selected Vulnerability

## Countries Dashbaord

![image](/assets/img/fullscreen-countries.PNG){: .mx-auto.d-block :}

In this dashboard, all the recorded countries and their information can be found. Additionally, the visualizations can be filtered to show only information regarding a specific country that the user selects.  
In the presented example, the UK is selected.


## Cities Dashbaord

![image](/assets/img/fullscreen-cities.PNG){: .mx-auto.d-block :}

For this dashbaord, in addition to the information contained by default about the cities, the user can select a specific city that they'd like to display its information, as well as select multiple cities from the "top 10 cities with the most vulnerabilities" to see what vulnerabilities they share and assist with information sharing and threat intelligence.  
In this example, London is displayed as the selected city and following, the pairs of London, Paris and Amsterdam are selected to display their shared vulnerabilities.


## Vulnerabilities Dashbaord

![image](/assets/img/fullscreen-vulns.PNG){: .mx-auto.d-block :}

In this dashboard, the user can filter the visualizations to show only the vulnerabilities that apply to a selected attack method. Also, a specific vulnerability can be selected to show the cities that contain it and the protocols it violates. Following, the users can select a specific protocol to display all the vulnerabilities that violate it.  
In this example, "Denial of Service" is selected as the exploit attack,  "CVE-2017-11145" as the vulnerability and "ProConOS" as the violated protocol.


## Selected City Dashbaord

![image](/assets/img/fullscreen-selected-city.PNG){: .mx-auto.d-block :}

This dashboard can be accessed when a city is selected from the main dashbaords. It shows a map in which its country is highlighted and is followed by all its details and the vulnerabilities it has.  
This example shows "London" as the selected City.


## Selected Vulnerability Dashbaord

![image](/assets/img/fullscreen-selected-vuln.PNG){: .mx-auto.d-block :}

Similarly to the Selected City dashbaord, this one can be accessed by selected a vulnerability from the main dashboards. It shows its details at the top followed by its exploitable attacks and the protocols it violates. Following all its details and properties, it displays all the cities that are affected by it.

{: .box-note}
If a user clicks on the vulnerability on the first panel, they are transferred to NIST's National Vulnerability Database where additional details about it can be found as well as different references where its credibility can be assessed

