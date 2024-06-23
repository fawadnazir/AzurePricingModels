Title: Azure OpenAI Cost Estimator for RAG-based Contact Center Agents UseCase

Description:

This Python script estimates the monthly cost of using Azure OpenAI and Azure AI Search for a Retrieval-Augmented Generation (RAG) based contact center agent use case. It helps you model a scenario where a large language model assists human agents in handling customer queries.

Features:

Calculates costs for various Azure OpenAI models (GPT-3.5, GPT-4) with different capabilities.
Considers storage tier selection for Azure AI Search.
Factors in agent activity, including average query length and interaction time.
Applies a configurable Azure discount to the estimated cost.
Provides a breakdown of costs for Azure Search (storage+ranking) and Azure OpenAI (input+output tokens).
Scales the cost estimation for multiple similar use cases.
How to Use:

Clone or download the repository.
Update the following parameters in the script ([410] # ------------------------------ # Parameters to adjust the model # ------------------------------ section):
Number of use cases
Number of contact center agents
Average time and number of queries per customer interaction
Average words in agent queries and responses
Working hours and days per month
Azure discount (optional)
Storage tier and Azure OpenAI model
Run the script. The script will print the estimated costs for a single use case and the scaled cost for the specified number of use cases with and without the discount applied.
References:

Azure OpenAI: https://azure.microsoft.com/en-us/products/ai-services/openai-service
Azure AI Search: https://learn.microsoft.com/en-us/azure/search/
RAG Model: https://learn.microsoft.com/en-us/azure/ai-studio/concepts/retrieval-augmented-generation
Azure Pricing Calculator: https://azure.microsoft.com/en-gb/pricing/calculator/
Note:

This script uses pricing data for the Australian East Region. Prices may vary depending on the region.
The script assumes a 1.34 tokens per word ratio, which may differ based on your use case.
