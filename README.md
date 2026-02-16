🤖 Business Reporting Automation with AI (LLM)
📌 Project Overview

This project demonstrates how Large Language Models (LLMs) can support a Data Analyst in automatically generating business insights and strategic recommendations based on aggregated sales data.

The analysis was conducted using a public dataset containing global video game sales data (source: Kaggle).

The project focuses on practical AI integration into the reporting workflow rather than pure model development.

🎯 Business Problem

Companies operating globally (e.g., game publishers, digital product companies) must regularly analyze:

sales trends

platform and product performance

regional differences

Manual preparation of analytical reports and strategic conclusions is time-consuming and difficult to scale.

This project explores how AI can assist in accelerating this process.

🧠 Project Objectives

Prepare structured sales data for business analysis

Automatically generate business insights using AI (LLM)

Demonstrate how AI can accelerate reporting and decision-making processes

🛠 Scope of Work
1️⃣ Data Preparation & Analysis (Python)

Data loading and cleaning (handling missing values in the Year column)

Sales aggregation:

Global time trends

Platform performance

Genre performance

Publisher performance

Regional sales (NA, EU, JP, Other)

2️⃣ Data Aggregation for AI

Instead of passing raw data to the LLM, structured business summaries were prepared, including:

Total global sales

Top platforms

Top genres

Top publishers

Regional sales comparison

Recent sales trends

The structured output was saved as:

ai_input_summary.json


This ensures that the AI receives clean, contextualized, and business-ready input.

3️⃣ AI-Based Business Analysis (LLM)

The aggregated data was provided to the language model together with business context.

The AI generated:

Key business insights

Potential risks

Strategic recommendations for future product releases

🤖 Role of AI in the Project

In this project, AI acts as a virtual business analyst that:

Interprets numerical data

Identifies patterns and trends

Supports strategic decision-making

The project demonstrates practical use of prompt engineering in data analysis workflows.

📈 Results

Simulated reduction in reporting preparation time

Clear, structured business insights in text format

AI-generated insights validated against Power BI dashboards

The project illustrates how AI can complement traditional BI tools rather than replace them.

🧰 Tech Stack

Python (pandas, numpy, matplotlib, seaborn)

Jupyter Notebook

AI / LLM (text analysis, prompt engineering)

JSON

Markdown

📁 Repository Structure
video-game-sales-ai/
│
├── data/
│   └── vgsales.csv
│
├── notebooks/
│   └── 01_data_analysis.ipynb
│
├── output/
│   ├── ai_input_summary.json
│   └── ai_business_report.md
│ 
├── prompts/
│   └── ai_prompt.md
│
└── README.md

🚀 Possible Extensions

Integration with Power BI dashboards

Automated recurring reporting (e.g., monthly updates)

Deployment as an internal reporting assistant

👩‍💻 Author

Created as part of a Data Analyst / AI-focused portfolio project, demonstrating practical AI integration in business analytics.
