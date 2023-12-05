# Product Recommendations

### Overview

The 'Product Recommendations' feature enables the agent to suggest product recommendations seamlessly within the conversation, drawing from the uploaded product data as needed. This can be used in sales or customer support scenarios, where the agent might need to recommend products based on the user's needs or preferences.

{% embed url="https://app.arcade.software/share/Hhcyitro2iQrUofV3jPy" %}

### **Data Cleaning Feature**

**Overview:** We've introduced the 'Smart Data Cleaning' feature to enhance the accuracy and efficiency of our product recommendation agent. It's not uncommon for CSV files to carry values that may not align with the expected data type. Our new feature ensures that such discrepancies are detected and rectified.

**Details:**

* **Number Format Rectification:** If a column contains values like '1,0', '2,0', and '3,5', the agent might read them as strings. Our smart cleaning detects this and converts them to the proper float format: '1.0', '2.0', '3.5', ensuring that mathematical operations can be performed on the column without hitches.
* **String + Number Simplification:** For values mixed with text, such as 'YEAR 2020', 'YEAR 2021', our feature smartly removes the non-numeric portion, leaving just the numeric values: '2020', '2021', '2022'. This simplifies data representation and enhances processing efficiency.

With this feature, users can expect a smoother, more intuitive data handling experience, ensuring that the product recommendation agent operates with optimal accuracy.
