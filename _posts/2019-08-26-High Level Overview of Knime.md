---
title: "High Level Overview of Knime"
date: 2019-08-26
tags: [data science, production, data engineer  ]
header:
  image: "/images/KnimeOverview/cover.jpg"

  excerpt: "Data Science,Analytics, Platform"

---

# Overview of analytics projects in manufacturing environments
For any advanced data projects, there are 4 main steps to address 4 questions:

1. Extract & collect data: How do we extract, collect, and connect various data sources?
2. Modeling & analyze: What algorithms do we use to create value from data?
3. Display & inform: How do we present the data output to allow our company to make decisions?
4. Automate & industrialize: How do we further eliminate waste through digital automation?

# Problems with traditional tools
During my internship at Continental Automotive, which is one of the biggest automotive suppliers in the world, I get to work with database systems in manufacturing, including MES and SAP. These are considered as being more structured. Other custom data comes in form of log file and IoT data, which is messier. Those data are then connected to business intelligence platforms, including Power BI, Tableau, MicroStrategy.

However, one of the weaknesses of BI platforms, in general, is data manipulation, so we need to rely heavily that data coming into BI platforms is already cleaned and prepared in structured tables, which is not the case often times. Also, licensing cost is another issue, as the bigger server and more usability for bigger data set would cost more, so it is not very affordable to scaling. Besides, BI platforms do not have much power in term of big data analytics. In general, as data grows, it becomes more problematic right at step 1 mentioned above.

# The need for KNIME as a data analytics and integration platform
To solve this problem, instead of directly connecting BI platforms with databases, we can use KNIME as an intermediate step for data wrangling before feeding it into BI. One advantage of KNIME is that it allows flexibility for different users, from non-programmers to more advanced data mining professionals using Python and R. This is a very important factor to consider, as most intended users are not programmers. KNIME has drag-and-drop interface, which makes it extremely easy to learn. Data can be then dumped into manufacturing datalake, and therefore can be accessed widely across the company. Even more impressive, KNIME supports various advanced components for machine learning, allowing even more powerful analytics usage to give more business insights. Another point worth mentioning is that KNIME is technically free and open source, so it is ideal for those who are on budget and those who want to customize accordingly to their needs.

# Outcome
A KNIME pipeline is set up to automatically pull all data needed, apply transformation, and create visualizations, which is a great help for engineers in their daily work. Before, this was done manually in Excel, which took a lot of time. Now, engineers can focus more on their actual work, increasing work efficiency. On top of that, a predictive model is built at the end of the pipeline, creating valuable insights to react faster to production.
