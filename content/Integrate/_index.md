+++
title = "Integrate Overview"
weight = 3
layout = "single"
solution = "Platform"
+++

# Integrate Overview

Integrate is a component of the BackOffice Data Stewardship Platform
(DSP)® that contains loading mechanisms to push data into an ERP system.

Integrate loads data to SAP using:

  - Batch Data Communication (BDC) processing
  - Graphical User Interface (GUI) scripting
  - A Remote Function Call (RFC) or a BAPI

Integrate can also create and transfer user defined text files formatted
as Delimited, Fixed Width, or XML to the SAP server.

Integrate uses standard SAP posting functionality as well as BackOffice
delivered custom processing and can be used by any platform component
(including the framework) to post data to the target system.

Integrate is organized into templates and processes. A template is based
on a template type and defines how data is posted into an ERP system.
Templates are not tied to data, but rather act as an independent guide
for posting that can be assigned to many processes. A process is a
series of posting steps that defines how Integrate takes data from the
component and loads it into SAP.

**NOTE:** Integrate is an automation tool that allows experienced SAP
users to leverage data loading capabilities provided by SAP. knowledge
of how to use SAP loading technologies such as BDC is required to use
Integrate and the documentation and technical support included does not
cover specific usage details or how this technology works. The use cases
provided are examples only and do not supply comprehensive instructions
to suit all situations.

## Setup and Configuration for Integrate

Before getting started with Integrate, verify the following steps have
been completed:

**NOTE:** These steps should only be completed by a developer or a
system administrator.

1.  [Set up Security](Config/Set_up_Security_for_Integrate.htm)
2.  [Configure Parameters](Config/Configure_ParametersIntegrate.htm)
3.  [Establish a Connection to a Target
    System](../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
4.  [Create Categories](Config/Create_Categories.htm)

A user can also [Extract RFC
Functions](Config/Extract_RFC_Functions.htm).
