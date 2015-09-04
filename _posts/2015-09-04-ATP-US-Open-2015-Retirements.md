---
layout: post
title: Trends in Match Duration and Retirements - US Open 1999 - 2014
comments: true
---

<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataScatterChartID68b756309fa () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 1991,
6 
],
[
 1992,
7 
],
[
 1993,
7 
],
[
 1994,
4 
],
[
 1995,
4 
],
[
 1996,
4 
],
[
 1997,
6 
],
[
 1998,
7 
],
[
 1999,
7 
],
[
 2000,
3 
],
[
 2001,
3 
],
[
 2002,
10 
],
[
 2003,
5 
],
[
 2004,
7 
],
[
 2005,
4 
],
[
 2006,
2 
],
[
 2007,
8 
],
[
 2008,
6 
],
[
 2009,
4 
],
[
 2010,
8 
],
[
 2011,
11 
],
[
 2012,
4 
],
[
 2013,
5 
],
[
 2014,
10 
] 
];
data.addColumn('number','year');
data.addColumn('number','walkover');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartScatterChartID68b756309fa() {
var data = gvisDataScatterChartID68b756309fa();
var options = {};
options["allowHtml"] = true;
options["width"] =   1000;
options["height"] =    600;
options["trendlines"] = {0:{type: 'exponential'}, 1: {}};
options["hAxis"] = {format: '####', title: 'Year', minValue : 1990, maxValue: 2014, 
			ticks: [1990, 1992, 1994, 1996, 1998, 2000, 2002, 2004, 2006, 2008, 2010, 2012, 2014]};
options["vAxis"] = {title: 'Total'};


    var chart = new google.visualization.ScatterChart(
    document.getElementById('ScatterChartID68b756309fa')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartScatterChartID68b756309fa);
})();
function displayChartScatterChartID68b756309fa() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartScatterChartID68b756309fa"></script>
 
<!-- divChart -->
  
<div id="ScatterChartID68b756309fa" 
  style="width: 1000; height: 600;">
</div>
 <div><span>Data: usopen_retirement[usopen_retirement$year > 1990, c("year", "walkover")] &#8226; Chart ID: <a href="Chart_ScatterChartID68b756309fa.html">ScatterChartID68b756309fa</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.5.9</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.2.1 (2015-06-18) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; <a href="https://google-developers.appspot.com/chart/interactive/docs/gallery/scatterchart">Documentation and Data Policy</a>
</span>
</div>

{% include twitter_plug.html %}
