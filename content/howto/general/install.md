---
title: "Install Mendix Studio Pro"
category: "General Info"
menu_order: 1
description: "Follow this how-to to learn how to install Mendix Studio Pro."
toc-level: "2"
tags: ["studio pro", "install", "install studio pro", "download"]
---

## 1 Introduction

Mendix Studio Pro enables you to build apps on the Mendix Platform. This how-to will guide you through the steps of installing the latest version of Mendix Studio Pro.

For a deep-dive demonstration of how to install Studio Pro, follow along in this video:

<img
  style="width: 100%; margin: auto; display: block;"
  class="vidyard-player-embed"
  src="https://play.vidyard.com/WUp2tLi68nXFQd7xhPbDtt.jpg"
  data-uuid="WUp2tLi68nXFQd7xhPbDtt"
  data-v="4"
  data-type="inline"
/>

## 2 Prerequisites

Before starting this how-to, make sure you have completed the following prerequisites:

* A Windows environment to install Studio Pro (For the full list of supported systems and required frameworks, see [System Requirements](/refguide/system-requirements))

## 3 Downloading Mendix Studio Pro

Mendix Studio Pro can be installed on your machine with a Windows executable file. This executable file can be downloaded from the Mendix Marketplace. Follow these steps to download Mendix Studio Pro:

1. Go to the Studio Pro download page in the [Mendix Marketplace](https://appstore.home.mendix.com/link/modeler/).
2.  Click the **Download** button in the top-right corner to download the latest Mendix Studio Pro.


## 4 Installing Mendix Studio Pro {#install}

Mendix Studio Pro needs to be installed on your computer before you can start building apps. Follow these steps to install Mendix Studio Pro:

1.  Open the downloaded Mendix Studio Pro executable. It is named like this: *Mendix-9.X.X-Setup*. Then click **Next**:

	{{% image_container width="400" %}}![](attachments/install/setup-wizard.png)
	{{% /image_container %}}

2.  Select **I accept the terms in the License Agreement** and click **Next**:

	{{% image_container width="400" %}}![](attachments/install/terms-of-use.png)
	{{% /image_container %}}

3.  Select the folder in which you want to install Studio Pro and click **Next**:

	{{% image_container width="400" %}}![](attachments/install/select-folder.png)
	{{% /image_container %}}

4.  Enter the start menu shortcuts folder you want to use and click **Next**:

	{{% image_container width="400" %}}![](attachments/install/shortcut-folder.png)
	{{% /image_container %}}

5.  Check the desktop option to create a shortcut to Studio Pro on your desktop and click **Next**.
6.  Click **Install** to install Studio Pro on your computer:

	{{% image_container width="400" %}}![](attachments/install/ready-to-install.png)
	{{% /image_container %}}

7.  If you are asked to restart your computer, make a selection and click **Finish**. Otherwise, check **Launch Mendix 9.X.X** and click **Finish** to finish the installation and launch Studio Pro.

## 5 Troubleshooting {#troubleshooting}

Sometimes you can run into problems when installing Studio Pro. One work-around is to restart your system and install the prerequisites separately if they are not installed yet. 

The prerequisites are the following:

* [Microsoft .NET Framework 4.7.2](https://download.microsoft.com/download/6/E/4/6E48E8AB-DC00-419E-9704-06DD46E5F81D/NDP472-KB4054530-x86-x64-AllOS-ENU.exe)
* [AdoptOpenJDK 11](https://cdn.mendix.com/installer/AdoptOpenJDK/OpenJDK11U-jdk_x64_windows_hotspot_11.0.3_7.msi)
* [Microsoft Visual C++ 2010 SP1 Redistributable Package](http://download.microsoft.com/download/A/8/0/A80747C3-41BD-45DF-B505-E9710D2744E0/vcredist_x64.exe)
* [Microsoft Visual C++ 2015 Redistributable Package](https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe)
* [Mendix Native Mobile Builder](https://appdev-mx-cdn.s3.amazonaws.com/native-builders/latest.exe)


Based on the error message you get from the installer you can decide to install a single prerequisite, or you can try to manually install them all.

After that you can retry installing Studio Pro.

## 6 Installing Mendix Studio Pro Offline {#offline}

The Mendix Studio Pro installation experience includes all the tools and frameworks required to run the application. If any of the prerequisites are not found at the moment of installation, the Studio Pro setup process will attempt to download and install the missing elements automatically. The Mendix Studio Pro installer does not include all dependencies and relies on internet connectivity to obtain them if any of the required pieces of software are missing. 

It is possible to prepare the prerequisite installers beforehand, so that the Mendix Studio Pro setup process can pick them up instead of downloading from the remote location. Follow these steps to prepare the installers:

1. Create a folder for the Mendix Studio Pro installer.
2. Download the latest [Mendix Studio Pro installer](https://appstore.home.mendix.com/link/modelers/) and move it into folder you created.
3. Create a folder with the name **Dependencies** in the same location where the Mendix Studio Pro installer was placed.
4. Download the prerequisites listed in the [Troubleshooting](#troubleshooting) section above and move them into the **Dependencies** folder.
5. Rename the following dependencies:
	* The `.NET Framework 4.7.2` executable to `dotnetfx472.exe`
	* The `Java Development Kit 11 (x64)` *msi* to `adoptopenjdk_11_x64.msi`

 	* The `Visual C++ 2010 SP1 Redistributable (x64)` executable to `vcredist2010_x64.exe`
 	* The `Visual C++ Redistributable for Visual Studio 2015 (x64)` executable to `vcredist2015_x64.exe`
 	* The `latest` executable to `mendix_native_mobile_builder.exe`
6. Run the installer as described in the [Installing Mendix Studio Pro](#install) section above.

## 7 Read More

* [Studio Pro Overview](/refguide/studio-pro-overview)
* [App Modeling](/refguide/modeling)
