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
<div align="center"><img src="https://i.ibb.co/0sL1yM5/Captura-de-Pantalla-2021-09-23-a-la-s-20-32-32.png" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select * from user_interaction where answerId in (select id from answer where name = value01 and botId=value02)</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Metric</b>: Record count</li>
<li><b>Aggregation</b>: auto</li>
<li><b>Type</b>: Number</li>
<li><b>Comparison calculation</b>: None</li>
<li><b>Running calculation</b>: None</li>
<li><b>Default date range</b>: Auto</li>
</ul>
</td>
<td>
<div align="center"><img src="https://i.ibb.co/kK4xkZp/Captura-de-Pantalla-2021-09-23-a-la-s-20-33-12.png" style="text-center"/></div>
</td>
</tr>
</table>

### **D. Total conversations**

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
<div align="center"><img src="#" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: table session</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Metric</b>: botId</li>
<li><b>Aggregation</b>: Count</li>
<li><b>Type</b>: Number</li>
<li><b>Comparison calculation</b>: None</li>
<li><b>Running calculation</b>: None</li>
<li><b>Default date range</b>: Auto</li>
<li><b>Filter</b>: Create filter with the following parameters.</li>
<li>Include</li>
<li>botId</li>
<li>Equal to (=)</li>
<li><b>value</b>: botId</li>    
</ul>
</td>
<td>
<div align="center"><img src="#" style="text-center"/></div>
</td>
</tr>
</table>

### **E. Total messages received**

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
<div align="center"><img src="" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select usrint.id,sess.botId,sess.channelId,usrint.createDate,usrint.text,usrint.confidence from alvoradadb.user_interaction usrint, alvoradadb.session sess where usrint.sessionCode = sess.sessionCode and sess.botId=value01</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Metric</b>: id</li>
<li><b>Aggregation</b>: Count</li>
<li><b>Type</b>: Number</li>
<li><b>Comparison calculation</b>: None</li>
<li><b>Running calculation</b>: None</li>
<li><b>Default date range</b>: Auto</li>
</ul>
</td>
<td>
<div align="center"><img src="" style="text-center"/></div>
</td>
</tr>
</table>

### **F. Top Answers**

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
<div align="center"><img src="" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select an.name,an.description,ui.sessionCode,ui.createDate from alvoradadb.user_interaction ui, alvoradadb.answer an where ui.answerID = an.id and ui.answerId in ('values')</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Dimension</b>: </li>
<li>description</li>
<li>name</li>
<li><b>Metric</b>:</li>
<li>name</li>
<li><b>Aggregation</b>: Count</li>
<li><b>Type</b>: Number</li>
<li><b>Comparison calculation</b>: None</li>
<li><b>Running calculation</b>: None</li>
<li><b>description</b>:</li>
<li><b>Aggregation</b>: Count</li>
<li><b>Type</b>: Percent</li>
<li><b>Comparison calculation</b>: Percent of total - Relative to corresponding data</li>
<li><b>Running calculation</b>: None</li>
<li><b>Sort</b>: description</li>
<li><b>Aggregation</b>: Count</li>
</ul>
</td>
<td>
<div align="center"><img src="" style="text-center"/></div>
</td>
</tr>
</table>

### **G. Total messages per users(api calls)**

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
<div align="center"><img src="" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: SELECT usrint.id, sess.botId, sess.channelId, usrint.createDate, usrint.text, usrint.confidence FROM alvoradadb.user_interaction usrint, alvoradadb.session sess where usrint.sessionCode = sess.sessionCode and usrint.userSent=1 and sess.botId=value</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Metric</b>: id</li>
<li><b>Aggregation</b>: Count</li>
<li><b>Type</b>: Number</li>
<li><b>Comparison calculation</b>: None</li>
<li><b>Running calculation</b>: None   </li> 
</ul>
</td>
<td>
<div align="center"><img src="" style="text-center"/></div>
</td>
</tr>
</table>

### **H. Total messages per bot**

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
<div align="center"><img src="" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select ui.* from user_interaction as ui inner join session as s on ui.sessionCode = s.sessionCode where ui.id in (select ui.userSentIdfrom user_interaction as ui inner join session as s on ui.sessionCode = s.sessionCode where ui.answerId in(values) and s.botId = value01) order by ui.createDate desc</li> 
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Dimension: </b></li>
<li>createDate</li>
<li><b>Type</b>: Date Hour Minute</li>
<li><b>text</b>:</li>
<li><b>Type</b>: Text</li>
<li><b>Sort</b>: createDate(date)</li>
</ul>
</td>
<td>
<div align="center"><img src="" style="text-center"/></div>
</td>
</tr>
</table>

