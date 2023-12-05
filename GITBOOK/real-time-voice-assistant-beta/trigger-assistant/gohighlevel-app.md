---
description: Installation Instructions
---

# GoHighLevel App

{% embed url="https://share.vidyard.com/watch/ys71aae7QEHUJh6zURHNKL" %}

Synthflow.ai has launched their official app on the GoHighLevel Marketplace, streamlining voice integration for both agency and subaccount use.\
\
\
**Marketplace Link:** [https://marketplace.gohighlevel.com/integration/653bee8ab4783e721f7b1348](https://marketplace.gohighlevel.com/integration/653bee8ab4783e721f7b1348)\
\
**Notes**

* The Synthflow App can be used for Agency and Subaccount

**Prerequisites**:

* An active subscription with Synthflow.ai is required.
  * Register at [voice.synthflow.ai](https://voice.synthflow.ai).
* Create a Trigger Agent and acquire the Model-Id on the Synthflow.ai dashboard.
* Generate an API-Key within your Synthflow.ai dashboard.

### Installation Instruction <a href="#installation-instruction" id="installation-instruction"></a>

1. Log into your GoHighLevel account.
2. Navigate to the "App Marketplace" located on the right-hand side.
3. Search for `Synthflow.ai` and proceed with the installation of the app.
4. Within Workflows, create a new workflow or edit an existing one.
5. Add a trigger that suits your use case.
6. Choose the "Make A Phone Call" action.
   1. Add the Model-Id from your Agent which you can obtain in the Synthflow.ai Dashboard
   2. Provide a Phone Number and Name for the call.
   3. Add the API-Key from your Agent which you can obtain in the Synthflow.ai Dashbaord
   4. Optional: Add Key/Value pairs which can be used to dynamically popluate the agent prompt that you have set in the Synthflow.ai Dashboard
7. Insert a "Wait" action to delay the webhook from receiving the call transcription until the call concludes, recommended delay is 10 minutes.
8. Add a "Custom Webhook" Action
   1. Select "POST" as Event
   2. Add following link to the URL field: [https://ai-finetune.bubbleapps.io/api/1.1/wf/wh\_voice\_agent\_ghl](https://ai-finetune.bubbleapps.io/api/1.1/wf/wh\_voice\_agent\_ghl)​
   3. Add a Query Param: Key: call\_id Value: \{{phonecall.1.response.call\_id\}}
   4. Add following code as the body

```json
{
  "id": "1698430018599x83XXXXXXXXXX",
  "name": "David",
  "phone_number": "+1818738984",
  "duration": "",
  "status": "",
  "transcript": "",
  "error": ""
}
```

9. Save your workflow and conduct a test to ensure functionality.



**Example Flow**

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>



<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>



<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

​

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
