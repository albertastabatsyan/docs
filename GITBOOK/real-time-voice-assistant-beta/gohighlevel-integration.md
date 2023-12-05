---
description: How to Deploy Voice Assistants on GoHighLevel
---

# GoHighLevel Integration

## Video

{% embed url="https://www.veed.io/view/f4e95700-467a-4295-9a7f-65564edc1a58?panel=share" %}
How to integrate GHL
{% endembed %}

**Marketplace Link:** [https://marketplace.gohighlevel.com/integration/653bee8ab4783e721f7b1348](https://marketplace.gohighlevel.com/integration/653bee8ab4783e721f7b1348)\
\
**Notes**

* The Synthflow App can be used for Agency and Subaccount

### **Prerequisites**:

* An active subscription with Synthflow.ai is required.
  * Register at [synthflow.ai/ghl](https://synthflow.ai/ghl).
* Generate an API-Key within your Synthflow.ai dashboard.

#### Preparing Your Assistants in Synthflow.ai

* **For Inbound Calls:** You must have an Inbound Assistant configured in Synthflow.ai.
* **For Outbound Calls:** You must set up an Outbound Workflow Assistant in Synthflow.ai.



Successfully integrating Synthflow.ai for both inbound and outbound calls within your GoHighLevel account involves creating two specific workflows: one for making calls and another for retrieving transcripts.

### Workflow #1: Make the Call

To initiate calls via Synthflow.ai, create the first workflow automation in GHL.

<figure><img src="../.gitbook/assets/screely-1701703232113.png" alt=""><figcaption></figcaption></figure>

1.  **Create a Workflow Trigger:**

    * Select <mark style="background-color:orange;">“Contact Tag”</mark> as your trigger.
    * Apply filters and choose <mark style="background-color:orange;">"call"</mark>&#x20;

    <div align="left">

    <figure><img src="../.gitbook/assets/screely-1701703598116 (1).png" alt="" width="375"><figcaption><p>Contact Tag Trigger</p></figcaption></figure>

    </div>
2.  **Configure the Call Action:**

    * Add a <mark style="background-color:orange;">"Make A Phone Call"</mark> action and select Synthflow.ai - AI Phone Assistant

    <div align="left">

    <figure><img src="../.gitbook/assets/screely-1701703870147.png" alt="" width="375"><figcaption></figcaption></figure>

    </div>

    * Enter the Model ID, which can be found in the Synthflow.ai app under the "More info" section.

    <div align="left">

    <figure><img src="../.gitbook/assets/screely-1701703973756.png" alt="" width="375"><figcaption><p>Model ID - Synthflow.ai App</p></figcaption></figure>

    </div>

    * Set the contact's phone number and first name fields:
      * Phone: Use the contact’s raw format phone number.
      * Name: Input the contact’s first name.
    * Insert your Synthflow.ai API key, which is available under the API tab in the Synthflow.ai app.

    <div align="left">

    <figure><img src="../.gitbook/assets/screely-1701704163511.png" alt="" width="563"><figcaption><p>API key - Synthflow.ai App</p></figcaption></figure>

    </div>

    * Map the 'lead\_name' to the contact's first name for personalization.

### Workflow #2: Retrieving the Call Transcript

To capture the call transcript, proceed with the following workflow.

<figure><img src="../.gitbook/assets/screely-1701704378089.png" alt=""><figcaption><p>Workflow 2 - Example</p></figcaption></figure>

1.  **Set Up an Inbound Webhook Trigger:**

    * Copy the provided webhook URL (POST/GET/PUT)

    <div align="left">

    <figure><img src="../.gitbook/assets/screely-1701704509588.png" alt="" width="375"><figcaption><p>COPY URL(POST/GET/PUT)</p></figcaption></figure>

    </div>

    * Paste this URL into the Synthflow.ai web app under your Assistant’s Deployment settings for GHL, and initialize.

    <div align="left">

    <figure><img src="../.gitbook/assets/screely-1701704614045 (1).png" alt="" width="563"><figcaption><p>PASTE URL - Synthflow.ai App</p></figcaption></figure>

    </div>

    * Select the <mark style="background-color:orange;">MAPPING REFERENCE</mark> dropdown and pick any sample request
2.  **Add Create or Update Contact Action:**

    * Use the "Create/Update Contact" action to log the phone number from the Inbound Webhook.

    <div align="left">

    <figure><img src="../.gitbook/assets/screely-1701704799664.png" alt="" width="375"><figcaption><p>CREATE UPDATE CONTACT - Phone_number</p></figcaption></figure>

    </div>
3.  **Add a Notes Action:**

    * Utilize the "Notes" action to record the call transcript, duration, and status by clicking <mark style="background-color:orange;">Custom Values > Inbound Webhook Trigger > Transcript/Duration/Status</mark>

    <div align="left">

    <figure><img src="../.gitbook/assets/screely-1701704949664.png" alt="" width="375"><figcaption><p>Notes Action</p></figcaption></figure>

    </div>

#### ! Important: Always Keep Allow re-entry enabled

<figure><img src="../.gitbook/assets/screely-1701705092860.png" alt=""><figcaption></figcaption></figure>
