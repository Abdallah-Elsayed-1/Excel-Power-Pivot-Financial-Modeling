<div align="center">

  <h1>📊 Excel Power Pivot Enterprise Sales & Financial Modeling</h1>
  <p><b>An Advanced Excel Financial Analytics Solution utilizing Power Query, Power Pivot Data Modeling (Star Schema), DAX Measures, and YoY Growth Tracking.</b></p>

  <!-- Clean Tech Stack Badge Bar -->
  <p align="center">
    <code>🟢 Microsoft Excel</code> &bull; 
    <code>⚡ Power Pivot</code> &bull; 
    <code>🔵 Power Query ETL</code> &bull; 
    <code>🧠 Advanced DAX</code> &bull; 
    <code>📈 YoY Analytics</code>
  </p>

</div>

<hr />
<br />

<h2>📌 Project Overview</h2>
<p>
  This project demonstrates advanced <b>Financial & Sales Modeling inside Microsoft Excel</b> by stepping beyond traditional spreadsheets. Leveraging <b>Power Query</b> for data extraction, <b>Power Pivot</b> for relational data modeling, and <b>DAX (Data Analysis Expressions)</b> for dynamic measures, this solution transforms raw sales data into an interactive executive dashboard with Year-over-Year (YoY) performance metrics.
</p>

<br />

<h2>📊 Executive Dashboard Preview</h2>
<p>Interactive Excel dashboard powered by dynamic Pivot Charts, Slicers, and Timelines:</p>

<div align="center">
  <img src="https://i.postimg.cc/mZjpmHtZ/dashbwrd.png" alt="Excel Power Pivot Dashboard" width="100%" />
</div>

<br />
<hr />
<br />

<h2>🔑 Financial Key Performance Indicators (KPIs)</h2>
<ul>
  <li><b>Total Sales Revenue:</b> Consolidated top-line sales calculated across all product lines.</li>
  <li><b>Total Net Profit & Profit Margin %:</b> Margin percentage calculations per region and category.</li>
  <li><b>Year-over-Year (YoY) Growth %:</b> Time intelligence measuring annual growth trajectory.</li>
  <li><b>Customer Segment Performance:</b> Breakdown across Consumer, Corporate, and Home Office segments.</li>
</ul>

<br />
<hr />
<br />

<h2>🛠️ Technical Architecture & Pipeline</h2>

<h3>Stage 1: Power Pivot Data Modeling (Star Schema)</h3>
<p>
  Instead of fragile <code>VLOOKUP</code> / <code>XLOOKUP</code> formulas, a relational <b>Star Schema</b> was built inside the Excel Data Model (Power Pivot). The central fact table (<code>Fact_Sales</code>) is connected to dimension tables (<code>Dim_Customer</code>, <code>Dim_Product</code>, <code>Dim_Date</code>, <code>Dim_Region</code>) via strict 1-to-Many relationships.
</p>

<div align="center">
  <table border="0" width="100%">
    <tr>
      <td width="50%" align="center" valign="top">
        <h4>Relational Data Model (Power Pivot Diagram)</h4>
        <img src="https://i.postimg.cc/Df6pxX8y/mwdylynj.png" width="95%" alt="Power Pivot Star Schema Model" />
      </td>
      <td width="50%" align="center" valign="top">
        <h4>DAX Measures & Calculation Area</h4>
        <img src="https://i.postimg.cc/MZ539QvS/mesures.png" width="95%" alt="Power Pivot Calculation Area" />
      </td>
    </tr>
  </table>
</div>

<br />

<h3>Stage 2: DAX Measures Formulation</h3>
<p>Engineered explicit DAX measures directly inside Excel's Data Model:</p>
<ul>
  <li><code>Total Sales</code> = <code>SUM(Fact_Sales[Sales])</code></li>
  <li><code>Total Profit</code> = <code>SUM(Fact_Sales[Profit])</code></li>
  <li><code>Profit Margin %</code> = <code>DIVIDE([Total Profit], [Total Sales], 0)</code></li>
  <li><code>YoY Growth %</code> = Dynamic DAX evaluation comparing current year sales against previous periods.</li>
</ul>

<br />
<hr />
<br />

<h2>🎯 Financial Slicing & Segment Analysis</h2>

<h3>1. Year-over-Year (YoY) Growth Trends</h3>
<p>Dedicated YoY performance view evaluating revenue scaling and percentage growth over time:</p>

<div align="center">
  <img src="https://i.postimg.cc/59gKsC6b/yoy.png" alt="YoY Growth Analysis" width="85%" />
</div>

<br />

<h3>2. Customer Segment & Category Cross-Filtering</h3>
<p>Dynamic slicing capabilities analyzing targeted customer bases and regional category distributions:</p>

<div align="center">
  <table border="0" width="100%">
    <tr>
      <td width="50%" align="center" valign="top">
        <h4>Home Office Segment Analysis</h4>
        <img src="https://i.postimg.cc/HsLZRkyD/hwm-awfys.png" width="95%" alt="Home Office Segment Slicer" />
        <p align="left"><small>Isolates sales performance and margins for the Home Office customer segment.</small></p>
      </td>
      <td width="50%" align="center" valign="top">
        <h4>Category & Regional Breakdown</h4>
        <img src="https://i.postimg.cc/44P2W9mx/katyjwry.png" width="95%" alt="Category Slicer" />
        <p align="left"><small>Slices profitability across specific product categories and geographical regions.</small></p>
      </td>
    </tr>
  </table>
</div>

<br />
<hr />
<br />

<h2>💡 Strategic Insights</h2>
<ol>
  <li><b>Data Model Efficiency:</b> Building a Star Schema inside Excel reduced workbook file size and accelerated Pivot Table refresh rates compared to traditional cell-based formulas.</li>
  <li><b>Targeting High-Margin Segments:</b> Home Office customers show a strong average order value, making them prime targets for cross-selling bundled office accessories.</li>
  <li><b>YoY Revenue Momentum:</b> YoY comparison confirms steady expansion, recommending inventory scale-ups prior to peak seasonal periods.</li>
</ol>

<br />
<hr />
<br />

<h2>📂 Repository Architecture</h2>
<pre>
├── Data/                        # Raw Sales Workbooks & Source Data
├── Workbooks/                   # Excel_Power_Pivot_Financial_Model.xlsx
├── Screenshots/                 # Model & Dashboard visual assets
└── README.md                    # Project documentation
</pre>
