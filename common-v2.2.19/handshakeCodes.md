---
layout: default-layout
title: Handshake Codes Management
keywords: Handshake Codes, manage license
description: This page is about managing handshake codes for licenses.
breadcrumbText: Handshake Codes
needAutoGenerateSidebar: true
---

# Manage the Handshake Codes for your licenses

> Read more on [what is a Handshake Code]({{site.about}}terms.html#handshake-code).

Dynamsoft trackable licenses are consumed through Handshake codes. When you click on "Configure the License" after activating a license or "Manage the License" for each activated license, you will land on the "Manage the Handshake Codes" page where you can

* [View existing handshake codes](#view-existing-handshake-codes)
* [Add new handshake codes](#add-a-handshake-code)
* [Edit existing handshake codes](#edit-a-handshake-code)
* [View the statistcs of a handshake code](#show-statistics)
* [Change license usage order](#change-license-usage-order) for handshake codes that have moer than one license item configured

We'll dive deeper into these topics below.

## View existing Handshake Codes

For Dynamsoft-Hosting License Tracking, a Handshake Code is generated by default for each activated License which may contain one or multiple License Items.

For Self-Hosting License Tracking, DLS generates a default Handshake Code for each imported License File.

After that, you can [add more Handshake Codes](#add-a-handshake-code) or [edit the existing Handshake Codes](#edit-a-handshake-code). For a Handshake Code that points to multiple License Items, you can also [Change License Usage Order](#change-license-usage-order).

> NOTE
>  
> Although default Handshake Codes are generated on a per purchase order basis, the Handshake Code itself has nothing to do with the purchase order. Instead, it is only related to the License Items configured to it, and these items can be from any order.s

## Add a Handshake Code

When you add a Handshake Code, you can configure it in a few ways

* Assign a string as the name of the Handshake Code. 

  The name of a Handshake Code consists of two parts

  {Dynamsoft ID} - {custom string}

  The first part is your Dynamsoft id and cannot be changed. The second part can be any valid string. For example

  + 216998-100025900
  + 216998-vehicleCode

* Set one or multiple validation field(s). 

> Read more on [what is a Validation Field]({{site.about}}terms.html#validation-field)

* Set a Session Password

> Read more on [what is a Session Password]({{site.about}}terms.html#session-password)

* Configure License Items for the Handshake Code

  All activated License Items will show up on the page, you can choose one or multiple items and add it to the Handshake Code.

## Edit a Handshake Code

You can edit any existing Handshake Code, the things you can change are exactly the same as when you [add a Handshake Code](#add-a-handshake-code).

> For Dynamsoft-Hosting License Tracking, the default names for the auto-generated Handshake Codes can not be changed.

## Change License Usage Order

If multiple License Items are configured to one Handshake Code, the question of which License Item is used first will arise. Dynamsoft Dynamsoft License Server has a default order which follows these rules

* The one with the closest expiration date is consumed first or
* The one containing the most specific permit is consumed first or
* The one containing the least restrictive permit is consumed first

With the default order, the Handshake Code should be able to take full advantage of all License Items. However, you can still rearrange the order as you see fit by clicking on the button "Change License Usage Order".

## View Statistics

<!-- Statistics per Item is also supported in 2.1 -->
You can click "View Statistics" under a Handshake Code to view its statistics.

On the top of the statistics page, you will see all the License Items configured to this Handshake Code. You can click the id of each License Item to view its own statistics.

> NOTE: Adding or removing License Items to/from the Handshake Code will not affect the historical figures for that Handshake Code.

Below the License Items, you can see a chart showing usage over a period of time. When you click on a certain date on the chart, you can view detailed usage of that day at the bottom of the page.

## Use a Handshake Code

A Handshake Code authorizes a client device to use a Dynamsoft software. Check out [How to Configure DLS]({{site.common}}mechanism.html#configure-dls) for more information.