Why you need to integrate WebPivotTable?

Follow Quick Start Guide, you can quickly install an individual WebPivotTable application. It includes a NodeJS web server internally so that you can start to use it right away and it is totally free. But if you have any list below requirements, you need to think about WebPivotTable Integration:

You want to embed WebPivotTable into your existing web application or website.
You want to embed WebPivotTable into your existing software product or SaaS solution.
You want to customize user interface and behaviours of WebPivotTable.
You want to load source data programmatically.
You want to use any kind of source data from your back end servers.
You want to save whole data analytic to the server so that it can be easily reopened.
You want to use updated source data with your pre-saved pivot operations.
You want to share source data and data analytic with others automatically.
You want to add user authentication and authorization on using WebPivotTable.
You want to hide "help" and "About" buttons on top right bar.
WebPivotTable is a Web version pivot table implementation, the core of WebPivotTable is a pure javascript component. You can integrate this component into any web application or web site, just like other javascript libraries. There is no binding of this component with any particular back end web server. You can use it together with any web server back end technology, for example, NodeJs, PHP, Python, Ruby, Java, C#, etc. You can even integrate it into your own software or your SaaS (Software as a Service) solution, we have an OEM/SaaS license for you to deliver your integrated software or SaaS solution to any number of your customers.

WebPivotTable core component had been carefully designed to meet all kinds of integration. There are lots of customize options for you to customize the user interface and behaviours, we also provide a lots of APIs(Application Programming Interfaces) for you to load any kinds of your source data or load your pre-saved WPT format files.

How to integrate WebPivotTable?

Get a proper WebPivotTable edition

To integrate WebPivotTable you need a WebPivotTable component edition. Go Download Page to request a trial version or Contact us to purchase a license of commercial version.

Copy all necessary files to Web Server

After you get WebPivotTable component edition packaged zip file(either trial version or commercial version), upzip this file to any of your local directory, then copy the whole content under public subdirectory to your web server's public directory (you can copy all contents directly under web server public root directory or under some subdirectory of public root directory).

Import all necessary css files and javascript files

In html file of your application's index page or page which will integrate WebPivotTable component, import all necessary css files and javascript files like below sample:



<!DOCTYPE HTML>
<html>
<head>
    <style type="text/css">
        html, body, #wpt-container {width:100%;height:100%;}
    </style>

    <!-- Step 1 import wpt.css file into the page -->
    <link rel='stylesheet' href='brightsea/wpt/wpt.css'>    

    <!-- Step 2 import third party javascript libraries-->    
    <script type="text/javascript" src="lib/filepicker/index.js"></script>
    <script type="text/javascript" src="lib/jquery/dist/jquery.min.js"></script>
    <script type="text/javascript" src="lib/highcharts-release/highcharts.js"></script>
    <script type="text/javascript" src="lib/highcharts-release/highcharts-3d.js"></script>
    <script type="text/javascript" src="lib/highcharts-release/highcharts-more.js"></script>
    <script type="text/javascript" src="lib/grouped_categories/grouped-categories.js"></script>
    <script type="text/javascript" src="lib/jszip/dist/jszip.min.js"></script>
    <script type="text/javascript" src="lib/js-xlsx/dist/ods.js"></script>
    <script type="text/javascript" src="lib/js-xlsx/dist/xlsx.min.js"></script>
    <script type="text/javascript" src="lib/papaparse/papaparse.min.js"></script>

    <!-- Step 3 import wpt.js file into the page with correct dojo config-->
    <script type="text/javascript" src="brightsea/wpt/wpt.js"  
        data-dojo-config="async:1, baseUrl: 'brightsea/dojo/'"></script> 

    <!-- Step 4 create WebPivotTable object after dojo domReady-->
    <script type="text/javascript">
        require(["wpt/WebPivotTable","dojo/domReady!"], function(WebPivotTable){
            new WebPivotTable({},"wpt-container");
        });
    </script>
</head>

<!-- Step 5 add "claro" class to body tag-->
<body class="claro">
    <div id="wpt-container"></div>
