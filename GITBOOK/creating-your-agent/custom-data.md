# Custom Data

The Fine-Tuner platform allows users to upload and utilize custom data to enhance the performance and contextual understanding of their AI agents. This chapter will guide you on how to upload data, the different sources you can use, and how the data is utilized by the agents.



### 1. Understanding Custom Data Usage

The agents in Fine-Tuner can use the uploaded data as a context during their operation. Essentially, this data is used to train the agents. This allows them to have a better understanding of the domain they will be working in, be it sales, customer support, or any other use case.

You can either upload new data or assign an already existing dataset (which already has data in it) to the agent. Note that one dataset can be assigned to multiple agents, so you can reuse your data effectively across multiple scenarios.

Furthermore, the specific sources and pages/rows of the context data used by the agent can be retrieved through the agent inference endpoint of the API. This allows you to track exactly which parts of your data the agent is utilizing and provides greater transparency into the agent's operation.

### 2. Uploading Custom Data

#### Step 1: Name the Data Source

You can give your data source a name to recall and find it easier in the future. Make sure to use a descriptive and intuitive name, especially if you plan to work with multiple data sources.

#### Step 2: Select Data Loader

Depending on the source and format of your data, you can select one of the following options to load your data into Fine-Tuner:

* **File**: Upload a PDF, CSV, PowerPoint, or Word document directly.
* **Text**: Copy and paste your content directly into the loader.
* **URL**: Load text from a webpage using the URL.
* **Crawler**: Loads multiple URLs from the root website URL. Useful for larger data collection tasks.
* **Twitter**: Load tweets with your Twitter handle.
* **Notion**: Load content from your Notion pages.

#### Step 3: Upload the Data

Once you have named your data source and selected the data loader, proceed to upload the data from the selected source.

Remember that the uploaded data serves as the knowledge base for your AI agent, so make sure to use relevant and high-quality data. The better the data you provide, the better your agent will perform.
