# Manual eva dashboards

## QUICK START GUIDE
Learn the basics of how Data Studio works
This document presents six key steps to quickly get started using Data Studio.
Data Studio is a flexible tool with which the same results can be achieved in several different ways. The workflow described in this article is just a basic example.

### **1. START WITH A REPORT**
Data Studio reports tell stories through data. These stories can be intended to persuade, provide valuable information, validate decisions, or promote change.
A good report is one in which finding useful information is quick and easy.

### **1.1 KEEP CONTENT UP TO DATE**

Report data is cached to improve performance. When all charts in a report are fetched from cache, a lightning bolt icon appears in the lower left corner. 
Report editors can refresh the cache by clicking the refresh data icon. 

### **1.2 CHANGE THE PERIOD**

Charts have different default periods depending on the data source they are based on. For example, Google Analytics charts show data from the last 28 days by default. The author of a report may have included a filter by period. In this case, you can use it to view a different period: the period control will apply to the entire report. All charts, including those containing date comparisons, will be subject to the new period that you have set.

### **1.3 REFINE THE VIEW DATA**

Reports can include filters. A filter restricts the data that is displayed in the report and includes only the important dimensions.

### **1.4 TURN THE PAGE**

Data Studio reports can have multiple pages. Use the Page menu or the page controls on the toolbar to navigate the report.

### **1.5 SHARE A REPORT**

Use the **File > Share** menu option to invite other users to view or collaborate on a report.
To share a report that someone else has created, you must get permission from the owner.

### **1.6 CUSTOMIZE THE REPORT**

Use the menu option **File > Create** a copy ... to save a version that can be modified.
The report editor must grant you edit permission to modify the copy.
When you log into Data Studio, you will see the main page with the Reports tab selected. All the reports you have access to appear in the center of the screen. The plus *(+)* buttons allow you to create a new blank report or start with a predefined report template.

### **Create a report**

You will then see the report editor, a blank canvas ready for you to tell your story through the data.
In the upper left corner, click 
Select Report

### **Connect to data**

A data source is a specific instance of a connection to your data. Data sources provide the structure (schema) of the fields that you and other report editors can use to create reports. 
When creating a report in Data Studio, you can add an existing data source or create one and add it. You can add as many data sources of any type to your reports as you need.

### **Connect to Analytics sample data**

- In the Add data to report panel, click My data sources.
- Select the [Sample] Google Analytics Data data source.
- In the bottom right, click Add.
- The data source is added to your report.
- A table appears with fields from that data source.
- To change the table's data and style, use the properties panel on the right.
- To rename your report, in the top left, click Untitled Report and enter a new name.

### **Connect to your data**

- In the Add data to report panel, click Connect to data.
- Select the kind of data this data source will provide, for example, Google Analytics or Sheets.
- If prompted, click Authorize to allow Data Studio to access your data on your behalf.
- Provide your account details.
- In the bottom right, click Add.
- A table appears with fields from that data source.
- To change the table's data and style, use the properties panel on the right.
- To rename your report, in the top left, click Untitled Report and enter a new name.

### **Data sources and connectors**

Data sources use connectors to get data from a specific platform, system, or product. Free connectors created by Google allow you to access data from Google Sheets, Google Ads, Google Analytics, and other Google Marketing Platform products.

### **1.7 Add charts and controls to the report**

- In the toolbar at the top of the editor, click Insert and select a chart, or select one from the toolbar.
- Select any of the available charts.
- Move and resize the chart, as desired.
- Add or change the dimensions and metrics by clicking the fields in the properties panel, or dragging and dropping them from the Available Fields panel (to the right of the properties panel).

## 2. OVERVIEW

### **A. conversations**

<table>
<tr>
<th align="center">
<img width="394" height="1px">
<p> 
<small>
Reference
</small>
</p>
</th>
<th align="center">
<img width="294" height="1">
<p> 
<small>
Configuration
</small>
</p>
</th>
<th align="center">
<img width="194" height="1">
<p> 
<small>
Screenshot
</small>
</p>
</th>
</tr>
<tr>
<td>
<div align="center"><img src="https://i.ibb.co/12s2JfF/Captura-de-Pantalla-2021-09-23-a-la-s-19-16-53.png" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: table session</li>
<li><b>Date Range Dimension:</b>: createDate(date)</li>
<li><b>Dimension</b>: createDate(Month Day)</li>
<li><b>Metric</b>: sessionCode (Conversations per day)</li>
<li><b>Aggregation</b>: Count Distinct</li>
<li><b>Type</b>: Number</li>
<li><b>Comparison calculation</b>: None</li>
<li><b>Running calculation</b>: None</li>
<li>sessionCode (Accumulated Conversations)</li>
<li><b>Aggregation</b>: Count Distinct</li>
<li><b>Comparison calculation</b>: None</li>
<li><b>Running calculation</b>: None</li>
<li><b>Sort</b>: createDate - Ascending</li>
<li><b>Default date range</b>: Auto</li>
<li><b>Filter</b>: Create filter with the following parameters.</li>
<li>Include</li>
<li>botId</li>
<li>Equal to (=)</li>
<li><b>value</b>: botId</li>
<li><b>Interactions</b>:</li>
<li>check Apply Filter</li>
<li>check Enable sorting</li>
</ul>
</td>
<td>
<div align="center"><img src="https://i.ibb.co/hcdXy5G/Captura-de-Pantalla-2021-09-23-a-la-s-19-29-53.png" style="text-center"/></div>
</td>
</tr>
</table>

### **B. Average conversations per period**

<table>
<tr>
<th align="center">
<img width="394" height="1px">
<p> 
<small>
Reference
</small>
</p>
</th>
<th align="center">
<img width="294" height="1">
<p> 
<small>
Configuration
</small>
</p>
</th>
<th align="center">
<img width="194" height="1">
<p> 
<small>
Screenshot
</small>
</p>
</th>
</tr>
<tr>
<td>
<div align="center"><img src="https://i.ibb.co/LJ5vgks/Captura-de-Pantalla-2021-09-23-a-la-s-20-10-58.png" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: table session</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Metric</b>: botId</li>
<li><b>Default date range</b>: Auto</li>
<li><b>Filter</b>: Create filter with the following parameters.</li>
<li>Include</li>
<li>botId</li>
<li>Equal to (=)</li>
<li><b>value</b>: botId</li>
</ul>
</td>
<td>
<div align="center"><img src="https://i.ibb.co/fqt4210/Captura-de-Pantalla-2021-09-23-a-la-s-20-22-55.png" style="text-center"/></div>
</td>
</tr>
</table>

### **C. Conversation ended in human transshipment**
### **D. Total conversations**
### **E. Total messages received**
### **F. Top Answers**
### **G. Total messages per users(api calls)**
### **H. Total messages per bot**
### **I. Not Handle by bot**

## 3. USERS

### **A. Total Users**


## 4. MESSAGES

### **A. Total per day**
### **B. Total per week**
### **C. Total per month**

## 5. SATISFACTION SURVEY

### **A. Insatisfecho**
### **B. Neutro**
### **C. Satisfecho**

## 5. QUESTIONS