</body>
</html>

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
 
<!DOCTYPE HTML>
<html>
<head>
    <style type="text/css">
        html, body, #wpt-container {width:100%;height:100%;}
    </style>
 
    <!-- Step 1 import wpt.css file into the page -->
    <link rel='stylesheet' href='brightsea/wpt/wpt.css'>    
 
    <!-- Step 2 import third party javascript libraries-->    
    <script type="text/javascript" src="lib/filepicker/index.js"></script>
    <script type="text/javascript" src="lib/jquery/dist/jquery.min.js"></script>
    <script type="text/javascript" src="lib/highcharts-release/highcharts.js"></script>
    <script type="text/javascript" src="lib/highcharts-release/highcharts-3d.js"></script>
    <script type="text/javascript" src="lib/highcharts-release/highcharts-more.js"></script>
    <script type="text/javascript" src="lib/grouped_categories/grouped-categories.js"></script>
    <script type="text/javascript" src="lib/jszip/dist/jszip.min.js"></script>
    <script type="text/javascript" src="lib/js-xlsx/dist/ods.js"></script>
    <script type="text/javascript" src="lib/js-xlsx/dist/xlsx.min.js"></script>
    <script type="text/javascript" src="lib/papaparse/papaparse.min.js"></script>
 
    <!-- Step 3 import wpt.js file into the page with correct dojo config-->
    <script type="text/javascript" src="brightsea/wpt/wpt.js"  
        data-dojo-config="async:1, baseUrl: 'brightsea/dojo/'"></script> 
 
    <!-- Step 4 create WebPivotTable object after dojo domReady-->
    <script type="text/javascript">
        require(["wpt/WebPivotTable","dojo/domReady!"], function(WebPivotTable){
            new WebPivotTable({},"wpt-container");
        });
    </script>
</head>
 
<!-- Step 5 add "claro" class to body tag-->
<body class="claro">
    <div id="wpt-container"></div>
</body>
</html>
 
Notes:
Above sample code assumed you put all WebPivotTable contents under the web server public root directory. If you put them under some subdirectory of public root directory, you need change the path of each css and javascript file accordingly, include the value of "baseUrl" parameter in "data-dojo-config" attribute when import wpt.js file.

If you don't need to support loading files from cloud drives, you can remove import statement of "lib/filepicker/index.js".

If you have JQuery library imported in your page somewhere else already, you can remove import statement of "lib/jquery/dist/jquery.min.js". Or if you would like to use some CDN JQuery library to improve page loading performance, you can change the path to CDN JQuery URL.

If you have Highcharts library imported in your page somewhere else already, you can remove those import statements of "lib/highcharts-release/...". Or if you would like to use some CDN Highcharts library to improve page loading performance, you can change the path to CDN Highcharts URL.

Remember to add a "claro" class to body tag

You can put "wpt-container" div anywhere on your page, remember to style it with your desired width and height.

Create and Initialize WebPivotTable Object

After all necessary css and javascript files imported into page, you can create and initialize a WebPivotTable object when page dom is ready. You can do this just like above sample code, or you can do it anywhere in your own code, for example, do it in some event handlers:



    function myEventHandler(evt){
           
        ...

        require(["wpt/WebPivotTable"], function(WebPivotTable){
            var wpt = new WebPivotTable({},"wpt-container");
        });

        ...
    }

1
2
3
4
5
6
7
8
9
10
11
12
 
    function myEventHandler(evt){
           
        ...
 
        require(["wpt/WebPivotTable"], function(WebPivotTable){
            var wpt = new WebPivotTable({},"wpt-container");
        });
 
        ...
    }
 
Next?

You can continue to read Technical Documents for all technical details of WebPivotTable, include all customize options and all APIs. If you have any questions, you can get answers at Q&A Page.

Primary Sidebar
Pivot Table Introduction
WebPivotTable Introduction
WebPivotTable Editions Introduction
Quick Start Guide
WebPivotTable Integration Guide
TECHNICAL DOCUMENTS

Customize Options
APIs
WPT File Format
Changes History