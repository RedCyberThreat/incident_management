AI-Powered Incident Management Assistant
This project demonstrates how to leverage Local Large Language Models (LLMs) via Ollama to automate common cybersecurity analyst tasks. The notebook contains three specialized modules for log analysis, incident classification, and report generation.

Features
Basic Log Analysis: Automatically scans raw log data (like IP addresses and login attempts) to identify suspicious patterns.

Incident Severity Classification: Uses AI to evaluate security incidents and categorize them as Low, Medium, or High severity based on system impact.

Automated Report Generator: Transforms raw incident data into a structured report including Summary, Impact, Actions Taken, and Recommendations.

Prerequisites
Since this script runs locally for data privacy, you need to have the Ollama runtime installed on your machine.

Install Ollama: Download it from ollama.com.

Pull the Model: This project uses the llama3 model. Run the following command in your terminal:

Bash
ollama pull llama3
Python Dependencies: Ensure you have the ollama Python library installed:

Bash
pip install ollama
How to Use
Clone the Repository:

Bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
Run the Notebook:

Open Incident Management.ipynb in VS Code, Jupyter Lab, or upload it back to Google Colab.

If using Colab, ensure you have a tunnel or a local runtime connected to your Ollama instance.

Execute Cells: Run the cells sequentially. The script will communicate with your local Ollama server to process the cybersecurity prompts.

Code Overview
The script utilizes the ollama.chat API to interact with the Llama 3 model. It uses System Prompts to define the AI's persona as a Cybersecurity Analyst, ensuring the output remains professional and technically accurate.

Example Input:

"User downloaded unknown executable and system behavior changed."

Example AI Output:

Severity: High
Reasoning: The execution of unknown binaries combined with behavioral changes suggests a potential malware infection or system compromise...

Security Note
This tool is intended for educational and assistant purposes. Always verify AI-generated analysis with manual investigation before taking remediation actions in a production environment.

How to add this to your GitHub:
On GitHub, click Add file > Create new file.

Name it README.md.

Paste the text above into the editor.

Click Commit changes.
