---
layout: post
title:  "One-Stop Azure Cert Guide for a GCP Professional: Microsoft Azure Certification DP-200: Implementing an Azure Data Solution"
author: anil

categories: [ Technology, Cloud, Azure, Certification, DP-200 ]
tags: [Certification, Lifelong Learning, Cloud, Cloud Certification, Azure Certification]
image: assets/images/posts/azure_certified.png
image-caption: "Image courtesy: Lambda Architecture using Azure"
image-caption-url: "https://azure.microsoft.com/en-us/blog/lambda-architecture-using-azure-cosmosdb-faster-performance-low-tco-low-devops/"
description: "As a Technical Architect at MediaAgility, I refined my approach to designing new customer solutions for large enterprises, and I got more…"
featured: true
hidden: true
rating: 5
---

As a Technical Architect at [MediaAgility](https://www.mediaagility.com/), I refined my approach to designing new customer solutions for large enterprises, and I got more inclined to learning, not just studying and memorizing.

**Why I chose Azure Learning:**

In the last two years, I designed GCP solutions for almost five enterprises and the common fact was, every enterprise was using/(willing to use) a hybrid cloud strategy regardless of their industry & service. And the compelling reason was no-vendor locking & utilize the best services across cloud providers and stay in the front line of their competition.

I am extensively working on GCP but at the same time taking care of Azure & AWS intersections. After completing [My 6X Google Cloud Certification Journey](https://medium.com/@khichar.anil/my-6x-google-cloud-certification-journey-dfca1abdaacc), I decided to start with Azure to gain more in-depth knowledge.

### DP-200 Journey:

**Brief:**

At the start of 2019, Microsoft released two Azure Data exams: [Implementing an Azure Data Solution](https://www.microsoft.com/en-us/learning/exam-DP-200.aspx) (DP-200) and [Designing an Azure Data Solution](https://www.microsoft.com/en-us/learning/exam-DP-201.aspx) (DP-201). If you pass _both_ of these exams, you become a Microsoft Certified [Azure Data Engineer Associate](https://www.microsoft.com/en-us/learning/azure-data-engineer.aspx).

{% include img_with_caption.html img_name="dp-200-cert.png"
img_caption="At the end of 2019 I started learning Azure and on January 4th, 2020, I got recognition as a <strong>Microsoft Certified: Azure Data Engineer Associate.!!</strong>" %}

### **Steps:**

1.  **Reverse engineering** [Google Cloud for Azure professionals](https://cloud.google.com/docs/compare/azure): This guide compares Google Cloud with Azure and highlights the similarities and differences between the two. In addition, the guide provides quick-reference mappings of Azure products, concepts, and terminology to the corresponding products, concepts, and terminology on Google Cloud.
2.  [**Gold**](https://docs.microsoft.com/en-us/learn/certifications/exams/dp-200?wt.mc_id=learningredirect_certs-web-wwl) **content at Microsoft learning path:** In my opinion, this is the best learning resource of all. The estimated total time for all of the following modules was around **30 hours**. However, I ended up around **100 hours** to cover hands-on experiments**.**

*   [Azure](https://docs.microsoft.com/learn/paths/azure-for-the-data-engineer/) for the Data Engineer
*   [Store](https://docs.microsoft.com/learn/paths/store-data-in-azure/) data in Azure
*   [Work](https://docs.microsoft.com/learn/paths/work-with-relational-data-in-azure/) with relational data in Azure
*   [Work](https://docs.microsoft.com/learn/paths/work-with-nosql-data-in-azure-cosmos-db/) with NoSQL data in Azure Cosmos DB
*   [Large](https://docs.microsoft.com/learn/paths/data-processing-with-azure-adls/) Scale Data Processing with Azure Data Lake Storage Gen2
*   [Implement](https://docs.microsoft.com/learn/paths/implement-data-streaming-with-asa/) a Data Streaming Solution with Azure Streaming Analytics
*   [Implement](https://docs.microsoft.com/learn/paths/implement-sql-data-warehouse/) a Data Warehouse with Azure Synapse Analytics
*   [Perform](https://docs.microsoft.com/learn/paths/data-engineering-with-databricks/) data engineering with Azure Databricks
*   [Extract](https://docs.microsoft.com/learn/paths/data-science/) knowledge and insights from your data with Azure Databricks

{% include img_with_caption.html img_name="dp-200-cert-bookmark.png"
img_caption="My personalized bookmark list, out of this long learning path :)" %}

3\. **Notes**: I took some useful notes in Evernote which I need to consolidate and share in a public Git Repo. If anyone is interested, then please write in the comments below or find me on [LinkedIn](https://www.linkedin.com/in/anilkhichar/).

4\. **Must-read content:** This was my revision list which can make you the winner if you were about to lose the nearline race. If you are well prepared and wants to cover last day content, here it is:

> 4.a. Implement Data Storage Solutions:

> _CosmosDB_

1.  Understand CosmosDB [use cases](https://docs.microsoft.com/en-us/azure/cosmos-db/use-cases).
2.  It’s really important to know the [decision criteria](https://docs.microsoft.com/en-us/learn/modules/choose-api-for-cosmos-db/3-analyze-the-decision-criteria) for CosmosDB APIs.
3.  Deep dive into Cosmos DB [partitioning](https://azure.microsoft.com/en-us/blog/azure-cosmos-db-partitioning-design-patterns-part-1/) and learn about query performance tuning like deciding the partitioning key, creating lookup collection, etc.
4.  Perceive the intended meaning of Cosmos DB [request units](https://docs.microsoft.com/en-us/azure/cosmos-db/request-units)(RUs) so that you can save the cost and estimate the amount of RU for a particular workload.
5.  Implement a [lambda architecture](https://docs.microsoft.com/en-us/azure/cosmos-db/lambda-architecture) on the Azure platform. Get a clear understanding of which service to use while following this approach like Apache Spark vs Apache Hadoop etc.
6.  Understand [HDFS architecture](https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html#NameNode+and+DataNodes) and get a clear understanding and use cases about Primary, Secondary, NameNode & DataNode.

> _Storage_

1.  Manage the Azure Blob [storage lifecycle](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-lifecycle-management-concepts?tabs=azure-portal). Experiment the mentioned example in this post about applying a lifecycle policy. **_hands-on_**
2.  Learn about [Access control](https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control) in Azure Data Lake Storage Gen2. Pay special attention to Azure AD setup while applying ACLs. **_hands-on_**
3.  Configure Azure [Storage firewalls](https://docs.microsoft.com/en-us/azure/storage/common/storage-network-security) and virtual networks. **_hands-on_**

> _Azure SQL Server & SQL Server Data Warehouse (Synapse Analytics)_

1.  [Which SQL](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-paas-vs-sql-server-iaas) option should I choose?
2.  [Export](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-export) an Azure SQL database to a BACPAC file. **_hands-on_**
3.  Learn about how to secure sensitive data in a SQL database with database encryption by using the [Always Encrypted](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-always-encrypted) wizard. **_hands-on_**
4.  Experience Azure SQL Database [Advanced Threat Protection](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-threat-detection) features & steps to enable it. **_hands-on_**
5.  Experiment and enable [TDE](https://docs.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql?view=sql-server-ver15) (Transparent Data Encryption) and keep a note on the steps: _Formula(memory trick)_: MCED — Master Key, Certificate, Encryption & Apply encryption on the DB. **_hands-on_**
6.  Do an experiment using [Powershell](https://docs.microsoft.com/en-us/azure/sql-database/scripts/sql-database-create-and-configure-database-powershell) & Azure [cloud shell](https://docs.microsoft.com/en-us/azure/cosmos-db/scripts/cli/sql/create). **_hands-on_**
7.  [IP firewall](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-firewall-configure) rules. **_hands-on_**
8.  Read about [dynamic data masking](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-dynamic-data-masking-get-started) for Azure SQL Database and Azure Synapse Analytics. Give special attention to the in-built masking functions & their appropriate usages (Default, Credit Card, Email, Random Number, Custom Text)
9.  **_Polybase_**: Please execute this [hands-on experiment](https://docs.microsoft.com/en-us/azure/sql-data-warehouse/sql-data-warehouse-load-from-azure-data-lake-store) multiple times to load the data from ADLS into WH and memorize all the steps in the correct sequence. _Formula(Memory trick):_ MCSFTL — Master, Credential, Source, File, Table, Load(CTAS). [Load New York Taxicab dataset](https://github.com/MicrosoftDocs/azure-docs/blob/master/articles/sql-data-warehouse/load-data-from-azure-blob-storage-using-polybase.md) **_hands-on_**
10.  DW performance [benchmarking](https://docs.microsoft.com/en-us/archive/blogs/apsblog/azure-sql-dw-performance-ctaspartition-switching-vs-updatedelete): This example demonstrates DW performance benchmarking and concluded to utilize a methodology of CTAS and partition switching in lieu of UPDATE and DELETE operations wherever possible. Get a full understanding of this fundamental approach. **_hands-on_**

> 4.b. Manage and develop data processing:

> _Azure Data Factory_

1.  Understand the difference between all the available [Integration runtime](https://docs.microsoft.com/en-us/azure/data-factory/concepts-integration-runtime). Pay special attention to the self-hosted integration runtime.
2.  Azure Data Factory Copy Activity: Find out [schema mapping](https://docs.microsoft.com/en-us/azure/data-factory/copy-activity-schema-and-type-mapping) ways between source & sink. **_hands-on_**

> _Storage & HDInsight_

1.  Get in-depth knowledge of using Azure Data Lake Storage Gen2 for big data requirements. Also, learn about different [Hadoop tools](https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-data-scenarios) discussed in this article.
2.  Choose the correct [HDInsight Configuration](https://docs.microsoft.com/en-us/learn/modules/hdinsight-config-open-source-solution/index) to build open-source analytics solutions. Give special attention to the use cases and get a better understanding of when to use Storm vs Spark etc.

> _Azure Databricks_

1.  Learn about the technology [choices for batch processing](https://docs.microsoft.com/en-us/azure/architecture/data-guide/technology-choices/batch-processing) and what is the decision criteria to choose one over the others.
2.  ETL using Azure [Databricks](https://docs.microsoft.com/en-us/azure/azure-databricks/databricks-extract-load-sql-data-warehouse#load-data-into-azure-sql-data-warehouse). Special attention to “Load data into Azure SQL Data Warehouse” **_hands-on_**
3.  Experiment on different [cluster configurations](https://docs.microsoft.com/en-us/azure/databricks/clusters/configure). **_hands-on_**

> _Azure Stream Analytics_

1.  [Window functions](https://docs.microsoft.com/en-us/azure/stream-analytics/stream-analytics-window-functions): You must know the practical difference between all the stream analytics windowing functions & their usage (Tumbling, Hopping, Sliding & Session windows). **_hands-on_**
2.  Learn how to use [lookup data](https://docs.microsoft.com/en-us/azure/stream-analytics/stream-analytics-use-reference-data) in the Azure Stream Analytics in a data streaming pipeline. **_hands-on_**
3.  Azure Stream Analytics on [IoT Edge](https://docs.microsoft.com/en-us/azure/stream-analytics/stream-analytics-edge)

> 4.c. Monitor and optimize data solutions:

1.  Understand the [SQL auditing](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-auditing) features & do a hand-on experiment on who/when & what got accessed from the Azure SQL DB & WH? **_hands-on_**
2.  Learn about enabling SQL server [automatic tuning](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-automatic-tuning-enable) & give special attention towards the inheritance with tuning options like _Force Plan, Create Index & Drop Index._ **_hands-on_**
3.  Read & understand [In-Memory](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-in-memory) technologies that improve performance without increasing the database service tier. **_hands-on_**
4.  Understand the [materialized view](https://docs.microsoft.com/en-us/azure/architecture/patterns/materialized-view) design pattern and think about its uses to boost a slow-performing SQL query. **_hands-on_**
5.  Learn how to enable and configure l[ogging of diagnostics](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-metrics-diag-logging) telemetry for Azure SQL databases. Pay special attention to the metric storage options like Azure SQL Analytics, Azure Event Hubs & Azure Storage. **_hands-on_**
6.  Imbibe [ADLS Gen2 performance optimization](https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-performance-tuning-guidance) techniques. Understand file sizing & data organization into folders.
7.  Discover [Azure data factory monitoring](https://docs.microsoft.com/en-us/azure/data-factory/monitor-using-azure-monitor) using Azure monitor and think about use cases like last quarter log analytics and find out different actionable trends. **_hands-on_**
8.  Learn about [on-premises HA data gateway](https://docs.microsoft.com/en-us/data-integration/gateway/service-gateway-high-availability-clusters) cluster to avoid single points of failure and to load balance traffic across gateways in a cluster.
9.  Understand the use of Azure Log Analytics to [monitor HDInsight](https://docs.microsoft.com/en-us/azure/hdinsight/hdinsight-hadoop-oms-log-analytics-tutorial) clusters. Pay special attention to “Install HDInsight cluster management solutions”. **_hands-on_**

...

Core mantra has to be: **Never target for certification, rather understand the platform & technology**, because this will help us to design better solutions for our customers and perform our work in a qualitative manner. These are the perks of being a lifelong learner.

In this post, I shared all the resources that I found and used. **Always check the latest official information from Microsoft before your exam.**

Prepare well and all the best for the exam!
