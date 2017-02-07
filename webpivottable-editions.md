Currently, there are two editions of WebPivotTable: free edition and component edition.

## WebPivotTable Free Edition

Free edition has all functionalities of WebPivotTable except the ability to be integrated into other web applications or web sites. It includes a [NodeJS](http://nodejs.org/) back end web server so that it can be used right after installation. The installation is quite easy and no technical background required. Follow [Quick Start Guide](/quick-start-guide.md), anybody can install a useful WebPivotTable application in few minutes.

_WebPivotTable Free Edition is totally free to any person or any company, either for personal use or for commercial use. You can go to [Download Page](http://webpivottable.com/download) to download a copy of this edition, install it on a personal computer or a cooperation server and use it right away. No license needed._

The most popular use case of free edition is to analyse data from data files. Through intuitive user interface, you can load source data from a data file existing on your local drive, cloud drives or on a web server and be published as a internet link. The file format can be most popular data file format, like CSV, TSV, Excel and Google Spreadsheet.

Another use case of free edition is to use it as a front end client for any OLAP(Online Analytical Processing) server, like Microsoft Analytic Service and Mondrian open source OLAP server. Although each OLAP server may provide its own front end client, for example, Excel is front end client for Microsoft Analytic Service and JPivot if a front end client for Mondrian OLAP Server, WebPivotTable can provide better user experience than those clients since it is web based and has very intuitive user interface. Another advantage of using WebPivotTable is it is free and follows XMLA standard so that it doesn't bind with any particular OLAP server.

WebPivotTable free edition allows you to save your analysis in a WPT format file and load this file later. This is great for sharing data analytic with others. You can send this file to anybody else and they can open it through any WebPivotTable application, either it is the same WebPivotTable application with you, or any other installed WebPivotTable applications. Once opened, everything resume back to exactly the same as when you save the file.

## WebPivotTable Component Edition

Component edition includes all functionalities of free edition, but add the support of customize options and APIs for developers to integrate it into any web application or web site. Follow [Integration Guide](/webpivottable-integration-guide.md), a technician with little web development background can make a quick integration.

WebPivotTable component edition is not free and any commercial use of it should purchase a license. Before making a purchase, you can go to Download Page to request a trial version of this edition by filling up a simple form.

Like free edition, there is a NodeJS back end web server included in component edition package. This back end server is optional and all back end services' source codes are opened, you can copy those codes into your own back end server if your web application is based on NodeJs platform as well. For other back end application platforms, like PHP, Python, Ruby, Java, C#, you can replace those services with your own implementations. Technical Documents provides all technical details about advanced integration, includes how to implement these services.

A typical use case of component edition is to load source data from server side. Component edition provides APIs for integration developer to load data into WebPivotTable programmatically, either directly from data file URL links or web services, or first retrieve data from server side to front end then load it as a data array. These APIs open doors to load any kinds of enterprise data, especially data stores in database system. End users can all access these data without knowing the storage details.

Another use case of component edition is to save all data analysis to the server and reload it by anybody else from the server. This makes sharing data analytic within enterprise or organization quite easy.

Embed WebPivotTable into other BI products or SaaS solutions is also a popular use case. Not only the user interface of WebPivotTable component can be customized, but also it can communicate with other parts of products or solutions bidirectionally.