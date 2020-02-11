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

OpenCommunity Data Standard Guidance

Version 1.0 This will be the version when it is finalised.

Introduction
============

This document provides guidance on using the data standard for locally delivered services.

It is the successor to the Local Government Association's (LGA's) comma separated values (CSV) schema developed by iStandUK and published [here](https://schemas.opendata.esd.org.uk/ServiceDirectory) in February 2017. It constitutes the official schema developed in partnership by the LGA and partners involved in the [Local](https://localdigital.gov.uk/)[  ](https://localdigital.gov.uk/)[Digital](https://localdigital.gov.uk/) [OpenCommunity](https://opencommunity.org.uk/) programme.

The Standard conforms to and extends the international [Open](https://openreferral.org/)[  ](https://openreferral.org/)[Referral](https://openreferral.org/) standard.

The Standard is managed by a community of private, public and third sector organisations governed by an OpenCommunity Board. These details have yet to be determined.

Purpose
=======

The Data Standard defines the structure of data expected in interfaces between standards compliant software. It also gives ranges of expected values for some fields.

The standard determines the structure of responses to application programming interface (API) web methods that return service and related data. The [API](https://api.porism.com/ServiceDirectoryService/swagger-ui.html)[  ](https://api.porism.com/ServiceDirectoryService/swagger-ui.html)[is](https://api.porism.com/ServiceDirectoryService/swagger-ui.html)[  ](https://api.porism.com/ServiceDirectoryService/swagger-ui.html)[defined](https://api.porism.com/ServiceDirectoryService/swagger-ui.html)[  ](https://api.porism.com/ServiceDirectoryService/swagger-ui.html)[here](https://api.porism.com/ServiceDirectoryService/swagger-ui.html).

The standard provides for recording sufficient data to be able to identify a small targets set of services that closely meet the needs of a prospective service user, as given by the user's location and circumstances.

The Standards and Open Referral
===============================

The OpenReferral schema defines a structure for human services data. The openCommunity standard *extends* Open Referral to support richer data where needed. It then *constrains* the resultant schema by means of an *application profile* which says what fields are recommended for English use and what external vocabularies to reference.

![Schema extension and constraint](file:///C:/Users/James/AppData/Local/Packages/oice_16_974fa576_32c1d314_28ea/AC/Temp/msohtmlclip1/01/clip_image001.png)

The application profile reflects user needs identified by LGA work with pilot councils and [proposed](https://opencommunitystandard.github.io/specification/#proposed-changes)[  ](https://opencommunitystandard.github.io/specification/#proposed-changes)[changes](https://opencommunitystandard.github.io/specification/#proposed-changes) recommended by [OpenCommunity](https://opencommunity.org.uk/wp-content/uploads/2019/05/Report-OpenCommunity-Data-standards.pdf)[  ](https://opencommunity.org.uk/wp-content/uploads/2019/05/Report-OpenCommunity-Data-standards.pdf)[discovery](https://opencommunity.org.uk/wp-content/uploads/2019/05/Report-OpenCommunity-Data-standards.pdf)[  ](https://opencommunity.org.uk/wp-content/uploads/2019/05/Report-OpenCommunity-Data-standards.pdf)[work](https://opencommunity.org.uk/wp-content/uploads/2019/05/Report-OpenCommunity-Data-standards.pdf). The document [Community](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[Services](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[Data](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[as](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[an](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[Application](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[Profile](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[of](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[Open](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[  ](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing)[Referral](https://docs.google.com/document/d/16E59vkv2a1khiPHDZJfg00p6ukD1Dhe9z4EJZNxnkzA/edit?usp=sharing) assigns MoSCoW (Must, Should, Could, Won't) prioritisations to the proposed changes.

The standard defined here reflects LGA findings combined with "Must have" changes recommended by OpenCommunity.

This Entity Relation Diagram shows the structure of data, distinguishing parts of the core Open Referral standard used from extensions introduced for Open Community.

Embed [this](https://raw.githubusercontent.com/esd-org-uk/human-services/master/Resources/LGA_ApplicationProfileBasicEntityRelationshipDiagram.png)[  ](https://raw.githubusercontent.com/esd-org-uk/human-services/master/Resources/LGA_ApplicationProfileBasicEntityRelationshipDiagram.png)[ERD](https://raw.githubusercontent.com/esd-org-uk/human-services/master/Resources/LGA_ApplicationProfileBasicEntityRelationshipDiagram.png) and allow click to open the full diagram - review/change file name.

The remaining "should have", "could have" and "won't have" recommendations are shown in the following diagram. They will be introduced in future versions of the standard if there is a business case for doing so. Local implementations may also choose to implement them.

Embed [this](https://raw.githubusercontent.com/esd-org-uk/human-services/master/Resources/OpenCommunityApplicationProfileERD.png)[  ](https://raw.githubusercontent.com/esd-org-uk/human-services/master/Resources/OpenCommunityApplicationProfileERD.png)[ERD](https://raw.githubusercontent.com/esd-org-uk/human-services/master/Resources/OpenCommunityApplicationProfileERD.png) and allow click to open the full diagram - review/change file name.

Data structure
==============

The OpenCommunity standard is defined [here](https://raw.githubusercontent.com/esd-org-uk/human-services/master/SchemaGenerator/Generator/ExtendedDataPackage.json)[  ](https://raw.githubusercontent.com/esd-org-uk/human-services/master/SchemaGenerator/Generator/ExtendedDataPackage.json)[in](https://raw.githubusercontent.com/esd-org-uk/human-services/master/SchemaGenerator/Generator/ExtendedDataPackage.json)[  ](https://raw.githubusercontent.com/esd-org-uk/human-services/master/SchemaGenerator/Generator/ExtendedDataPackage.json)[JSON](https://raw.githubusercontent.com/esd-org-uk/human-services/master/SchemaGenerator/Generator/ExtendedDataPackage.json)[  ](https://raw.githubusercontent.com/esd-org-uk/human-services/master/SchemaGenerator/Generator/ExtendedDataPackage.json)[format](https://raw.githubusercontent.com/esd-org-uk/human-services/master/SchemaGenerator/Generator/ExtendedDataPackage.json) compliant with the [Open](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[  ](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[Knowledge](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[  ](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[Foundation](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)['](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[s](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[  ](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[tabular](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[  ](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[data](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[  ](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[package](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[  ](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json)[format](https://raw.githubusercontent.com/openreferral/specification/master/datapackage.json).

It comprises:

● Tables, which may also be seen as classes in a data structure

● Table fields, which may be seen as class properties

Service directories supporting the standard may keep their data in the structure given or may just transform it to that structure for API requests.

Each table and field is described below.

Embed [HTML](http://htmlpreview.github.io/?https://github.com/esd-org-uk/human-services/blob/master/Schemas/documentation.html)[  ](http://htmlpreview.github.io/?https://github.com/esd-org-uk/human-services/blob/master/Schemas/documentation.html)[documentation](http://htmlpreview.github.io/?https://github.com/esd-org-uk/human-services/blob/master/Schemas/documentation.html)

See also
========

Separate document on using the API - To be written by Mike

See [Por](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[10762 - ](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[Use](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[  ](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[of](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[  ](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[Taxonomies](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[  ](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[with](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[  ](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[OpenCommunity](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[  ](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[services](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[  ](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)[data](https://docs.google.com/document/d/1UiYBv_Lgmj4CWCi_AXZEjso-SY-5ypwFLB4HZgy5lYM/edit?usp=sharing)

Por10760
# End of file    
