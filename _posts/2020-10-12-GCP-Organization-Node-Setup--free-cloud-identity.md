---
layout: post
title: "GCP Organization Node Setup (free cloud identity)"
author: anil

categories: [ Technology, Cloud, GCP, Foundation, OrgNode ]
tags: [Lifelong Learning, Cloud, GCP, Organization Setup, Foundation, Cloud Identity]
image: assets/images/posts/gcp-org-node-setup.png
image-caption: "GCP Org Structure"
description: ""
featured: false
hidden: false
rating: 5
---

### **Problem Statement:**
> An organization node is available for **G Suite** and **Cloud Identity** customers. There is a lot of content about GCP org node but still, it’s not clear if a customer can start leveraging Org Node advantage without being a GSuite customer.

It’s [mentioned](https://cloud.google.com/resource-manager/docs/creating-managing-organization):

_You can use a_ [_free_](https://support.google.com/cloudidentity/answer/7319251?visit_id=636934455105255816-106820737&rd=1) _Cloud Identity account to create an Organization resource._ **_Cloud Identity Free edition_** _includes core identity and endpoint management services. It provides free, managed Google Accounts to users who don’t need G Suite Services, such as Gmail or Google Drive. You can use Cloud Identity accounts with other Google services, such as Google Cloud Platform (GCP), Chrome, Android enterprise, and a large catalog of third-party applications. Upgrade your feature set by signing up for the Cloud Identity Premium edition._

Cloud Identity is Free as well as Paid. GCP customers who don’t want to move to GSuite but want to use Google authentication/identity for GCP login can subscribe to Cloud Identity for free.

> **But there is no free edition of** [**cloud identity**](https://cloud.google.com/identity/)**. Am I missing something?**

**The ideal** structure of an organization: Everyone wants to utilize this structure but sometimes customers feel shy to go with the GSuite route.  
References: [cloud-platform-resource-hierarchy](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy), [best-practices-for-enterprise-organizations](https://cloud.google.com/docs/enterprise/best-practices-for-enterprise-organizations)

![Example Google Cloud resource hierarchy](https://cdn-images-1.medium.com/max/800/0*PAz0Q7GEh4Pi-40_.png)

> Solution:

Free cloud identity details:

[**Option A (If you already have a GCP project and want to connect this project with an org node):**](https://support.google.com/cloudidentity/answer/7389973)
{% include img_with_caption.html img_name="gcp-signup-for-cloud-identity.png"
img_caption="" %}

**Option B (Setup Org node and then start migrating/connecting existing GCP projects):**

<iframe width="560" height="315" src="https://www.youtube.com/embed/TlDW1up98Uc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Steps:**

1.  Free Cloud Identity Setup: [https://gsuite.google.com/signup/gcpidentity](https://gsuite.google.com/signup/gcpidentity)
2.  Verify domain ownership: [https://support.google.com/cloudidentity/answer/7331243?hl=en](https://support.google.com/cloudidentity/answer/7331243?hl=en)
3.  Continue with GCP Console
4.  GCP free account setup/Billing setup
5.  Folder management
6.  Organization Policy Overview

I hope this post will help in setting up a strong foundation pillar on GCP.