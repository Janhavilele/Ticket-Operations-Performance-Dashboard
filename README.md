# Ticket-Operations-Performance-Dashboard

**1. Title:** _Ticket Operations Performance Dashboard_

A one-page analytical PowerBI dashboard built to monitor operational efficiency by analyzing ticket volume, resolution trends, assignee performance, product/platform distribution, and overall ticket lifecycle.

**2. Purpose:**

- The Ticket Operations Performance Dashboard provides a unified view of issue-tracking performance by visualizing ticket counts, statuses, resolution times, and system-wise distribution.
- It enables engineering, operations, and support teams to evaluate workload, track bottlenecks, and improve turnaround time.

**3. Tech Stack:**

This project was developed using the following tools and technologies:

**Data Processing:**

- Python (Pandas, NumPy) : Data cleaning & preprocessing

- Google Colab : Exploratory data analysis

- Datetime processing : Duration calculation, timestamps, and resolution time conversion

**Dashboard Development:**

- Microsoft Power BI : For visual creation

- DAX / Calculated Fields : KPI measures

- Data Modeling : Connecting cleaned tables for reporting


**4. Data Source:**

- The project uses an issue-tracking dataset containing operational ticket logs.


**Data Cleaning Performed Using Python:**

- Removed duplicates based on Issue id

- Checked null values across all columns

- Dropped missing records in Reporter and Reporter Id

- Filled missing values in Ops Product Name and Ops Platform with "Unknown"

- Comments column kept as null (no transformation applied)

- Converted all date fields to datetime format

- Cleaned string columns (trimmed spaces, standardized formatting)

- Converted duration text → numeric using a custom function

- Created Resolution Time column (Resolved - Created)

- Mapped status to two final values: "Open" and "Resolved"

This cleaned data feeds directly into the dashboard.


**5. Features:**


_• Business Problem:_

Operations and engineering teams often struggle to quickly understand ticket volumes, open backlogs, and product/platform-specific issues.

Answering questions such as:

1. How many tickets are still open?

2. Which product or platform generates the most issues?

3. What is the average resolution time?

4. How is the workload distributed across assignees?

is difficult with raw logs.



_• Goal of the Dashboard:_

- To provide a clear, interactive, and actionable tool that:

- Tracks total, open, and resolved issues

- Shows resolution time behavior

- Identifies product/platform hotspots

- Highlights team performance & bottlenecks

- Monitors ticket lifecycle efficiency



_• Walkthrough of Key Visuals:_

**i) KPI Cards (Top Section)**

- Total Issues

- Resolved Issues

- Open Issues

- Average Resolution Time (Days)

- Max Resolution Time (Days)

These provide an at-a-glance understanding of the system performance.

**ii) Issue by Status (Bar Chart):**

Displays volume of open vs. resolved issues, helping teams identify backlog and closure rate.

**iii) Issue by Resolution Duration (Histogram / Column Chart):**

Shows how many tickets fall into various resolution time ranges, highlighting extreme delays or quick resolutions.

**iv) Issues by Product Name (Bar Chart):**

Identifies which Ops Product Names generate the highest ticket volume.

**v) Issues by Ops Platform (Bar Chart):**

Shows the distribution of tickets across different operational platforms for resource planning.



_• Business Impact & Insights:_

- Operational Efficiency: Understand overall ticket load and resolution status

- Bottleneck Detection: Identify products/platforms causing frequent issues

- Performance Management: Check if SLAs are being met

- Improvement Opportunities: Reduce long-duration tickets

- Resource Allocation: Reassign workloads based on assignee or platform trends


**6. Screenshot:**

![Dashboard Screenshot](https://github.com/Janhavilele/Ticket-Operations-Performance-Dashboard/blob/main/Dashboard.PNG)
