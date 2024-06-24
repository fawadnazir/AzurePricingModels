**Customer Friendly Azure OpenAI Cost Estimator for RAG-based Contact Center Agents Usecase**

This Python script empowers you to estimate the monthly cost of utilizing Azure OpenAI and Azure AI Search within a Retrieval-Augmented Generation (RAG) based contact center agent use case. It facilitates modeling a scenario where a large language model assists human agents in efficiently handling customer inquiries.

**Key Functionalities:**

- Calculates costs for various Azure OpenAI models (GPT-3.5, GPT-4) with diverse capabilities.
- Considers storage tier selection for optimal Azure AI Search configuration.
- Integrates agent activity metrics, including average query length and interaction duration.
- Applies a configurable Azure discount to the estimated cost for potential savings.
- Provides a detailed breakdown of cost components for Azure Search (storage + ranking) and Azure OpenAI (input + output tokens).
- Scales the cost estimation to encompass multiple similar use cases for comprehensive financial planning.


**Usage Instructions:**

1. Clone or download the repository.
2. Within the script, locate the section designated [410] # ------------------------------ # Parameters to adjust the model # ------------------------------. Update the following parameters to reflect your specific use case:
- Number of use cases
- Number of contact center agents
- Average time and number of queries per customer interaction
- Average word count in agent queries and responses
- Working hours and days per month
- Azure discount (optional)
- Storage tier and Azure OpenAI model selection
3. Execute the script. It will generate estimated costs for a single use case and the scaled cost for the specified number of use cases, both with and without the discount applied.

**References:**
- Azure OpenAI: https://azure.microsoft.com/en-us/products/ai-services/openai-service
- Azure AI Search: https://learn.microsoft.com/en-us/training/modules/intro-to-azure-search/
- RAG Model: https://learn.microsoft.com/en-us/azure/search/retrieval-augmented-generation-overview
- Azure Pricing Calculator: https://azure.microsoft.com/en-gb/pricing/calculator/

**Important Considerations:**

- This script utilizes pricing data from the Australian East Region. Prices may vary depending on your chosen region.
- The script assumes a 1.34 tokens per word ratio, which may differ based on the specifics of your use case.

By leveraging this script, you can gain valuable insights into the potential cost implications of implementing a RAG-based contact center agent solution with Azure services. This information can empower you to make informed decisions during the planning and budgeting stages of your project.
