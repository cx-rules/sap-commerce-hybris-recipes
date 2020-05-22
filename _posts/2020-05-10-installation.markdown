---
layout: post
title: "Installation"
date: 2020-05-10
description: How to install SAP Commerce (Hybris) on Windows.
img:  # Add image post (optional)
---
## SAP Commerce (Hybris) website

### Go to: <https://help.sap.com/viewer/product/SAP_COMMERCE/1905/en-US>.

{% include screenshot.html
	div-name="SAPCommerceWebsite"
	img-name="SAPCommerceWebsite.png"
	img-description="SAP Commerce (Hybris) website"
%}

{% include arrow.html %}

## Go to "Installing and Upgrading"

{% include screenshot.html
	div-name="SAPCommerceWebsite_Implement"
	img-name="SAPCommerceWebsite_Implement.png"
	img-description="SAP Commerce (Hybris) installing and upgrading"
%}

{% include arrow.html %}

## Navigate to "Third-Party Compatibility"

### Download SAP Virtual Machine

{% include screenshot.html
	div-name="SAPCommerce3rdPartyCompatibility"
	img-name="SAPCommerce3rdPartyCompatibility.png"
	img-description="SAP Commerce 3rd party compatibility"
%}

{% include arrow.html %}

## Agree to leave SAP website

{% include screenshot.html
	div-name="3rdPartyCompatibilityLeaveSAP"
	img-name="3rdPartyCompatibilityLeaveSAP.png"
	img-description="SAP Commerce 3rd party compatibility - leave SAP website"
%}

{% include arrow.html %}

## Download SAP Virtual Machine

{% include screenshot.html
	div-name="DownloadSAPMachine"
	img-name="DownloadSAPMachine.png"
	img-description="Download SAP Java Virtual Machine"
%}

{% include arrow.html %}

## Extract the ZIP file

{% include screenshot.html
	div-name="SAPMachineDownloaded"
	img-name="SAPMachineDownloaded.png"
	img-description="SAP Java Virtual Machine is downloaded"
%}

{% include arrow.html %}

## Extract SAP JDK

{% include screenshot.html
	div-name="ExtractedSAPJDK"
	img-name="ExtractedSAPJDK.png"
	img-description="Extract SAP JDK..."
%}

{% include arrow.html %}

## Set environment variables (user variables)

### E.g. `JAVA_HOME = C:\java\sapmachine-jdk-11.0.7`
### Add this to Path: `%JAVA_HOME%\bin`

{% include arrow.html %}

## Verify Java Version

{% include screenshot.html
	div-name="VerifyJavaVersion"
	img-name="VerifyJavaVersion.png"
	img-description="Verify Java version"
%}

{% include arrow.html %}

## Extract Hybris ZIP file

### File will be in format: `CXCOMM190500P_X-XXXXXXXX.zip`.
### Target directory should be close to root, no spaces.

{% include arrow.html %}

## Directory structure

{% include screenshot.html
	div-name="DirectoryStructure"
	img-name="DirectoryStructure.png"
	img-description="Directory structure"
%}

{% include arrow.html %}

## Navigate to `hybris\bin\platform`

{% include arrow.html %}

## Run `setantenv.bat`

{% include screenshot.html
	div-name="SetAntEnv"
	img-name="SetAntEnv.png"
	img-description="Run setantenv.bat"
%}

{% include arrow.html %}

## Run `ant clean all`

{% include arrow.html %}

## Choose `develop` configuration template

{% include screenshot.html
	div-name="DevelopProduction"
	img-name="DevelopProduction.png"
	img-description="Choose develop or production"
%}

{% include arrow.html %}

## Build will run for several minutes

{% include screenshot.html
	div-name="BuildRunning"
	img-name="BuildRunning.png"
	img-description="Build running"
%}

{% include arrow.html %}

## Build is complete

{% include screenshot.html
	div-name="BuildFinished"
	img-name="BuildFinished.png"
	img-description="Build finished"
%}

{% include arrow.html %}

## Set admin password

### Edit file `hybris\config\local.properties`.
### Set property `initialpassword.admin=<yourSecurePass>`.

{% include arrow.html %}

## Run `ant initialize`

{% include screenshot.html
	div-name="AntInitializeStart"
	img-name="AntInitializeStart.png"
	img-description="Ant initialize - started"
%}

{% include screenshot.html
	div-name="AntInitializeFinished"
	img-name="AntInitializeFinished.png"
	img-description="Ant initialize - finished"
%}

{% include arrow.html %}

## Run `hybrisserver.bat`

{% include screenshot.html
	div-name="HybrisStartBeginning"
	img-name="HybrisStartBeginning.png"
	img-description="Ant start - beginning"
%}

{% include arrow.html %}

## Message `INFO: Server startup in 26438 ms` signifies successful start.