### **I. Not Handle by bot**

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
<div align="center"><img src="" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select ui.* from user_interaction as ui inner join session as s on ui.sessionCode = s.sessionCode where ui.id in (select ui.userSentIdfrom user_interaction as ui inner join session as s on ui.sessionCode = s.sessionCode where ui.answerId in(values) and s.botId = value01) order by ui.createDate desc</li> 
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Dimension: </b></li>
<li>createDate</li>
<li><b>Type</b>: Date Hour Minute</li>
<li><b>text</b>:</li>
<li><b>Type</b>: Text</li>
<li><b>Sort</b>: createDate(date)</li>
</ul>
</td>
<td>
<div align="center"><img src="" style="text-center"/></div>
</td>
</tr>
</table>

## 3. USERS

### **A. Total Users**

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
<div align="center"><img src="" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: table sessions</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Dimension</b>: createDate (Month Day)</li>
<li><b>Metric</b>: userRef</li>
<li><b>Aggregation</b>: Count</li>
<li><b>Type</b>: Number</li>
<li><b>Comparison calculation</b>: None</li>
<li><b>Running calculation</b>: None</li>
<li><b>Filter</b>: Create filter with the following parameters.</li>
<li>Include</li>
<li>botId</li>
<li>Equal to (=)</li>
<li>value: botId</li>
</ul>
</td>
<td>
<div align="center"><img src="" style="text-center"/></div>
</td>
</tr>
</table>


## 4. MESSAGES

### **A. Total per day**

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
<div align="center"><img src="" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select b.id, b.name, u.createdate fecha, day(u.createdate) dia, count(*) mensajesEnviados from user_interaction u ,session s , bot b where u.sessionCode = s.sessionCode and b.id = s.botId and u.userSent=1 and b.id =value group by b.id, dia order by b.name, fecha, dia</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Dimension</b>: createDate</li>
<li><b>Metric:</b></li>
<li>mensajesEnviados</li>
<li>Agreggation: Sum</li>
<li>Type: Number</li>
<li>Comparison calculation: None</li>
<li>Running calculation: None</li>
<li><b>Sort</b>: createDate</li>
</ul>
</td>
<td>
<div align="center"><img src="" style="text-center"/></div>
</td>
</tr>
</table>

### **B. Total per week**

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
<div align="center"><img src="#" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select b.id, b.name, u.createdate fecha, week(u.createdate) semana, count(*) mensajesEnviados from user_interaction u ,session s , bot b where u.sessionCode = s.sessionCode and b.id = s.botId and u.userSent=1 and b.id =value group by b.id, semana order by b.name, fecha, semana</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Dimension</b>: createDate</li>
<li><b>Metric:</b></li>
<li>mensajesEnviados</li>
<li>Agreggation: Sum</li>
<li>Type: Number</li>
<li>Comparison calculation: None</li>
<li>Running calculation: None</li>
<li><b>Sort</b>: createDate</li>
</ul>
</td>
<td>
<div align="center"><img src="#" style="text-center"/></div>
</td>
</tr>
</table>

### **C. Total per month**

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
<div align="center"><img src="#" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select b.id, b.name, u.createdate fecha, month(u.createdate) mes, count(*) mensajesEnviados from user_interaction u ,session s , bot b where u.sessionCode = s.sessionCode and b.id = s.botId and u.userSent=1 and b.id =value group by b.id, mes order by b.name, fecha, mes</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Dimension</b>: createDate</li>
<li><b>Metric:</b></li>
<li>mensajesEnviados</li>
<li>Agreggation: Sum</li>
<li>Type: Number</li>
<li>Comparison calculation: None</li>
<li>Running calculation: None</li>
<li><b>Sort</b>: createDate</li>
</ul>
</td>
<td>
<div align="center"><img src="#" style="text-center"/></div>
</td>
</tr>
</table>

## 5. SATISFACTION SURVEY

