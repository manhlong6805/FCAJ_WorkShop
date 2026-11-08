---
title: "Blog 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---


# BLOG 3: Using AI for Automated Website Testing with Amazon Nova Act

This blog post from AWS introduces how Epsilon company applies Amazon Nova Act and Amazon Bedrock AgentCore Browser to build an automated system for testing website interfaces using artificial intelligence. Traditional testing methods often require programmers to write code and define interface elements, which is time-consuming when the website changes. Epsilon's solution allows testing steps to be described in natural language, helping to simplify the testing process and reduce code maintenance.

**Key points to know:**

* Amazon Nova Act is a service designed to help build AI agents capable of interacting with website interfaces based on natural language instructions.

* Intent-driven UI Testing allows users to define testing objectives, eliminating the need to write code for every individual action on the interface.

* Amazon Bedrock AgentCore Browser provides a managed browser environment for executing automated test tasks.

* Natural Language Instructions enable the AI ​​to understand and perform actions such as entering data, clicking buttons, scrolling through pages, and verifying outcomes.

* Amazon S3 is used to store screenshots, reports, and the results of the testing process.

* AWS IAM facilitates access management and the isolation of testing environments across different development teams.

* Automated Test Reporting tracks the success or failure status of each test step, aiding in error analysis.

* The system can integrate AI-driven testing with Playwright, combining the AI’s ability to interpret interfaces with the stability of traditional testing methods.

According to Epsilon’s internal testing results, Amazon Nova Act reduces the effort required to build test scripts by approximately 4–6 times compared to an equivalent approach using Playwright. This solution demonstrates the potential of Agentic AI in automating software testing, shortening script development time, and enhancing the efficiency of quality management for web applications.

**Testing Service Architecture**
![Testing Service Architecture](/FCAJ_WorkShop/images/blog3.png)

**Original article link:**https://aws.amazon.com/vi/blogs/machine-learning/building-intent-driven-ui-testing-with-amazon-nova-act/