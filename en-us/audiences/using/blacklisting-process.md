---
title: Blacklisting process
seo-title: Blacklisting process
description: Blacklisting process
seo-description: Understand how blacklisting is managed in Adobe Campaign.
page-status-flag: never-activated
uuid: 7ea66167-1dc8-4c2d-b7a4-abd0e69f4f43
content-encoding: ISO-8859-1
aemsrcnodepath: /content/help/en/campaign/standard/audiences/using/blacklisting-process
contentOwner: sauviat
cq-designpath: /etc/designs/help
cq-lastmodified: 2018-04-11T07 13 45.901-0400
products: SG_CAMPAIGN/STANDARD
audience: audiences
content-type: reference
topic-tags: understanding-blacklisting-process
cq-template: /apps/help/templates/article-3
discoiquuid: 9f7de20a-d2be-4826-a0df-27bbe04be289
herogradient: light
isreadyforlocalization: false
jcr-created: 2018-03-15T09 01 17.793-0400
jcr-createdby: admin
jcr-description: Blacklisting process
jcr-ischeckedout: true
jcr-language: en_us
lochandoffdate: 2018-04-11T07 13 45.899-0400
navTitle: Blacklisting process
publishexternaldate: 2018-03-26
sha1: 724710ed0cf69894d75e98692ceac8cc185bf284
index: y
internal: n
snippet: y
---

# Blacklisting process

Blacklisting process

## Blacklisting from a recipient's profile

A recipient can be blacklisted (opt-out) by an operator directly from the profile **General** tab.

Select the channel from which you want to exclude the recipient, or the **No longer contact (by any channel)** option to exclude the recipient from all deliveries.

![](assets/blacklisting_profile.png)

## Blacklisting from a landing page

To give your recipients the ability to be blacklisted (opt-out) from any delivery, you have to create and publish a **BlackList** landing page. For more on landing pages creation, refer to [this page](../../channels/using/about-landing-pages.md).

Once a recipient clicks on the landing page link, the **No longer contact (by any channel)** option in the recipient's profile is automatically selected.

![](assets/blacklisting_allChannels.png)

To give your recipients the ability to be blacklisted from a specific channel, you have to create and publish a **Profile acquisition** landing page. The recipients will then be able to select the channels from which they want to be blacklisted. 