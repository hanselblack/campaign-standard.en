---
title: Control rules
seo-title: Control rules
description: Control rules
seo-description: Learn how to reinforce the quality check of your messages with control rules.
uuid: 336c320a-9354-4ba4-8934-19678824059f
content-encoding: ISO-8859-1
aemsrcnodepath: /content/help/en/campaign/standard/administration/using/control-rules
contentOwner: sauviat
cq-designpath: /etc/designs/help
cq-lastmodified: 2018-07-25T09 29 32.020-0400
cq-lastreplicated: 2018-07-23T05 53 53.223-0400
cq-lastreplicatedby: sauviat
cq-lastreplicationaction: Activate
products: SG_CAMPAIGN/STANDARD
audience: administration
content-type: reference
topic-tags: working-with-typology-rules
cq-template: /apps/help/templates/article-3
discoiquuid: 421147d7-2be9-4229-984e-f338b7a4fc59
firstPublishExternalDate: 2018-07-23T05:53:53.161-0400
herogradient: light
isreadyforlocalization: false
jcr-created: 2018-02-16T08 03 06.782-0500
jcr-createdby: admin
jcr-description: Control rules
jcr-ischeckedout: true
jcr-language: en_us
lastPublishExternalDate: 2018-07-23T05:53:53.161-0400
lochandoffdate: 2018-07-25T09 29 32.020-0400
loclangtag: locales fr;locales de;locales ja
lr-lastreplicatedby: sauviat@adobe.com
navTitle: Control rules
publishexternaldate: 2018-07-23T05 53 53.161-0400
publishExternalURL: https://helpx.adobe.com/campaign/standard/administration/using/control-rules.html
sha1: 27832c0719861ab988cff29848787c243049a170
topicBrowsingSortDate: 2018-07-23T05:53:53.161-0400
index: y
internal: n
snippet: y
---

# Control rules

Control rules

Control rules allow the user to check the validity and quality of the messages before they are sent, such as character display, SMS message size, address format, etc.

A set of default rules available in Adobe Campaign ensures the standard controls:

* **Check subject** (email): checks that the subject and sender address do not contain special characters which may cause problems on certain mail transfer agents, and checks that the message subject has been completed.
* **Check URL labels** (email): checks that each tracking URL has a label.
* **Check URLs** (email): checks the tracking URLs (presence of the "&" character).
* **Check proof size** (all channels): generates an error message if the proof target population exceeds 100 recipients.
* **Check unsubscription link** (email): checks for the presence of at least one unsubscription (opt-out) URL in each content (HTML and Text).
* **Check delivery size** (all channels): checks the size of the messages.
* **Check social network sharing link** (email): checks the presence of a link to a mirror page when including a social network sharing link (ViralLinks) in the content.
* **A/B Test**: extracts the test population for a delivery with an A/B test.

You can choose the moment at which the rule will be applied from one of the phases of the delivery's life cycle. Select the value to apply in the drop-down list from the **Phase** field of the typology rule.

![](assets/typology_phase.png)

Possible values are:

* **At the start of targeting**

  The control rule can be applied at this phase so that the personalization step is not executed in the event of an error.

* **After targeting**

  If you need to know the volume of the target in order to apply the control rule, select this phase.

  For example, the **Check proof size** control rule applies after the targeting stage: this rule prevents the preparation of message personalization if there are too many proof recipients.

* **At the start of personalization**

  This phase must be selected if the check concerns approving message personalization. Message personalization is carried out during the analysis phase.

* **At the end of the analysis**

  When a check requires message personalization to be complete, select this phase.
