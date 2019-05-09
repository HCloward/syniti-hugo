+++
title = "Collect Overview"
weight = 3
layout = "single"
solution = "Platform"
+++

# Collect Overview

Collect is a data repository management component that is a core entity
of many DSP® product offerings. Collect maintains a unified collection
of data from multiple, disparate systems without requiring users to
connect to the actual systems. It can be configured to extract the data
at scheduled intervals and at an individual table level. In this way,
the data can be kept in sync based on the processing schedule of each
data source. Collect also contains import groups to organize and manage
sets of tables.

Collect provides the option to use DBMoto® to pull data from SAP. This
integration provides change data capture; only changed data is pulled
from SAP instead of every table. The integration of DBMoto® provides
many benefits:

  - No dgSAP down time
  - Time savings
  - Network savings
  - Real-time visibility into SAP

## Setup and Configuration for Collect

Before getting started with Collect, verify the following has been
completed:

  - [Set up Security](../Sys_Admin/Use_Cases/Setting_security)
    (performed by an Administrator)
  - [Register Target and Source Data
    Sources](Config/Register_Target_and_Source_Data_Sources)
  - [Create DBMoto® Source
    Connections](Config/Create_DBMoto_Source_Connections)
  - [Encrypt Data Source
    Password](Config/Encrypt_CranSoft_DataSource_Password)
    (performed by an Administrator)
  - [Configure Parameters in
    Common](Config/Configure_Parameters_in_Common)
  - [Set up Connection Types](Config/Set_up_Connection_Types)
  - [Set up Schedule Groups](Config/Set_Up_Schedule_Groups)
