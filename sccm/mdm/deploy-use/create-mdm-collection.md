---
title: "Create an MDM collection"
titleSuffix: "Configuration Manager"
description: "Create an MDM collection using Configuration Manager."
ms.date: 03/21/2019
ms.prod: configuration-manager
ms.technology: configmgr-hybrid
ms.topic: conceptual
ms.assetid: d1b4337f-85e8-45e6-8bbe-9f18b49041c7
author: aczechowski
ms.author: aaroncz
manager: dougeby
ms.collection: M365-identity-device-management
---
# Create an MDM collection with Configuration Manager and Microsoft Intune

*Applies to: Configuration Manager (current branch)*

A Configuration Manager user collection is required to specify the users who can enroll devices into management. You can only use user collections (instead of device collections) because Intune licenses are assigned by user.

> [!NOTE]
> To enroll devices with Intune, you do not need to assign licenses to users in the Microsoft 365 admin center or Azure Active Directory portal. Including the users in a collection that gets associated with the Intune subscription (in a [later step](configure-intune-subscription.md)) is all that's required.

For testing purposes you can set up a **Direct rule** and add specific users who can enroll devices. In the Configuration Manager console, choose, **Assets and Compliance** > **User Collections**, click the **Home** tab > **Create** group, and then click **Create User Collection**. For broader distribution you should use **Query rules** to define users. For more information about collections, see [How to create collections](https://technet.microsoft.com/library/mt629371.aspx).

![Create a user collection for MDM](../media/mdm-create-user-collection.png)

> [!div class="button"]
> [Next step >](confirm-dns.md)
