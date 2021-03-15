---
description: Create forms
---

# JotForm

Updated: Mar. 2, 2021

![](https://lh6.googleusercontent.com/hKped11JQn9HnVnVKXJXGT0sd33Rv4of2_pTslIMgP-l115v1kP-xPHmBOa0plM_7AZS0a1X-gbMzdOhYFZqSqj-z5Jy54uSmVQzGsAobu1Jg3LzMb9scusYCVIYqzZ3uH2MKHGx)

\*\*\*\*[**https://www.jotform.com**](https://www.jotform.com)\*\*\*\*

**Note:** This is a living document. [Share your comments and experience to improve it](https://form.jotform.com/210477511316045).

## Author

[Alex Allain](mailto:alex@usdigitalresponse.org), USDR Staff

## Description <a id="h.7w7zez36b1wy"></a>

‌A highly configurable drag and drop form builder with light programmable capabilities.

## Tags

* 🌈  No-code
* 🎁  Free
* 💸  Freemium
* 💰 Paid
* 🥁 Trial
* \*\*\*\*🗝 **USDR account** - [Request access](https://airtable.com/shrgI6dxsMqWbwId5)
* ♿  Accessible \([enable accessibility checks](https://www.jotform.com/help/592-how-can-i-make-my-forms-accessible)\)
* 🌐  Supports multiple languages \([details](https://www.jotform.com/help/298-how-to-make-your-forms-multilingual)\)

## Category <a id="h.275oysyrlu3w"></a>

* Data
* data/productivity
* Design
* Forms
* Services

## ‌Procurement <a id="h.go61rzbnc73"></a>

‌JotForm has both free and paid tiers. The most expensive plan is $79/month but is overkill for all but the most heavyweight use cases. The $29/month plan supports 10,000 form submissions and is sufficient in almost all cases. See [https://www.jotform.com/pricing](https://www.google.com/url?q=https://www.jotform.com/pricing&sa=D&source=editors&ust=1612994048910000&usg=AOvVaw3TVfX8yWa4Qu1MWPiMr3Vr) for details.

## Alternative / Similar Tools <a id="h.ru44st8agyw1"></a>

‌Alternative tools a project lead could look at to compare:

* ‌Cognito Forms
* Airtable Forms
* TypeForm
* forms.microsoft.com
* &lt;probably others&gt;

What sets JotForm apart from Google Forms, Microsoft Forms and Airtable Forms is that it is much more customizable. You have more control over the types of inputs, the flow between form elements, and the UI. For example, with Microsoft Forms, you cannot create a form that accepts uploads from anyone on the  internet, control whether individual questions are hidden/displayed or prevent the form from being submitted. 

JotForm also includes features like esignatures and a [gallery of widgets](https://www.jotform.com/widgets) that can be used to customize inputs. This flexibility makes JotForm a good option even when it's not immediately needed, as it provides more options when requirements change.

## ‌Integration With Other Tools

This tool integrates well with the following tools:

* [Slack](https://www.jotform.com/help/563-how-to-use-slack-with-your-form)
* [Zapier](https://zapier.com/apps/jotform/help)
* [Power Automate](https://www.jotform.com/blog/microsoft-flow-integration/) \(requires a Premium Power Automate license\)
* [AirTable](https://www.jotform.com/help/561-how-to-integrate-jotform-with-airtable)
* [OneDrive](https://www.jotform.com/blog/announcing-onedrive-integration)

Integration with Power Automate is straightforward for basic use cases. However, if access to uploaded files is required, it is significantly more complicated and multiple steps are required. This [webpage](https://www.jotform.com/answers/2358500-how-to-upload-the-files-in-a-submission-to-sharepoint-through-power-automate) describes approximately how to do it. It requires changing form access settings, then using the HTTP connector. This is a multi-step process as the URLs provided by JotForm 301 to the final file destination, so multiple HTTP connector steps are needed. 

This tool does NOT integrate well with the following tools:

* 🔴SharePoint - connecting JotForm to SharePoint requires using Power Automate, so while it is possible to do so, it requires an extra tool that must be monitored. If you need to move files from JotForm to SharePoint, you have to deal with the hurdles mentioned above.
  * Note: if you can replace SharePoint in the workflow with OneDrive, your life should be considerably easier now that JotForm has a OneDrive integration.
* 🔴Power Automate - we have also run into issues with using Power Automate and JotForm together. Sometimes the data from JotForm is not populated in the Power Automate trigger - see this [support ticket](https://www.jotform.com/answers/2125992-problem-with-the-integration-with-microsoft-flow-power-automate) for an example. At this point, I would _not_ recommend starting a new project where Power Automate is used with JotForm. 

## Vendor Support <a id="h.e50orjda7y75"></a>

I’ve never actually needed  to contact their support. There is a pretty rich amount of information available via Google as they have many forum posts. They appear to be quite responsive in that setting.

## Maintenance <a id="h.o456lrtyv134"></a>

JotForm requires very little maintenance. While we have seen them experience the occasional outage, there’s not a great deal you need to do unless your form hits one of the paid plan limits.

### Monitoring <a id="h.mkbsvjvtwwdv"></a>

JotForm can generally just be left on its own without hitting any issues, as long as you don’t hit one of the paid plan limits.

## Security Level

Forms can be encrypted at rest and some plans have PCI and HIPAA compliance. More details at https://www.jotform.com/security/

{% hint style="danger" %}
The security level is: **PRIVATE / HIGH SECURITY** - Information related to the USDR volunteers or government partners that, if disclosed, may lead to legal or regulatory repercussions including securities violations and mandated data breach reporting. May contain personal data with other related legal or regulatory privacy requirements or obligations. Improper or unauthorized collection, use, disclosure, retention, or disposal may pose some risk to the data subject.
{% endhint %}

## How I've Used This Tool <a id="h.flwakkvuwzba"></a>

* To import a PDF and use JotForm to fill out the PDF \(and then use Power Automate to link that PDF to SharePoint\). Here's [an example using Bexar County's poll worker application](https://form.jotform.com/202521613393044) to fill in a PDF.  Here's a [Vote-by-Mail demo app](https://form.jotform.com/202688090585060) that fills in a PDF.
* To build a number of wizard/screener flows that don’t actually anticipate a form being submitted at all, but instead use JotForm’s programmatic capabilities. Here's a generic example that shows a [wizard for helping someone ensure they are ready to vote](https://form.jotform.com/202405673455151).
* To build a number of longer, multi-page intake forms.
* JotForm has many plugins, including the ability to do scheduling and take payment information, but I have not used those.

## Lessons Learned <a id="h.9j1dk9qzdv6e"></a>

**PROCEED!** What this tool is great for ... almost any basic form task -- JotForm is quite good.

1. JotForm is a great tool to prototype any Form or Form-like flow to show what is possible to a government partner. Often, building a form is expected to be hard, but JotForm makes it easy. JotForm also makes it look good. Customizing JotForm to have the look-and-feel of our partners is pretty easy, and can make for a really quick win when creating a demo.
2. It is very easy to build a JotForm for a partner and then transfer the form to them by cloning the form through the “Create Form\|Import Form” workflow, so you don’t need to have access to their JotForm account just to build the form.
3. The “one question at a time” flow is very good for wizards/screeners.
4. JotForm makes it easy to integrate with AirTable \(and has more powerful form functionality - particularly the programmability - than AirTable\) as well as other tools, so it is a good module in a larger suite of SaaS tools.
5. JotForm has the ability to import a PDF, and then produce a filled version of that PDF. This can be a good way to quickly digitize the intake process for workflows that are currently paper based.
6. JotForm can accept file uploads. If someone fills out the form on a phone, that widget allows them to take a photo.

**BEWARE!** What's hard to do with this tool ...

1. It is more difficult to build wizards/screening questions in the single page version of the form - but this is generally solvable by using the one-question-at-a-time process.
2. JotForm may not be a good tool if your partner already has access to a different form builder - e.g., Cognito Forms.
3. JotForm may not be a good fit if you only need to build simple forms. FOr example., if you are using a product like AirTable \(or GSuite\) that has its own forms and they are good enough for what you need to do. JotForm introduces another procurement hurdle and another tool to integrate. That being said, JotForm’s user experience is also nice, so even in those cases, you find it is a good choice.
4. JotForm &lt;-&gt; SharePoint is not as easy as some other tool integrations.
5. JotForm's Power Automate integration has known issues as outlined above.



## Other Landmines

1. Uploading files to JotForm via Power Automate is very tedious and challenging.
2. Emails sent from JotForm may be subject to attachment size limits, so if you are relying on emails to route uploaded documents, be careful that the size never exceeds 5MB.
3. The classic form view \("all questions on one page"\) does not make it possible \(from what I can tell\) to prevent submitting a form. The card form view \("show single question per page"\) view does. If you're used to building wizards with the latter view, this can be frustrating if you want to create a regular form that prevents submission.
4. JotForm allows you to hide fields manually, and also set conditional logic to hide and show fields. If you have conditional logic that controls which fields are displayed, they operate as constraints, not procedural statements. I.e. if you say "if A, show field", then if A is false, the field is hidden. This will override any default settings of whether the field is hidden or not. Moreover, if you have multiple conditions that control the visibility of the same field, and they conflict, you will get very confusing results.

## Training Resources <a id="h.jjhr8ylgtcxa"></a>

JotForm UI is pretty intuitive and most questions can be answered by googling.

## Hmm, What Else? <a id="h.citc7idtx8n3"></a>

‌In my opinion, JotForm is the go to form builder for USDR at the moment. While there might be better tools out there that we should consider, of all the form builders we’ve used, I think it’s the best.

## Share your experience with this tool

Would you like to add additional information from your experience to help others vet or use this tool? [Share your comments here](https://form.jotform.com/210477511316045).

## Was this helpful? 

Please rate the information in this page with a🙂😐☹at the bottom of the page to help us improve it. 

