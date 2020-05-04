# Choosing the Right Data Science Services in Azure: <small><br>Scale, Automate, and Deploy with Ease</small>

<a href="https://emdata.ai"><img src="https://raw.githubusercontent.com/emdata-design/azure-data-science/master/assets/images/logo_emdata_300_blue.png" alt="emdata logo" align="right" width="115" hspace="10" vspace="0"/></a>

## Table of Contents
- [Introduction](#Introduction)
- [Machine Learning Options on Azure](#Machine-Learning-Options-on-Azure)
- [Azure Government](#Azure-Government)
- [Standard ML Modeling Workflow](#Standard-ML-Modeling-Workflow)
- [Hidden Technical Debt in Machine Learning Systems](#Hidden-Technical-Debt-in-Machine-Learning-Systems)
- [Ideal Data Science Team](#Ideal-Data-Science-Team)
- [Resources](#Resources)

## Introduction

Microsoft Azure offers a multitude of cloud-based products that simplify creating solutions that solve your analytical problems with machine learning and AI. Together these products help your team with all aspects of the data science process.

With _Choosing the Right Data Science Services in Azure: Scale, Automate, and Deploy with Ease_, we unpack the challenge in determining which Azure data science product is best suited to solve your analytical problems. We explore the most popular machine learning and AI products and describe how each fit into our machine learning workflow.

Our <a href="https://www.lucidchart.com/documents/embeddedchart/acf9aa5d-a85f-4786-bf56-e49a88a63bac" target="_blank">machine learning workflow</a>
covers the full lifecycle of the data science process from data acquisition to scaling and serving finished models on production systems. Within each of the tasks in the process, we explore the right Azure products that help us easily scale our solutions.

We also explore how to right-size <a href="https://raw.githubusercontent.com/emdata-design/azure-data-science/master/assets/Ideal%20Data%20Science%20Team.png" target="_blank">your data science team</a> to best utilize each product so you’re solving problems as quickly and cheaply as possible.

The materials here will help you understand how to choose the set of Azure machine learning and AI products that fit your data science team within a typical machine learning workflow, allowing you to scale, automate, and deploy analytical solutions with ease.

###  Machine Learning Options on Azure

There are a number of machine learning options on Azure that allow data analysts, data engineers, data scientists, and AI engineers work collaboratively on AI and ML models. 

<table cellspacing=0 border=1>
    <thead>
    <tr>
        <th style=min-width:50px></th>
        <th style=min-width:165px>Product</th>
        <th style=min-width:50px>What it is</th>
        <th style=min-width:50px>What you can do with it</th>
    </tr>
    </thead>
    <tr>
        <td><img src="assets\images\AML.png" width="45"/></td>
        <td style=min-width:50px>Azure Machine Learning service</td>
        <td style=min-width:50px>A managed cloud service for Machine Learning.</td>
        <td style=min-width:50px>Train, deploy, and manage models in Azure using Python, Azure CLI, and Azure portal.</td>
    </tr>
    <tr>
        <td><img src="assets\images\ADB.png" width="45"/></td>
        <td style=min-width:50px>Azure Databricks</td>
        <td style=min-width:50px>Apache Spark–based analytics platform with an integrated notebook interface that seamlessly integrates with Azure Active Directory (Azure AD) and data services.</td>
        <td style=min-width:50px>Build and deploy models and data workflows with big data.</td>
    </tr>
    <tr>
        <td><img src="assets\images\DSVM.png" width="45"/></td>
        <td style=min-width:50px>Azure Data Science Virtual Machine</td>
        <td style=min-width:50px>A virtual machine with preinstalled data science tools.</td>
        <td style=min-width:50px>Develop machine learning solutions in a preconfigured data science environment.</td>
    </tr>
    <tr>
        <td><img src="assets\images\SQL.png" width="45"/></td>
        <td style=min-width:50px>SQL Server Machine Learning Services</td>
        <td style=min-width:50px>Integrated with Microsoft SQL Server, this scalable analytics server supports the Python and R language.</td>
        <td style=min-width:50px>Build and develop models in an on-premises SQL server that scales to match the SQL Server engine. Microsoft Machine Learning Server is also available as a cluster type in Azure HDInsight.</td>
    </tr>
</table>

Two of these products -- Azure Machine Learning Service (Preview) and Azure Databricks -- allow you to build models from the ground up. The materials in this repository focus on the services within these two products.

###  Azure Government

As of May 2020, Azure Machine Learning Services is an [available product on Azure Government](https://azure.microsoft.com/en-us/global-infrastructure/services/?products=machine-learning-service&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia) and has [feature parity with the commercial version](https://devblogs.microsoft.com/azuregov/azure-government-releases-40-new-services-nearing-parity-with-azure-commercial/). Microsoft’s [Azure Government documentation](https://docs.microsoft.com/en-us/azure/azure-government/compliance/azure-services-in-fedramp-auditscope#azure-public-services-by-audit-scope) states that Azure Machine Learning has DoD CC SRG IL 2, FedRAMP Moderate, and FedRAMP High certifications.

Azure Databricks is expected to be in [preview on Azure Government by the end of Q2 2020](https://azure.microsoft.com/en-us/global-infrastructure/services/?products=databricks&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia) at the US Gov Arizona and US Gov Virginia locations.

More details in the table below:

<table border>
<head>
<tr>
    <th style=min-width:155px>Product</th>
    <th style=min-width:50px>US DoD Central</th>
    <th style=min-width:50px>US DoD East</th>
    <th style=min-width:50px>US Gov Arizona</th>
    <th style=min-width:50px>US Gov Iowa</th>
    <th style=min-width:50px>US Gov Texas</th>
    <th style=min-width:50px>US Gov Virginia</th>
</tr>
</head>
<tbody>
<tr>
    <td style=min-width:50px>Azure Databricks </td>
    <td style=min-width:50px>Not available</td>
    <td style=min-width:50px>Not available</td>
    <td style=min-width:50px>Not available</td>
    <td style=min-width:50px>Preview expected: Q2 2020</td>
    <td style=min-width:50px>Not available</td>
    <td style=min-width:50px>Preview expected: Q2 2020</td>
</tr>
<tr>
    <td style=min-width:50px>Azure Machine Learning</td>
    <td style=min-width:50px>Not available</td>
    <td style=min-width:50px>Not available</td>
    <td style=min-width:50px>Not available</td>
    <td style=min-width:50px>Available</td>
    <td style=min-width:50px>Not available</td>
    <td style=min-width:50px>Available</td>
</tr>

</tbody>
</table>

###  Standard ML Modeling Workflow

_(click on the image below to view the original diagram)_
[![Machine learning workflow](https://raw.githubusercontent.com/emdata-design/azure-data-science/master/assets/Standard%20ML%20Modeling%20Workflow.png)](https://www.lucidchart.com/documents/embeddedchart/acf9aa5d-a85f-4786-bf56-e49a88a63bac)

###  Hidden Technical Debt in Machine Learning Systems



![Hidden Technical Debt in Machine Learning Systems](https://raw.githubusercontent.com/emdata-design/azure-data-science/master/assets/Hidden%20Technical%20Debt%20in%20Machine%20Learning%20Systems.png)

###  Ideal Data Science Team

![Ideal Data Science Team](https://raw.githubusercontent.com/emdata-design/azure-data-science/master/assets/Ideal%20Data%20Science%20Team.png)

###  Resources



