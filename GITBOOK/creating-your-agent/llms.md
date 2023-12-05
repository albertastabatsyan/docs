# LLMs

Fine-Tuner supports a variety of Language Model options, both proprietary Anthropic models and OpenAI models. This chapter will guide you on how to select a Language Model (LLM) for your AI agent and

### 1. Language Models Supported

#### Anthropic Models:

* claude-1.0
* claude-2.0

#### OpenAI Models:

* davinci-003
* gpt-3.5-turbo
* gpt-4
* gpt-3.5-turbo-0613
* gpt-4-0613
* gpt-3.5-turbo-16k

Different models offer different capabilities and trade-offs. For instance, Claude 2 is impressive with its focus on safety, ethics, and large context handling, while GPT-4 is strong in advanced reasoning.

### 2. Configuring Language Models

Fine-Tuner provides options for users to adjust the behavior of the chosen Language Model. One of these options is adjusting the "temperature".

* **Temperature**: This parameter controls the randomness of the model's responses. A higher temperature results in more diverse outputs, while a lower temperature makes the model's responses more deterministic and focused.

By default, users use Fine-Tuner's commercial API keys to access these models. However, if you have your own LLM API keys, you can include and use them in the API Keys tab in your portal. This offers more flexibility and control over the usage and billing of the language models.

When setting up your agent, ensure to select the most suitable language model and adjust the parameters based on your specific use case. The right configuration can significantly improve the performance and effectiveness of your AI agent.
