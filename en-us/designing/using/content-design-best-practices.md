---
title: Content design best practices
seo-title: Content design best practices
description: Content design best practices
seo-description: Read about these guidelines to ensure the editor's optimal operation.
uuid: 5061d036-5633-4ddd-93f2-05bc571552b3
content-encoding: ISO-8859-1
aemsrcnodepath: /content/help/en/campaign/standard/designing/using/content-design-best-practices
contentOwner: sauviat
cq-designpath: /etc/designs/help
cq-lastmodified: 2018-07-26T02 53 20.971-0400
cq-lastreplicated: 2018-07-23T08 13 16.032-0400
cq-lastreplicatedby: sauviat
cq-lastreplicationaction: Activate
products: SG_CAMPAIGN/STANDARD
audience: designing
content-type: reference
topic-tags: about-content-design
cq-template: /apps/help/templates/article-3
discoiquuid: 713d4a82-e414-4d2d-933a-c824de2230a0
firstPublishExternalDate: 2018-07-23T05:57:28.019-0400
herogradient: light
isreadyforlocalization: false
jcr-created: 2018-07-23T07 30 12.604-0400
jcr-createdby: admin
jcr-description: Content design best practices
jcr-ischeckedout: true
jcr-language: en_us
lastPublishExternalDate: 2018-07-23T08:13:15.962-0400
lochandoffdate: 2018-07-26T02 53 20.971-0400
loclangtag: locales fr;locales de;locales ja
lr-lastreplicatedby: sauviat@adobe.com
navTitle: Content design best practices
publishexternaldate: 2018-07-23T08 13 15.962-0400
publishExternalURL: https://helpx.adobe.com/campaign/standard/designing/using/content-design-best-practices.html
sha1: ce6012b532965738a146ee5f9733b448748aea9e
topicBrowsingSortDate: 2018-07-23T08:13:15.962-0400
index: y
internal: n
snippet: y
---

# Content design best practices

Content design best practices

To ensure the editor's optimal operation, we recommend observing the following guidelines:

* SCSS style sheets are not supported. Use regular CSS if you import ZIP files containing your HTML content.
* When editing **email content**:

  Preview your messages before sending them. Adobe Campaign offers a way to test email rendering using Litmus. For more on this, see [Email rendering](../../sending/using/email-rendering.md).

* When editing **landing page content**:

    * Before importing an HTML page template in Adobe Campaign, please make sure the template opens and displays correctly in the various browsers.
    * If the HTML page contains JavaScript scripts, they need to execute without errors outside of the editor. In general, avoid using scripts in message content to make sure it is correctly processed by email clients.
    * When building a template, we recommend adding a **'type'** attribute to  tags. This information will be processed by the editor and help the user to link a database field to the form field when configuring the web application.

      Example of HTML code in the template:

      ```    
      
      <input id="email" type="email" name="email"/>
         
      ```    
    
      The official list of 'type' attributes is available at the following address: [http://www.w3schools.com/tags/att_input_type.asp](http://www.w3schools.com/tags/att_input_type.asp)

More design and general best practices regarding messages are presented in the following Adobe Campaign step-by-step guide: [Delivery best practices with Adobe Campaign](https://docs.campaign.adobe.com/doc/standard/getting_started/en/ACS_DeliveryBestPractices.html ).