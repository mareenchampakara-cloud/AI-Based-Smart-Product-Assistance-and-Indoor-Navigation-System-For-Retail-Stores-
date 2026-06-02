<div align="center">

<img src="https://www.sju.edu.in/assets/img/st-joseph-university-logo.png" height="80" style="background:white; padding:8px; margin:0 16px;" />
<img src="https://www.erafoundationindia.org/images/logo.svg" height="80" style="background:white; padding:8px; margin:0 16px;" />
<img src="https://comedkares.org/wp-content/uploads/2023/04/Comedkares-Logo-EPS.png" height="80" style="background:white; padding:8px; margin:0 16px;" />

</div>

---

# AI-Based-Smart-Product-Assistance-and-Indoor-Navigation-System-For-Retail-Stores

<div align="center">
  
**Rovan John, MSc BDA, 252BDA42· Mareen Biju George, MSc BDA, 252BDA21· A Carton Britto, MCA, 253MCA64.G Jeshwanth, MCA, 253MCA02·Shaik Mohammad Farhanulla Sami, MCA, 253MCA52·**

</div>

---
## Abstract

The retail industry is rapidly adopting Artificial Intelligence (AI) technologies to improve customer experience and operational efficiency. This project proposes an AI-Based Smart Product Assistance System that utilizes Large Language Models (LLMs), Conversational Recommender Systems (CRS), and Product Recognition technologies to assist customers in retail stores. The system provides personalized product recommendations, answers customer queries, understands shopping preferences, and offers real-time product information through natural language conversations. By integrating recommendation algorithms, conversational AI, and inventory-aware product databases, the proposed system aims to create an intelligent shopping assistant that enhances customer satisfaction and simplifies decision-making. The solution is designed for both physical retail stores and digital commerce environments.
---


## Keywords

Artificial Intelligence, Large Language Models, Conversational Recommender Systems, Product Recommendation, Retail Automation, Natural Language Processing, Customer Assistance, Explainable AI, Smart Retail, Personalization.

---

## 1. Introduction

The modern retail industry is undergoing a significant transformation driven by Artificial Intelligence and data-driven decision-making. Customers increasingly expect personalized shopping experiences, intelligent recommendations, and instant access to product information. Traditional recommendation systems often fail to provide interactive and context-aware assistance, limiting their ability to understand customer preferences effectively.

Large Language Models (LLMs) and Conversational Recommender Systems (CRS) offer new opportunities to improve customer engagement by enabling natural and personalized interactions. These systems can understand customer needs, provide product suggestions, answer questions, and explain recommendations in a human-like manner.


---

## 2. Literature Review

The literature review focuses on five major research papers related to conversational recommendation systems, retail AI, and large language models.

Paper 1

Smart Customer Service in Unmanned Retail Store Enhanced by Large Language Model

This study demonstrates how AI-powered customer service can be integrated into retail stores using SKU recognition and LLMs. The system improves customer interaction and product recommendation capabilities.

Paper 2

Leveraging Large Language Models in Conversational Recommender Systems

The paper explores the integration of LLMs with conversational recommendation engines to improve dialogue management, recommendation accuracy, and customer engagement.

Paper 3

Advances and Challenges in Conversational Recommender Systems: A Survey

This survey presents various conversational recommendation architectures, highlighting challenges such as preference elicitation, dialogue generation, and recommendation explainability.

Paper 4

Conversational Recommender System and Large Language Model Are Made for Each Other in E-Commerce Pre-sales Dialogue

The research explains how LLMs can improve recommendation quality in e-commerce environments through interactive customer conversations.

Paper 5

Towards Personalized Conversational Sales Agents

The study introduces contextual user profiling techniques that help AI sales assistants provide personalized and persuasive product recommendations.

---

## 3. Problem Statement


Traditional retail recommendation systems often provide generic product suggestions and lack the ability to understand customer needs through natural conversations. Customers frequently face difficulties in finding suitable products, comparing alternatives, and making informed purchasing decisions, which can lead to a less efficient shopping experience. Furthermore, many existing systems do not provide personalized recommendations, explain the reasons behind their suggestions, or consider real-time product availability. Therefore, there is a need for an intelligent product assistance system that can understand customer preferences, provide personalized and explainable recommendations, and offer real-time conversational support. The proposed AI-Based Smart Product Assistance System addresses these challenges by integrating Large Language Models (LLMs), Conversational Recommender Systems (CRS), and recommendation algorithms to enhance customer experience and improve decision-making in retail environments.

