# API Keys

API keys are used to authenticate and grant access to various functionalities within Fine-Tuner. They act as a secure bridge between your applications, third-party tools, and the Fine-Tuner platform.

### 1. Fine-Tuner Key

The Fine-Tuner Key is your primary API key used to authenticate your access to Fine-Tuner's API. It <mark style="color:orange;">**enables interaction with Fine-Tuner's REST API endpoints, Widgets and Plugins**</mark>. This key is available on all paid plans.&#x20;

{% content-ref url="../deployment/synthflow-ai-api-key.md" %}
[synthflow-ai-api-key.md](../deployment/synthflow-ai-api-key.md)
{% endcontent-ref %}

### 2. LLM Keys

LLM Keys are specific to the Language Models you are utilizing within Fine-Tuner. You have the option to use your own OpenAI & Anthropic API keys or the default Fine-Tuner commercial key. Here's how to manage you LLM Keys:

1. **Go to the 'LLM Keys' Tab**: In the API Keys section, select the 'LLM Keys' tab.
2. **Add or Manage Keys**: If you opt to use your own keys, you can add new keys for different Language Models or manage existing ones here.
3. **Integration**: Use these keys to integrate specific Language Models with your AI agents or other applications.

Choosing to use your own LLM API keys provides greater autonomy and potential cost control. If you prefer the convenience of a ready-to-use solution, Fine-Tuner's commercial key is provided as the default option, allowing you to start building your agents without any extra configuration.

Remember that these keys, whether Fine-Tuner's or your own, are associated with specific models and must be managed carefully. Always adhere to best practices for key management to ensure the security and functionality of your integrations.

<figure><img src="../.gitbook/assets/Screenshot 2023-08-07 145811.png" alt=""><figcaption></figcaption></figure>

### 3. Third-Party Keys

Fine-Tuner allows integration with various third-party tools, and this is where you'll manage the keys for those integrations:

1. **Select the 'Third-Party Keys' Tab**: In the API Keys section, go to the 'Third-Party Keys' tab.
2. **Add or Edit Keys**: You can add new keys for different third-party services or edit existing ones.
3. **Follow Integration Guidelines**: Ensure you are following the integration guidelines provided by the third-party service. Each service may have unique requirements.