### **A. Insatisfecho**

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
<div align="center"><img src="#" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: SELECT stf.sessionCode session,stf.evaluation evaluation,stf.userComments comments,stf.createDate createDate,sess.userRef IP,sess.locale locale FROM alvoradadb.satisfaction stf, alvoradadb.session sess where stf.sessionCode=sess.sessionCode and sess.botId=value01 and sess.channelID=value02</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Metric</b>: Record count</li>
<li><b>Filter</b>: evaluation equal 01</li>
</ul>
</td>
<td>
<div align="center"><img src="#" style="text-center"/></div>
</td>
</tr>
</table>

### **B. Neutro**

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
<div align="center"><img src="#" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: SELECT stf.sessionCode session,stf.evaluation evaluation,stf.userComments comments,stf.createDate createDate,sess.userRef IP,sess.locale locale FROM alvoradadb.satisfaction stf, alvoradadb.session sess where stf.sessionCode=sess.sessionCode and sess.botId=value01 and sess.channelID=value02</li>
<li><b>Date Range Dimension</b>: createDate(date)</li>
<li><b>Metric</b>: Record count</li>
<li><b>Filter</b>: evaluation equal 02</li>
</ul>
</td>
<td>
<div align="center"><img src="#" style="text-center"/></div>
</td>
</tr>
</table>

### **C. Satisfecho**

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
<div align="center"><img src="#" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: SELECT stf.sessionCode session,stf.evaluation evaluation,stf.userComments comments,stf.createDate createDate,sess.userRef IP,sess.locale locale FROM alvoradadb.satisfaction stf, alvoradadb.session sess where stf.sessionCode=sess.sessionCode and sess.botId=value01 and sess.channelID=value02</li>
<li><b>Metric</b>: Record count</li>
<li><b>Filter</b>: evaluation equal 03</li>
</ul>
</td>
<td>
<div align="center"><img src="#" style="text-center"/></div>
</td>
</tr>
</table>

## 5. QUESTIONS

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
<div align="center"><img src="https://i.ibb.co/hXHLrWC/Captura-de-Pantalla-2021-09-27-a-la-s-15-43-13.png" style="text-center"/></div>
</td>
<td>
<ul>
<li><b>Datasource</b>: select count(*) cantidad, '75% - 100%' tag, createDate from (select text,createDate, avg(confidence) asertiveness from (select text, confidence,u.createDate from user_interaction u ,session s , bot b where u.sessionCode = s.sessionCode and b.id = s.botId and b.id=value and confidence is not null and text is not null) asd group by text order by text desc ) C1 where asertiveness <= 1 and asertiveness > 0.75 union all select count(*) cantidad, '50% - 75%' tag, createDate from (select text,createDate, avg(confidence) asertiveness from (select text, confidence,u.createDate from user_interaction u ,session s , bot b where u.sessionCode = s.sessionCode and b.id = s.botId and b.id=value and confidence is not null and text is not null) asd group by text order by text desc ) C2 where asertiveness <= 0.75 and asertiveness > 0.5 union all
select count(*) cantidad, '25% - 50%' tag, createDate from (select text,createDate, avg(confidence) asertiveness from (select text, confidence,u.createDate from user_interaction u ,session s , bot b where u.sessionCode = s.sessionCode and b.id = s.botId and b.id=value and confidence is not null and text is not null) asd group by text order by text desc) C3 where asertiveness <= 0.5 and asertiveness > 0.25 union all select count(*) cantidad, ' 0% - 25%' tag, createDate from (select text,createDate, avg(confidence) asertiveness from (select text, confidence,u.createDate from user_interaction u ,session s , bot b
where u.sessionCode = s.sessionCode and b.id = s.botId and b.id=value and confidence is not null and text is not null) asd group by text order by text desc
) C4 where asertiveness < = 0.25 and asertiveness > 0
</li>
<li><b>Dimension</b>: TAG</li>
<li><b>Type</b>: Number</li>
<li><b>Metric</b>: cantidad</li>
<li><b>Aggregation</b>: Sum</li>
<li><b>Sort</b>: cantidad</li>  
<li><b>Aggregation</b>: Sum</li>
</ul>
</td>
<td>
<div align="center"><img src="https://i.ibb.co/Fw38qvt/Captura-de-Pantalla-2021-09-27-a-la-s-15-44-09.png" style="text-center"/></div>
</td>
</tr>
</table>