---

## 4. Objectives

1)Develop an AI-powered smart product assistant for retail stores.
2)Provide personalized product recommendations using customer preferences.
3)Enable natural language interaction through Large Language Models.
4)Improve customer decision-making through explainable recommendations.
5)Integrate inventory-aware product recommendation mechanisms.
6)Enhance overall customer shopping experience.


---

## 5. Methodology


The proposed AI-Based Smart Product Assistance System follows a multi-stage architecture that combines Natural Language Processing (NLP), Large Language Models (LLMs), Conversational Recommender Systems (CRS), and Explainable Artificial Intelligence (XAI) to provide personalized product recommendations and customer assistance in retail stores.

## 5.1 System Architecture

The system consists of the following modules:

1. User Interaction Module
2. Natural Language Processing Module
3. User Preference Extraction Module
4. Product Knowledge Base
5. Recommendation Engine
6. Large Language Model Module
7. Explainable AI Module
8. Response Generation Module


## 5.2 Data Collection

The product dataset is collected from retail inventory databases and contains:

| Attribute               | Description                   |
| ----------------------- | ----------------------------- |
| Product ID              | Unique identifier             |
| Product Name            | Product title                 |
| Category                | Product classification        |
| Brand                   | Manufacturer                  |
| Price                   | Product cost                  |
| Nutritional Information | Calories, Protein, Fat, Sugar |
| Customer Ratings        | User reviews                  |
| Product Description     | Detailed information          |

The collected data is stored in a structured MySQL database.

---

## 5.3 Data Preprocessing

Before recommendation generation, the dataset undergoes preprocessing.

### Step 1: Data Cleaning

Tasks performed:

* Remove duplicate records
* Handle missing values
* Correct inconsistent product names
* Standardize categories

### Step 2: Feature Engineering

New features are generated:

* Price Range
* Health Score
* Popularity Score
* Recommendation Weight

### Step 3: Text Processing

Product descriptions are processed using NLP techniques:

* Tokenization
* Stop Word Removal
* Lemmatization
* TF-IDF Vectorization

The processed text is later used by recommendation models.

---

## 5.4 User Query Processing

The user enters a query through text or voice.

Example:

"I need a healthy breakfast under ₹300."

The NLP module extracts:

### Intent

Intent = Product Recommendation

### Entities

Budget = ₹300

Category = Breakfast

Preference = Healthy

### User Constraints

* Low Sugar
* High Protein
* Affordable

The extracted information is passed to the recommendation engine.

---

## 5.5 Conversational AI Module

The Conversational AI Module is powered by a Large Language Model.

Functions include:

### Query Understanding

Understanding customer needs through natural language.

### Context Management

Maintaining conversation history.

Example:

Customer:
"I want a healthy breakfast."

System:
"Do you prefer vegetarian or non-vegetarian options?"

### Preference Refinement

The chatbot asks follow-up questions to improve recommendation quality.

---

## 5.6 User Profiling Module

The system creates a dynamic user profile using:

### Explicit Preferences

Collected directly from users:

* Budget
* Dietary Preferences
* Favorite Brands
* Product Categories

### Implicit Preferences

Learned automatically:

* Purchase History
* Search History
* Click Behavior
* Frequently Recommended Products

The profile is continuously updated after every interaction.

---

## 5.7 Recommendation Engine

A Hybrid Recommendation Model is implemented.

### Content-Based Filtering

Products are recommended based on similarity.

Features considered:

* Category
* Price
* Nutrition
* Brand

Similarity is calculated using:

Cosine Similarity

between user preferences and product features.

### Collaborative Filtering

Recommendations are generated based on similar users.

Methods:

* User-Based Filtering
* Item-Based Filtering



---

## 5.8 Large Language Model Integration

The Large Language Model is responsible for:

* Product explanation
* Customer assistance
* Follow-up questioning
* Natural language recommendation

Example:

Instead of displaying:

"Product A"

The LLM generates:

"I recommend Kellogg's Oats because it is rich in fiber, supports digestion, and fits within your budget."

This improves customer trust and understanding.

---

## 5.9 Explainable AI Module

Explainability is integrated into every recommendation.

The system explains:

* Why the product was recommended
* Which preferences were considered
* Price comparison
* Health benefits

Example:

Recommendation Reason:

* Matches breakfast category
* Under ₹300 budget
* High protein content
* Highly rated by similar users

