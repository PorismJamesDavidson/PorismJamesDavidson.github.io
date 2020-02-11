---
title: Title
layout: default
---
{% comment %}
[Test](/page/)
<div id="readme"></div>
{% include README.md %}     
 
<div id="docs"></div>
{% endcomment %}

<!----- Conversion time: 0.718 seconds.


Using this Markdown file:

1. Cut and paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β17
* Tue Feb 11 2020 02:39:54 GMT-0800 (PST)
* Source doc: https://docs.google.com/a/porism.com/open?id=1yniNp9IaXveXWALlZivjOP5PE4g0rhDoEpj56b9H0pM
* This document has images: check for >>>>>  gd2md-html alert:  inline image link in generated source and store images to your server.

WARNING:
You have 5 H1 headings. You may want to use the "H1 -> H2" option to demote all headings by one level.

----->


<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 1; ALERTS: 1.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>



# OpenCommunity Data Standard Guidance

Version 1.0 This will be the version when it is finalised.


# Introduction

This document provides guidance on using the data standard for locally delivered services.

It is the successor to the Local Government Association’s (LGA’s) comma separated values (CSV) schema developed by iStandUK and published [here](https://schemas.opendata.esd.org.uk/ServiceDirectory) in February 2017. It constitutes the official schema developed in partnership by the LGA and partners involved in the [Local Digital](https://localdigital.gov.uk/) [OpenCommunity](https://opencommunity.org.uk/) programme.

The Standard conforms to and extends the international [Open Referral](https://openreferral.org/) standard.

The Standard is managed by a community of private, public and third sector organisations governed by an OpenCommunity Board. These details have yet to be determined.


# Purpose

The Data Standard defines the structure of data expected in interfaces between standards compliant software. It also gives ranges of expected values for some fields.

The standard determines the structure of responses to application programming interface (API) web methods that return service and related data. The [API is defined here](https://api.porism.com/ServiceDirectoryService/swagger-ui.html).

The standard provides for recording sufficient data to be able to identify a small targets set of services that closely meet the needs of a prospective service user, as given by the user’s location and circumstances.


# The Standards and Open Referral

The OpenReferral schema defines a structure for human services data. The openCommunity standard _extends_ Open Referral to support richer data where needed. It then _constrains_ the resultant schema by means of an _application profile_ which says what fields are recommended for English use and what external vocabularies to reference.



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/Copy-of0.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/Copy-of0.png "image_tooltip")


The application profile reflects user needs identified by LGA work with pilot councils and [proposed changes](https://opencommunitystandard.github.io/specification/#proposed-changes) recommended by [OpenCommunity discovery work](https://opencommunity.org.uk/wp-content/uploads/2019/05/Report-OpenCommunity-Data-standards.pdf). The document [Community Services Data as an Application Profile of Open Referral](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing) assigns MoSCoW (Must, Should, Could, Won’t) prioritisations to the proposed changes.

The standard defined here reflects LGA findings combined with “Must have” changes recommended by OpenCommunity.

This Entity Relation Diagram shows the structure of data, distinguishing parts of the core Open Referral standard used from extensions introduced for Open Community.

Embed [this ERD](https://raw.githubusercontent.com/esd-org-uk/human-services/master/Resources/LGA_ApplicationProfileBasicEntityRelationshipDiagram.png) and allow click to open the full diagram - review/change file name.

The remaining “should have”, “could have” and “won’t have” recommendations are shown in the following diagram. They will be introduced in future versions of the standard if there is a business case for doing so. Local implementations may also choose to implement them.

Embed [this ERD](https://raw.githubusercontent.com/esd-org-uk/human-services/master/Resources/OpenCommunityApplicationProfileERD.png) and allow click to open the full diagram - review/change file name.


# Data structure

The OpenCommunity standard is defined [here in JSON format](https://raw.githubusercontent.com/esd-org-uk/human-services/master/SchemaGenerator/Generator/ExtendedDataPackage.json) compliant with the [Open Knowledge Foundation’s tabular data package format](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json).

It comprises:



*   Tables, which may also be seen as classes in a data structure
*   Table fields, which may be seen as class properties

Service directories supporting the standard may keep their data in the structure given or may just transform it to that structure for API requests.

Each table and field is described below.

Embed [HTML documentation](http://htmlpreview.github.io/?https://github.com/esd-org-uk/human-services/blob/master/Schemas/documentation.html)


# See also

Separate document on using the API - To be written by Mike

See [Por10762 - Use of Taxonomies with OpenCommunity services data](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)

<p style="text-align: right">
Por10760</p>



<!-- Docs to Markdown version 1.0β17 -->

# End of file    
