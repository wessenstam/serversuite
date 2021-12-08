.. _l1:

--------------------------------------
Installation and initial configuration
--------------------------------------

Introduction
------------

This first lab will cover:

1. Initial installation of Server Suite, Authentication and Privilege
2. Initial configuration


Greensafe Payroll Services has recently purchased Centrify Server Suite. Alex Foster has been identified as the project engineer in charge of implementing the solution. In this exercise, Alex (you) will install Centrify Authentication and Privilege.

.. note::
    Estimated time to complete this lab: **20 minutes**


Installation and Configuration
******************************

Systems used in this lab:

- dc.greensafe.lab
- apps-server.greensafe.lab

Installation
^^^^^^^^^^^^

#. Login to **apps-server.greensafe.lab** with the following credentials: 

   - **Username:** afoster
   - **Password:** *Provided by Trainer*

#. Open Windows Explorer and navigate to C:\\Share\\CSS2021.1
#. Launch the **Autorun** application and click **Authentication and Privilege**
#. When prompted to install Microsoft SQL Compact 4.0 for support of the Sudoers Import process, click **NO**
#. At the Welcome Message, click **Next**
#. Accept the EULA and click **Next**
#. Enter the Company Name **Greensafe Payroll Services**
#. Under *Property Components*, expand *Centrify Utilities* and click the **checkbox** next to *Zone Provisioning Agent*
#. Click **Next**
#. Under the *Destination* folder, click **Next**
#. Under *Confirm Settings*, click **Next**
#. Once completed, **UNCHECK** the options to configure the following products:

   - Centrify Reporting Services
   - Centrify Zone Provisioning Agent

#. Click **Finish**
#. Click **Yes** when prompted about using a Local system account to manage the Zone Provisioning Agent (ZPA)
#. **Close** the Centrify Server Suite Installation Package

Configuration
^^^^^^^^^^^^^

In this exercise, Alex (you) will complete the initial configuration of the solution using the management console, Centrify Access Manager. This configuration will include the creation of an active directory deployment structure and licensing.

#. While still being on the *apps-server.greensfae.lab* Open Windows Explorer and navigate to **C:\\Share**
#. Open **Training License Keys** and copy the **DirectControl License Key** to the clipboard
#. **Close** the file
#. Launch C**entrify Access Manager** from the Desktop shortcut
#. Click **OK** to connect to **dc-server.greensafe.lab**
#. At the *Welcome Message*, click **Next**
#. Under *User Credentials*, maintain the default setting and click **Next**
#. Under *Generate Centrify Recommended Deployment Structure*, Click the **checkbox** to generate the structure and click Next
#. Under *Choose Container*, click **Browse**
#. Select **greensafe.lab**
#. Click **Next**
#. Click **Next** once the deployment structure container has been populated
#. When the deployment structure has been created successfully, click **Next**
#. Under *Install License*, maintain the default container and click **Next**
#. When prompted, click **yes** to grant all users read permissions to the license container
#. Paste the License key (copied earlier) in the space provided and click **Add**
#. Click **Next**
#. Under the *Default Container for Zones*, maintain the default settings and click **Next**
#. Under *Delegate Permission*, maintain the default settings and click **Next**
#. Under *AD Admin Notification Handler*, maintain the default settings and click **Next**
#. Under *Setup Properties Pages*, maintain the default settings and click **Next**
#. Under *Summary*, Click **Next**
#. Click **Finish** to complete the initial configuration wizard


.. raw:: html

    <hr><CENTER>
    <H2 style="color:#80BB01">This concludes this lab</font>
    </CENTER>