---

## 5.10 Inventory-Aware Recommendation

Before displaying products, the system checks inventory status.

Conditions:

If Stock > 0
→ Product Recommended

If Stock = 0
→ Alternative Product Recommended

This prevents recommending unavailable products.

---

## 5.11 Response Generation

The final recommendation is generated using:

Recommendation Results + LLM Explanation + Inventory Status

Output Example:

Recommended Products:

1. Kellogg's Oats
2. Yogabar Muesli
3. Quaker Oats

Reason:

These products match your healthy breakfast preference, are available in stock, and fall within your ₹300 budget.

---

## 5.12 Model Evaluation

The recommendation system is evaluated using:

### Precision

Measures recommendation relevance.

### Recall

Measures recommendation coverage.

### F1 Score

Balances precision and recall.

### Accuracy

Measures overall recommendation correctness.

### User Satisfaction Score

Collected through user feedback surveys.

### Response Time

Measures recommendation generation speed.

---

## 5.13 Deployment

The final system is deployed using:

Frontend:

* React.js

Backend:

* FastAPI

Database:

* MySQL

AI Models:

* Llama 3 / GPT API

Cloud Platform:

* AWS / Azure

The deployed system can be accessed through a web application and integrated into retail store environments.

## 6. Implementation


The AI-Based Smart Product Assistance System was developed using a combination of web technologies, recommendation algorithms, and Large Language Models (LLMs) to provide intelligent product recommendations and customer assistance.

## 6.1 Frontend Development

The user interface was developed using React.js, providing customers with an interactive platform to search products, ask queries, and receive personalized recommendations through a chatbot interface.

## 6.2 Backend Development

The backend was implemented using Python and FastAPI. It handles user requests, processes customer queries, communicates with the recommendation engine, and generates responses using the AI model.

## 6.3 Database Management

A MySQL database was used to store product information, inventory details, customer preferences, and recommendation history. The database enables efficient retrieval of product data and real-time stock availability.

## 6.4 Recommendation Engine

A hybrid recommendation approach combining Content-Based Filtering and Collaborative Filtering was implemented. The system analyzes customer preferences, product features, and user behavior to generate personalized recommendations.

## 6.5 Large Language Model Integration

A Large Language Model (LLM) was integrated to understand customer queries, maintain conversational context, and provide human-like responses. The model also generates explanations for product recommendations.

## 6.6 Inventory-Aware Assistance

Before displaying recommendations, the system verifies product availability from the inventory database. If a product is out of stock, suitable alternatives are suggested automatically.

## 6.7 System Workflow

The customer enters a query through the chatbot interface. The NLP module extracts preferences and requirements, which are processed by the recommendation engine. The selected products are validated against inventory data and passed to the LLM, which generates personalized explanations before displaying the final recommendations to the customer.

## 6.8 Deployment

The application can be deployed on cloud platforms such as AWS or Azure. The system is accessible through web browsers and can be integrated into retail store environments to provide real-time customer assistance.


---

## 7. Results & Analysis


The AI-Based Smart Product Assistance System successfully provides personalized product recommendations based on customer preferences, budget, and product requirements. The integration of Large Language Models (LLMs) enables natural language interaction and improves customer engagement through conversational assistance.

The hybrid recommendation engine generates relevant product suggestions by analyzing product features and user preferences. Additionally, the inventory-aware module ensures that only available products are recommended, improving recommendation reliability.

| Feature                   | Result                                  |
| ------------------------- | --------------------------------------- |
| Query Understanding       | Accurate extraction of user preferences |
| Product Recommendation    | Personalized suggestions                |
| Conversational Assistance | Natural and interactive responses       |
| Inventory Awareness       | Real-time stock verification            |
| Customer Experience       | Improved shopping assistance            |

Overall, the proposed system enhances the retail shopping experience by combining AI-driven recommendations, conversational interaction, and explainable product suggestions.

---

## 8. Discussion


The proposed AI-Based Smart Product Assistance System demonstrates how Large Language Models (LLMs) and Conversational Recommender Systems (CRS) can improve customer experience in retail environments. By understanding customer queries and preferences, the system provides personalized product recommendations and meaningful explanations.

Unlike traditional recommendation systems, the proposed solution enables natural conversations, real-time assistance, and inventory-aware recommendations. This helps customers make informed purchasing decisions while reducing the time required to search for products.

