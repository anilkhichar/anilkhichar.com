---
layout: post
title:  "Now Google BigQuery is truly enterprise-ready DW (DML without limits; Integer
  range partitioning)"
author: anil
categories: [ Technology, Cloud, GCP, BigQuery ]
tags: [Lifelong Learning, Cloud, GCP, BigQuery, New Feaure]
image: assets/images/now-bq-enterprise-dw_1.jpg
image-caption: Power of BigQuery
description: "I have been using BigQuery for a couple of years and designing/migrating
  enterprise data warehouses but the new announcement on limitless"
featured: false
hidden: false
---
I have been using BigQuery for a couple of years and designing/migrating enterprise data warehouses but the new announcement on [limitless DML](https://cloud.google.com/bigquery/docs/creating-integer-range-partitions) inspired me to write about its beauty.

I do have strong hands-on experience with on-prem traditional data warehouse & data warehousing across cloud providers (Redshift, SQL Data Warehouse a.k.a. Synapse). I always considered Google BigQuery as the next generation DW but following two nonexistence bothering me all the time:

1.  **Limited DML operations:** It’s limitless now since Feb 26, 2020 [announcement](https://cloud.google.com/blog/products/data-analytics/dml-without-limits-now-in-bigquery?utm_source=feedburner&utm_medium=email&utm_campaign=Feed:%2Bgoogleblog%2FCNkG%2B%28Google%2BCloud%2BPlatform%2BBlog%29).
2.  **Date only partition**: It used to support Date & Timestamp(it is an illusion, practically it’s also a date partition). Now BigQuery also supports tables [partitioned on an integer column](https://cloud.google.com/bigquery/docs/creating-integer-range-partitions) as well. I hope in the near future there will be more partitioning options like the oracle.

DML was always a struggle while migrating data from traditional enterprise data warehouses and especially dealing with the CDC(change data capture). In my recent Oracle EDW migration to BigQuery, managing update/delete on the new CDC was a big challenge.

Top 10 BigQuery features which I do consider it is the next generation EDW:

1.  Quick setup & the most cost-effective DW
2.  Fully managed and server-less
3.  Scales on-demand from gigabytes to petabytes
4.  Seamless access due to data replication so the data is always available
5.  Automatic snapshots and data backup reduces worries about unexpected data changes
6.  Encrypted, durable, and highly available
7.  Built-in machine learning for predictive analytics
8.  In-memory BI Engine for blazing-fast reporting

{% include img_with_caption.html img_name="now-bq-enterprise-dw_2.png"
img_caption="This is why it’s the leader in DW" %}

9\. This is how BigQuery removes the traditional data warehousing barriers:

{% include img_with_caption.html img_name="now-bq-enterprise-dw_3.png"
img_caption="This is why it’s the leader in DW" %}

10\. Real-time insights: Insert up to 100,000 rows of data per second and analyze business events as they unfold.

Read more about BigQuery [here](https://cloud.google.com/bigquery).

Happy coding & keep spreading happiness and kindness :)