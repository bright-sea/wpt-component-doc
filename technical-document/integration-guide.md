\#\# Integration Guide 



Integrating WPT component into your own web application or web site is quite easy. 

What you need to do is import a css file and some javascript files into your web page.





\#\#\# Quick Start Guide

 

After you get WPT component, you can extract all contents in "public" subdirectory

to your web root directory. Then follow list below steps to import necessary css file

and javascript files into your page.

    

    &lt;!DOCTYPE HTML&gt;

    &lt;html&gt;

    &lt;head&gt;

        &lt;style type="text/css"&gt;

            html, body, \#wpt-container {width:100%;height:100%;}

        &lt;/style&gt;

    

        &lt;!-- Step 1 import wpt.css file into the page --&gt;

        &lt;link rel='stylesheet' href='brightsea/wpt/wpt.css'&gt;    

    

        &lt;!-- Step 2 import third party javascript libraries--&gt;    

        &lt;script type="text/javascript" src="lib/filepicker/index.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/jquery/dist/jquery.min.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/highcharts-release/highcharts.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/highcharts-release/highcharts-3d.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/highcharts-release/highcharts-more.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/grouped\_categories/grouped-categories.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/custom\_events/customEvents.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/jszip/dist/jszip.min.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/js-xlsx/dist/xlsx.min.js"&gt;&lt;/script&gt;

        &lt;script type="text/javascript" src="lib/papaparse/papaparse.min.js"&gt;&lt;/script&gt;

    

        &lt;!-- Step 3 import wpt.js file into the page with correct dojo config--&gt;

        &lt;script type="text/javascript" src="brightsea/wpt/wpt.js"  

            data-dojo-config="async:1, baseUrl: 'brightsea/dojo/'"&gt;&lt;/script&gt; 

        

        &lt;!-- Step 4 create WebPivotTable object after dojo domReady--&gt;

        &lt;script type="text/javascript"&gt;

            require\(\["wpt/WebPivotTable","dojo/domReady!"\], function\(WebPivotTable\){

                new WebPivotTable\({},"wpt-container"\);

            }\);

    	&lt;/script&gt;

    &lt;/head&gt;

    

    &lt;!-- Step 5 add "claro" class to body tag--&gt;

    &lt;body class="claro"&gt;

    	&lt;div id="wpt-container"&gt;&lt;/div&gt;

    &lt;/body&gt;

    &lt;/html&gt;





\* Step1: import wpt.css file into the page

\* Step2: import third party javascript libraries

\* Step3: import wpt.js file into the page with correct dojo config

\* Step4: create WebPivotTable object after dojo domReady

\* Step5: add "claro" class to body tag



