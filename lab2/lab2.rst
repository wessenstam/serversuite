.. _l1:

-----
Zones
-----

Introduction
------------

This second lab will cover:

1. Creation of Zones
2. Preparing Zone Server objects

In this exercise, Alex (you) will continue the initial configuration of the Centrify solution by assigning Centrify Administrators and creating Parent and Child Zones for Centrify privilege management. There will be one Global Zone for all users, and two child zones based on server operating systems.

| As part of your preparations to implement Centrify Server Suite features to the infrastructure, you can prepare the objects prior to the implementation of each server. This will avoid any interruptions in service and provide you the opportunity to confirm effective security rights are accurate. In this exercise, Alex (you) will use Centrify Access Manager to create the AD objects in the appropriate Centrify Zones so they are organized properly and effective rights are applied prior to the server being joined.


.. note::
    Estimated time to complete this lab: **25 minutes**

Creation of Zones
*****************

Systems used in this lab:

- dc.greensafe.lab
- apps-server.greensafe.lab

#. Open Active Directory Users and Computers (ADUC).
#. Navigate to Centrify Centrify Administration
#. Open the AD group cfyA_Global_CentrifyAdmins.
#. Click Members.
#. Click Add.
#. Add Team_Security and close the group properties.
#. Close ADUC. Let’s now create the Parent Zone
#. Open Centrify Access Manager.
#. Expand Centrify Access Manager (dc-server.greensafe.lab).
#. Right Click on Zones and select Create New Zone.
#. Name the new zone Global Zone.
#. Click Next
#. Click Finish Let’s now delegate zone controls to the appropriate administrators
#. Right Click the new Global Zone and select Delegate Zone Control.
#. Click Add.
#. Search for and add the AD group cfyA_Global_CentrifyAdmins.
#. Click Next.
#. Under Tasks to Delegate, click All.
#. Click Next.
#. When prompted about the msDS-azScope objects, click Yes.
#. Click Finish. Let’s now create the Child Zones.
#. Right Click Global Zone and select Create Child Zone.
#. Name the new child zone UNIX Zone.
#. Click Next.
#. Click Finish. We have to remember to delegate zone controls to each zone. In some cases, you may have different administrators responsible for each zone.
#. Right Click the new UNIX Zone and select Delegate Zone Control.
#. Click Add.
#. Search for and add the AD group cfyA_Global_CentrifyAdmins.
#. Click Next.
#. Under Tasks to Delegate, click All.
#. Click Next.
#. When prompted about the msDS-azScope objects, click Yes.
#. Click Finish. Let’s now create the Windows Child Zones.
#. Right Click Global Zone and select Create Child Zone.
#. Name the new child zone Windows Zone.
#. Click Next.
#. Click Finish. Don’t forget to delegate zone controls for this zone.
#. Right Click the new Windows Zone and select Delegate Zone Control.
#. Click Add.
#. Search for and add the AD group cfyA_Global_CentrifyAdmins.
#. Click Next.
#. Under Tasks to Delegate, click All.
#. Click Next.
#. When prompted about the msDS-azScope objects, click Yes.
#. Click Finish.

.. raw:: html

    <hr><CENTER>
    <H2 style="color:#80BB01">This concludes this lab</font>
    </CENTER>
