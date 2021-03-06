[< back](../Lab2.md#The-Plan-for-the-Day)

# Lab 2.1: Getting started with Cognitive Services
Duration: 1 - 1.5 hours

[![Generic badge](https://img.shields.io/badge/STATUS-DRAFT-ORANGE.svg)](https://shields.io/)

This session introduces you to to working with pre-trained models from the Azure Cognitive Services, and enables you to explore their capabilities.
<!---
<img src=https://docs.microsoft.com/en-us/learn/achievements/data-ai/classify-and-moderate-text-with-azure-content-moderator.svg/>
<img src=https://docs.microsoft.com/en-us/learn/achievements/data-ai/create-and-publish-a-luis-model.svg>
<img src=https://docs.microsoft.com/en-us/learn/achievements/classify-user-feedback-with-the-text-analytics-api.svg>

-->
## 1. Explore the Azure Cognitive Services with the Intelligent Kiosk


**Option 1**: Install the pre-compiled Intelligent Kiosk App

[![Generic badge](https://img.shields.io/badge/mode-no_code-BLUE.svg)](https://shields.io/)

The pre-compiled Kiosk is great for an initial look. This version uses some preconfigured API keys so you can get going straight away.

Step 1: Download the Kiosk app from the Microsoft App Store here: https://www.microsoft.com/en-gb/p/intelligent-kiosk/9nblggh5qd84


Step 2: Launch the application - you should arraive at a 'Demo Gallery'. Find the Translator API Panel, to load the Translator Explorer.

<img src='img/kiosk_overview.jpg' />

Then follow this guide to explore the capabilities of the Translator explorer.

https://github.com/microsoft/Cognitive-Samples-IntelligentKiosk/blob/master/Documentation/TranslatorExplorer.md

*Note: If you speak another language, note some of the subtleties when using OCR: for example, an erroneous recognition of the word 'oceanic' as 'occanic' in this picture results in a best-guess german translation of 'okkanisch'.*

<img src='./img/OCR.jpg' />

<!-- **Option 2**: Run the Kiosk locally with Visual Studio

[![Generic badge](https://img.shields.io/badge/mode-no_code-BLUE.svg)](https://shields.io/)

Step 0: Install Visual Studio

Step 1: Clone the following repo to your machine:

https://github.com/Microsoft/Cognitive-Samples-IntelligentKiosk

Step 2: Follow the guidance on [this](https://github.com/Microsoft/Cognitive-Samples-IntelligentKiosk#Running-the-sample) page to load the Kiosk solution into Visual Studio 


Next: This local version does not have any preconfigured API connections [TODO - verify this!], so please move on to 2. below to provision your own.
-->


## 2. Provision your own Cognitive Services instances

In this section, we will show you how to obtain your own API keys for cognitive services with your subscription. 

> 💡 **Hint:** You may already have done this if you worked through the pre-requisite learning material in your own subscription.

You can connect these to your Kiosk, or explore below other ways of interacting with these service instances.

**Option 1:** Use the Azure portal - an example

[![Generic badge](https://img.shields.io/badge/mode-no_code-BLUE.svg)](https://shields.io/)

Here, we'll use the Azure portal to obtain your own API key for the Cognitive Services that you will also be working with this afternoon.


1. Create a Speech Resource

    https://docs.microsoft.com/en-gb/learn/modules/convert-speech-to-text/3-subscribe-to-speech-translation-api
2. View subscription keys and endpoints

    https://docs.microsoft.com/en-gb/learn/modules/convert-speech-to-text/4-viewing-access-keys-and-endpoints


**Option 2:** Set up all required services with an azure-cli script 

[![Generic badge](https://img.shields.io/badge/mode-azure_cli-TEAL.svg)](https://shields.io/)

If you have worked with the azure-cli before, the following script provisions an instance of the cognitive services required by the Intelligent Kiosk, and returns your API keys.

https://github.com/microsoft/Cognitive-Samples-IntelligentKiosk/blob/master/KeyAcquisitionScript.md

> 💡 **Tip:** For users already familiar with Azure, this is a good opportunity to familiarise yourself with template-driven provisioning of resources - review the script and try to make some changes.

## 3. Connect to your Cognitive Service

### To connect Kiosk application to your own service instances

[![Generic badge](https://img.shields.io/badge/language-no_code-BLUE.svg)](https://shields.io/)

Add your API keys to the 'settings' page of the Kiosk application.

Click on <img src='./img/settings.jpg' height=40px /> in the bottom left corner of the Kiosk application.

Under Cognitive Services Keys, set `Shared Keys` to off, and enter your API keys in the relevant fields.

<img src='./img/custom_keys.jpg' width=60%/>


## 4. Explore some of the [documented scenarios](https://github.com/Microsoft/Cognitive-Samples-IntelligentKiosk#Scenarios) 

Use any remaining time to explore some of the [documented scenarios](https://github.com/Microsoft/Cognitive-Samples-IntelligentKiosk#Scenarios) in your Kiosk application, and prepare a few notes as to what appears relevant to your business and what this exercise has inspired you to explore further.
We will do a quick round-table in the debrief at the end of the day, so that we can use this to tailor the follow on technical workshops.

<hr>

## Give Session Feedback
> 💬 Please fill out the session feedback: http://bit.ly/AI4GFeedback 💬

<hr>


## Go Further
#### To interact with your cognitive services with python

[![Generic badge](https://img.shields.io/badge/language-python-YELLOW.svg)](https://shields.io/)

For those of you with python skills, here is some sample code to help you learn how to interact with cognitive services with python.

You need to have provisioned your own services to do this - see for example step 2 above. (Note some of this will be easier once you have done the afternoon sessions)
- https://github.com/caiomsouza/Microsoft-Cognitive-Services
- https://github.com/caiomsouza/Microsoft-Cognitive-Services/tree/master/textanalytics


<pre>


</pre>

[next >](../Lab2.md#The-Plan-for-the-Day)