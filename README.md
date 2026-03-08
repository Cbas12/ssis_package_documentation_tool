# SSIS Package Documentation Tool 🚀

[Castellano / Spanish](https://github.com/Cbas12/ssis_package_documentation_tool/blob/main/README.es.md)

This tool automates the process of documenting SQL Server Integration Services (SSIS) packages (.dtsx files). By combining Python's parsing capabilities with Generative AI, it extracts the internal logic, control flows, and data transformations to generate comprehensive, human-readable documentation.

## 🚀 Key Features
- **Automated Parsing:** Extracts metadata, SQL queries, and task logic directly from the XML structure of .dtsx files.
- **AI-Driven Analysis:** Uses Large Language Models (LLMs) to explain complex transformations and business logic in plain language.
- **Markdown Output:** Generates clean, structured documentation ready to be hosted on GitHub, GitLab, or internal Wikis.
- **Efficiency:** Reduces documentation time for legacy or complex ETL processes.

## 💰 Cost Efficiency
This tool is designed for multiple file processing at a small cost. During development and testing:
- **Scalability:** Successfully documented **30+ Stored Procedures**.
- **Total Cost:** Less than **$2.50 USD** (using Gemini API).
- **Value:** High-speed documentation at a fraction of the cost of manual labor or enterprise tools.

## 🛠️ Tech Stack
- **Language:** Python
- **AI Orchestration:** Google Gemini API
- **Main libraries:** lxml for XML parsing, google-generativeai for documentation

## 📋 Prerequisites
Before running the notebook, ensure you have:
- Python 3.10+
- A Google AI (Gemini) API Key.

## ⚙️ Configuration
1. **Clone the repository:**
    git clone https://github.com/Cbas12/ssis_package_documentation_tool.git

2. **Setup Credentials:**
    - Use the file gemini.txt to write down your own Gemini API Key. Simply copy the text inside.

## 📖 Usage
1. Open *ssis_package_documentation_tool_ENG.ipynb* in VS Code or Jupyter.
2. Ensure you added the input and output paths:
    - *ssis_location:* The folder path containing your dtsx, param and conmgr files.
    - *temp_output:* The folder where the tool will temporally save the summaries of the param and conmgr files to be used in combination with the clean dtsx files.
    - *docutentation_output_location:* The folder where you want the documentation files to be saved.
3. It's  suggested that, in the beginning of the section *"PROCESS THE FILES"* you reduce the number of files processeced at first, just to ensure everything goes accordingly to your expectations.
4. Run all cells. The tool will process each file and generate a detailed natural language explanation for each DTSX.

## 📄 License
This project is open-source. Feel free to clone, download, and adapt it to your own data workflows.