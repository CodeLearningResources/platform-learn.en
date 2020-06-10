---
title: Query Service - Getting Started
description: Query Service - Getting Started
kt: 5342
audience: Data Engineer, Data Architect, Data Analyst, BI Expert
doc-type: tutorial
activity: 
---

# 7.1 Getting Started

## Objectives

- Log in to Adobe Experience Platform
- Browse datasets
- Introduction to Query Service
- Connect PSQL client to Query Service

## 7.1.1 - Getting familiar with the Adobe Experience Platform UI

Make sure you are logged into the [Adobe Experience Platform UI](https://platform.adobe.com).

![platform-login.png](./images/platform-login.png)

## 7.1.2 - Explore data on the platform

Bringing data from different channels is a tough task for any brand. And in this exercise, Luma Telco customers are engaging with Luma Telco on its website, on its mobile app, purchase data is collected by Luma Telco’s Point of Sale system, and they have CRM and Loyalty data. Luma Telco is using Adobe Analytics and Adobe Launch to capture data across its website, mobile app as well as POS system, so this data is already flowing into Adobe Experience Platform. Let's begin with exploring all the data for Luma Telco that already exists in Adobe Experience Platform.

In the left menu, click **Datasets**.

![emea-website-interaction-dataset.png](./images/emea-website-interaction-dataset.png)

Luma Telco is streaming data into Adobe Experience Platform and this data is available in the `AEP Demo - Website Interactions` dataset. Search for `AEP Demo - Website Interactions`.

![emea-callcenter-interaction-dataset.png](./images/emea-website-interaction-dataset1.png)

Luma Telco's Callcenter Interaction data is captured in the `AEP Demo - Call Center Interactions` dataset. Search for `AEP Demo - Call Center Interactions` data in search box. Click on the dataset's name to get dataset details.

![emea-callcenter-interaction-dataset.png](./images/emea-callcenter-interaction-dataset.png)

After clicking the dataset, you will get an overview of the dataset activity such as ingested and failed batches.

![preview-interaction-dataset.png](./images/preview-interaction-dataset.png)

Click on **Preview Dataset** to see a sample of the data stored in `AEP Demo - Call Center Interactions` dataset. The left panel shows schema structure for this dataset.

![QS](./images/previewds.png)

You can open the schema structure by clicking on the schema's name in the left panel.

![explore-interaction-dataset.png](./images/explore-interaction-dataset.png)

Click the **Close** button to close the **Preview Dataset** window.

## 7.1.3 - Introduction to Query Service

Adobe Experience Platform Query Service is accessed by clicking on **Queries** in the left menu.

![select-queries.png](./images/select-queries.png)

By going to **Log** you'll see the Query List page, which provides you a list of all the queries that have run in this organization, with the latest at the top.

![query-list.png](./images/query-list.png)

Click on any SQL query from the list and observe the details provided in the right rail.

![click-sql-query.png](./images/click-sql-query.png)

You can scroll the window to see the entire query, or you can click on the icon highlighted below to copy the entire query to your notepad. You do not have to copy the query at this time.

![click-copy-query.png](./images/click-copy-query.png)

You can't just see the queries that have been executed, this User Interface lets you create new datasets from queries. These datasets can be linked to Adobe Experience Platform's Real-time Customer Profile or can be used as input for Adobe Experience Platform Data Science Workspace.

## 7.1.4 - Connect PSQL Client to Query Service

Query Service supports clients with a driver for PostgreSQL. In this we'll be using PSQL, a command-line interface, and Power BI or Tableau. Let's connect to PSQL.

Click on **Credentials**.

![queries-select-configuration.png](./images/queries-select-configuration.png)

You will see the screen below. The Configuration screen provides server information and credentials for authenticating to Query Service. For now, we will focus on the right side of the screen which contains a connect command for PSQL. Click on the Copy button to copy the command to your clipboard.

![copy-psql-connection.png](./images/copy-psql-connection.png)

For Windows: Open the command line by hitting the windows key and typing cmd  and then clicking on the Command Prompt result.

![open-command-prompt.png](./images/open-command-prompt.png)

For OSX: Open the terminal.app via spotlight search:

![open-terminal-osx.png](./images/open-terminal-osx.png)

Paste the connect command that you have copied from the Query Service UI and hit enter in the command prompt window:

Windows:

![command-prompt-connected.png](./images/command-prompt-connected.png)

OSX:

![command-prompt-paste-osx.png](./images/command-prompt-paste-osx.png)

You are now connected to Query Service using PSQL.

In the next exercises, there will be quite some interaction with this window. We will refer to it as your **PSQL command-line interface**.

Now you are ready to start submitting queries!

Next Step: [7.2 - Using the Query Service](./ex2.md)

[Go Back to Module 7](./query-service.md)

[Go Back to All Modules](../../overview.md)