The integration of conversational AI, recommendation algorithms, and product information creates a more interactive and intelligent shopping experience. The system also has the potential to support future enhancements such as voice-based interaction, product image recognition, and multilingual assistance.

---

## 9. Conclusion


The AI-Based Smart Product Assistance System demonstrates the potential of combining Large Language Models (LLMs) and Conversational Recommender Systems (CRS) to enhance customer experience in retail stores. The system provides personalized product recommendations, understands customer preferences, and delivers intelligent conversational assistance.

By integrating recommendation algorithms, inventory-aware product suggestions, and explainable AI, the proposed solution improves product discovery and supports better purchasing decisions. Overall, the system offers an efficient, interactive, and customer-centric approach to modern retail shopping.

---

## 10. Future Scope



The AI-Based Smart Product Assistance System has significant potential for future enhancements. One possible improvement is the integration of voice-based interaction, allowing customers to communicate with the system using natural speech for a more convenient shopping experience. Multilingual support can also be incorporated to assist customers from different linguistic backgrounds.

The system can be enhanced with computer vision techniques such as barcode scanning and product image recognition, enabling customers to obtain product information by simply scanning or capturing images. Integration with real-time inventory management systems would ensure that recommendations are always based on current stock availability.

Future versions may also utilize customer purchase history, browsing behavior, and feedback data to provide highly personalized recommendations. Mobile application deployment and indoor store navigation features can further improve customer convenience by helping shoppers quickly locate recommended products within the store.

Additionally, advanced analytics and machine learning models can be employed to predict customer preferences, identify shopping trends, and support business decision-making. These enhancements will contribute to creating a more intelligent, efficient, and customer-centric retail shopping environment.

---

## Acknowledgements


We would like to express our sincere gratitude to our faculty members for their valuable guidance, encouragement, and continuous support throughout the development of this project.

We also extend our thanks to **Mr. Adithya, Assistant Manager, Namdhari Agro Fresh Pvt. Ltd.**, for providing valuable industry insights and helping us understand the practical challenges and requirements of retail store operations. His suggestions played an important role in shaping the direction of this project.

We are grateful to our institution for providing the necessary resources and learning environment to carry out this research successfully. Finally, we would like to thank all team members for their dedication, teamwork, and contributions towards the successful completion of the **AI-Based Smart Product Assistance System** project.


---

## References


[1] Y. Wang, X. Zhang, J. Li, and H. Chen, “Smart Customer Service in Unmanned Retail Store Enhanced by Large Language Model,” *Scientific Reports*, vol. 14, no. 1, 2024. DOI: 10.1038/S41598-024-71089-9.

[2] H. Gao, Z. Liu, and Y. Chen, “Leveraging Large Language Models in Conversational Recommender Systems,” *Proceedings of the ACM Conference on Recommender Systems (RecSys)*, 2024.

[3] Z. Lei, Y. Zhang, and T. Chen, “Advances and Challenges in Conversational Recommender Systems: A Survey,” *AI Open*, vol. 2, pp. 100–126, 2021. DOI: 10.1016/j.aiopen.2021.06.002.

[4] J. Wang, K. Zhou, and Y. Li, “Conversational Recommender System and Large Language Model Are Made for Each Other in E-commerce Pre-sales Dialogue,” *Findings of the Association for Computational Linguistics: EMNLP 2023*, pp. 9588–9604, 2023. DOI: 10.18653/v1/2023.findings-emnlp.643.

[5] S. Kumar, A. Sharma, and R. Patel, “Towards Personalized Conversational Sales Agents: Contextual User Profiling for Strategic Action,” *Findings of the Association for Computational Linguistics: EMNLP 2025*, 2025. DOI: 10.18653/v1/2025.findings-emnlp.275.

[6] I. Goodfellow, Y. Bengio, and A. Courville, *Deep Learning*. Cambridge, MA: MIT Press, 2016.

[7] S. Russell and P. Norvig, *Artificial Intelligence: A Modern Approach*, 4th ed. Pearson, 2021.

[8] J. Leskovec, A. Rajaraman, and J. Ullman, *Mining of Massive Datasets*, 3rd ed. Cambridge University Press, 2020.

[9] T. Mikolov, K. Chen, G. Corrado, and J. Dean, “Efficient Estimation of Word Representations in Vector Space,” 2013.

[10] A. Vaswani et al., “Attention Is All You Need,” *Advances in Neural Information Processing Systems (NeurIPS)*, 2017.
