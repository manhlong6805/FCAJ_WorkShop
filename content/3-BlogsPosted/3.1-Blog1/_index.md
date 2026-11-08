---
title: "Blog 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---


# BUILDING SECURE MULTI-USER AI SYSTEMS WITH AMAZON BEDROCK

An AWS blog post highlights how PAR Technology developed a multi-tenant AI system using Amazon Bedrock to enable natural language data analysis. A key challenge was allowing multiple users to share the same AI system while ensuring robust security and precise access control. To address this, PAR Technology implemented a three-layered security architecture designed to prevent unauthorized access and mitigate the risk of data leakage between organizations.

**Key points to know:**

* Multi-tenant AI allows multiple organizations to share a single AI system, while ensuring that each organization’s data remains independently protected.
* Amazon Bedrock provides AI models capable of interpreting natural language questions and generating SQL queries for data analysis.
* AWS Signature Version 4 (SigV4) authenticates identities and ensures the integrity of access requests.
* Semantic Validation examines the content of a question to verify that the request is valid before any data is retrieved.
* Row-Level Security restricts access to individual data rows based on user roles and identities.
* Split-Plane SQL decouples the process of enforcing data access permissions from the AI-driven query generation process, preventing the model from accessing data outside its authorized scope.
* The system employs a multi-layered security architecture to mitigate the risk of data leakage, even in the event that the AI ​​model generates an incorrect query.

This solution is particularly useful for businesses that provide AI applications to multiple clients, where access control and data protection are critical requirements. It demonstrates how Amazon Bedrock can be integrated with AWS security mechanisms to build AI systems that are flexible, secure, and scalable.

**Hierarchical structure**
![Hierarchical structure](/FCAJ_WorkShop/images/structured.png)

**Multi-user AI architecture**
![Multi-user AI architecture](/FCAJ_WorkShop/images/blog1.png)

**Link to original article**https://aws.amazon.com/vi/blogs/machine-learning/multi-tenant-llm-analytics-with-row-level-security-how-we-built-a-secure-agent-on-aws/
