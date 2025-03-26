# 🚀 Email Classification and Data Extraction

## 📌 Table of Contents
- [Introduction](#introduction)
- [Demo](#demo)
- [Inspiration](#inspiration)
- [What It Does](#what-it-does)
- [How We Built It](#how-we-built-it)
- [Challenges We Faced](#challenges-we-faced)
- [How to Run](#how-to-run)
- [Tech Stack](#tech-stack)
- [Team](#team)

---

## 🎯 Introduction
Loan servicing teams manually process high-volume emails which are diverse requests and attachments. Manual triage is time-consuming and error-prone,
Need an AI-powered solution to automate classification & data extraction.

## 🎥 Demo
🔗 [Live Demo](#) (if applicable)  
📹 [Video Demo](#) (if applicable)  
🖼️ Screenshots:
![Image20250326133404](https://github.com/user-attachments/assets/773174b7-d4a3-4385-a2c4-06900ad51814)
![Image20250326133411](https://github.com/user-attachments/assets/8858414a-d4a0-43ee-8cad-b3110d749aab)

## 💡 Inspiration
What inspired you to create this project? Describe the problem you're solving.

## ⚙️ What It Does
Features

### Email Fetching
Email fetching is the process of connecting to an Internet Message Access Protocol (IMAP) server to retrieve the latest emails from a user's inbox. This involves establishing a secure connection to the server, authenticating the user’s credentials, and then querying the server for any new messages since the last fetch. The system efficiently downloads the most recent emails, allowing for timely processing and ensuring that users have access to the latest communications. This step is crucial for maintaining an up-to-date workflow and is typically performed at regular intervals or triggered by specific user actions.

### Email Classification
Email classification is a sophisticated process that utilizes a Large Language Model (LLM) to analyze the content of incoming emails in order to accurately determine their request type and sub-type. This involves parsing the text of the email, including subject lines and body content, to identify keywords, phrases, and context that signify the nature of the request. For example, the LLM may classify an email as a "support request," "billing inquiry," or "general query," and further categorize it into sub-types such as "technical issue" or "payment problem." This systematic classification is vital for routing requests to the correct teams and ensuring a prompt response.

### Data Extraction
Data extraction is the process of identifying and pulling out key details from the email content and any attached files. This may include extracting information such as names, dates, order numbers, and specific details relevant to the request. Advanced algorithms may also be employed to scan attachments—like PDFs or images—to extract text or data using Optical Character Recognition (OCR) technology. The extracted information is then structured and formatted for easy use in subsequent processes, such as logging requests or generating reports, which enhances overall efficiency and accuracy in handling inquiries.

### Multi-Request Handling
Multi-request handling refers to the system's capability to recognize and manage emails containing multiple requests from a single sender. This involves analyzing the content to identify both primary and secondary requests, allowing the system to address each issue appropriately. For instance, an email may contain a request for assistance with a product issue while also asking about shipping status. By effectively categorizing and prioritizing these requests, the system ensures that all issues are acknowledged and resolved without neglecting any, thereby improving customer satisfaction and operational effectiveness.

### Duplicate Email Detection
Duplicate email detection is a critical feature that helps prevent redundant service requests by identifying emails that are identical or nearly identical in content. The system employs algorithms to compare incoming emails against a database of previously processed requests. If a duplicate is detected, the system can flag it, consolidate the request, or inform the user that their inquiry has already been received. This not only streamlines the workflow by reducing unnecessary duplication of efforts but also enhances resource allocation and response times.

### Skill-Based Routing
Skill-based routing is an intelligent system feature that assigns incoming requests to the appropriate team or personnel based on the classification results. Once the email has been classified, the system evaluates the specific skills and expertise of available personnel to determine the best fit for addressing the request. This ensures that inquiries are handled by individuals who have the relevant experience and knowledge, leading to quicker resolutions and a more efficient handling of cases. By directing requests to the most qualified teams, organizations can improve service quality and customer satisfaction.

### Web-Based UI
The web-based user interface (UI) provides a simple and intuitive frontend that allows users to view and interact with the results of the email processing system. This interface displays the classified requests, extracted data, and any relevant metrics in a clear and organized manner. Users can easily navigate through their emails, view detailed information about each request, and track the status of responses. The UI is designed for ease of use, enabling both technical and non-technical users to efficiently manage their email requests and access insights without needing extensive training or technical knowledge. Additionally, the web-based nature of the UI ensures accessibility from any device with internet connectivity, promoting flexibility and convenience in communication management.

## 🛠️ How We Built It
Briefly outline the technologies, frameworks, and tools used in development.


## 🚧 Challenges We Faced
Describe the major technical or non-technical challenges your team encountered.

## 🏃 How to Run
1. Clone the repository  
   ```sh
   git clone https://github.com/your-repo.git
   ```
2. Install dependencies  
   ```sh
   npm install  # or pip install -r requirements.txt (for Python)
   ```
3. Run the project  
   ```sh
   npm start  # or python app.py
   ```
Installation & Setup

Prerequisites

Python 3.8+

OpenAI API Key

IMAP Email Access

Flask for the web UI

Installation

Clone the repository:

git clone https://github.com/ewfx/gaied-xtreme-thinkers.git
cd gaied-xtreme-thinkers

Install dependencies:

pip install -r requirements.txt

Configure the config.json file with your OpenAI API key and email credentials:

{
    "openai_api_key": "your-api-key",
    "email_host": "imap.example.com",
    "email_user": "your-email@example.com",
    "email_pass": "your-password",
    "openai_model": "gpt-4",
    "classification_prompt": "Classify the following email: {email_content}",
    "extraction_prompt": "Extract structured data from this email: {email_content}",
    "routing_map": { "Loan Adjustment": "Loan Processing Team" }
}

Running the Application

Option 1: Run with Shell Script (Linux/macOS)

chmod +x run.sh
./run.sh

Option 2: Run with Batch Script (Windows)

run.bat

Option 3: Manually Start Flask App

python app.py

Once running, access the UI at http://127.0.0.1:5000/.

Running Unit Tests

Navigate to the unit_tests directory:

cd unit_tests

Run all tests:

python -m unittest discover

Folder Structure

├── app.py               # Main application file
├── config.json          # Configuration file
├── templates/           # HTML files for web UI
│   ├── index.html
├── static/              # Static files (CSS, JS)
├── unit_tests/          # Unit test scripts
│   ├── test_email_fetch.py
│   ├── test_classification.py
│   ├── test_data_extraction.py
│   ├── test_routing.py
├── requirements.txt     # Python dependencies
├── run.sh               # Shell script to start app
├── run.bat              # Windows batch script to start app
├── README.md            # Project documentation

## 🏗️ Tech Stack
- 🔹 flask
- 🔹 imapclient
- 🔹 pdfplumber
- 🔹 Other: OpenAI API 
  
## 👥 Team
- **Your Name** - [GitHub](#) | [LinkedIn](#)
- **Teammate 2** - [GitHub](#) | [LinkedIn](#)
