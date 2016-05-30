# Chartin.js
Chartin.js is a JavaScript module for creating `Bar Charts`, `Histograms`, `Pie Charts` and `Line Charts`

Contributions, policies and releases are managed under an open governance model.

##Installation
###Bower
Use `bower` to install:
```
bower install chartinjs
```

##Application
Add it to the `scripts` tag on your html header:
```
<script src='./bower_components/chartinjs/index.js'></script>
```
Once you've added it at the head of your page create a div where the canvas is to be drawn and give it `id="chartDiv"`. This is to be the chart container for the canvas element. 
You can add some CSS styling for the div (below is an example):
```
#chartDiv {
  width: 500px;
  margin-top:50px;
  background: #bbbbbb;
  border-left: 1px solid #555555;
  border-bottom: 1px solid #555555;
  height: 200px;
  left: 50%;
  margin-left: -200px;
  overflow: hidden;
}
```
To use the library:
```
function bar() {
  var dataset = receiveInput();
  drawBarChart(dataset, null);
}

function line() {
  var dataset = receiveInput();
  drawLineChart(dataset, null);
}

function hist() {
  var dataset = receiveInput();
  drawHistogram(dataset, null);
}

function pie() {
  var dataset = receiveInput();
  drawPieChart(dataset, null);
}

```
The `dataset`, is an array that is used to input into the drawing functions.
### Screen shots
Pie Chart
![Screenshot](/images/pie_chart.png)

Line Chart
![Screenshot](/images/line_chart.png)

Bar Chart
![Screenshot](/images/bar_chart.png)

Histogram
![Screenshot](/images/histogram.png)
