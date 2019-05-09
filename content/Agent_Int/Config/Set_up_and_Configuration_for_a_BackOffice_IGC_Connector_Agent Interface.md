+++
title = 'Set up and Configuration for a BackOffice IGC Connector Agent'
solution = 'Platform'
+++

# Set up and Configuration for a BackOffice IGC Connector Agent

## Overview

![](../../../Resources/Images/AgentDiagram.png)

The BackOffice IGC™ Connector Agent is a Windows service that presents
an HTTP interface to the DSP® on port 8000, and securely communicates
with the cloud at https://connect.boaweb.com over an encrypted channel
using TLS 1.2 or higher. The DSP transmits dspMigrate™ Wave metrics to
the cloud via the service. To view the Migration dashboard, navigate to
your instance of IGC (https://igc.boaweb.com) in a supported web
browser. If you need help to access your cloud instance, contact your
Customer Success team at <CustomerSuccess@boaweb.com>.

**NOTE:** Outgoing firewall policies must allow the service to initiate
a connection to connect.boaweb.com:443.

**NOTE:** To install and configure the Connector Agent, you must have
administration rights on the server where the Connector Agent will be
installed.

**NOTE:** An additional component will need to be added to your DSP
license to permit access to the Agent Interface WebApp and the Migration
dashboard. Contact your BOA Account Manager for more information. If you
do not have contact information then open a support ticket at
[https://support.boaweb.com](https://support.boaweb.com/).

## Prerequisites

DSP 7.0.1 or later must be installed.

Outbound traffic to port 443 and the following domain must be permitted
so that the Connector Agent can communicate with the IGC:

  - wss://connect.boaweb.com/ws
  - https://connect.boaweb.com/auth

**NOTE:** The standard deployment configuration requires the Connector
Agent to be installed on the same server as DSP. For alternative
configurations please contact support at
[https://support.boaweb.com](https://support.boaweb.com/) for
assistance.

## System Requirements for the BackOffice IGC Connector Agent

  - Windows Server 2016
  - Windows Server 2012 R2 64-bit

**NOTE:** The Migration dashboard can be used in Chrome, Internet
Explorer 11 and Safari. It is viewable on desktop, iOS 11 or later and
Android Oreo.

## Connector Agent Installation

The most common deployment scenario for the Connector Agent is
installation of the Windows Service on the DSP Application Server. An
overview of the process is below:

1.  Contact the IGC Provisioning team at <licenserequests@boaweb.com> at
    least **3 business days prior** to the day you are ready to install
    the Connector Agent to request:
    
      - The Connector Agent installer
      - The IGC token you will need to complete the Connector Agent
        install
      - A replacement DSP license to enable the Connector Agent
    
    **NOTE:** During installation of the Connector Agent Windows Service
    you will enter the token provided to you. This token permits secure
    authentication of on-premise components to the IGC tenant containing
    the Migration dashboard where metrics are displayed.

2.  [Install the Connector Agent on the DSP application
    server.](Install_the_BackOffice_IGC_Connector_Agent_Service)

3.  [Add the Agent URL to the *[Parameters -
    IGC](../../../Master_Data_Mgmt/dspConduct/Page_Desc/Parameters_IGC)*
    page in DSP.](Add_a_BackOffice_IGC_Connector_Agent_URL_in_DSP)

4.  [Test the connection to the Connector Agent in
    DSP.](Test_a_BackOffice_IGC_Agent_Connection_in_DSP)
