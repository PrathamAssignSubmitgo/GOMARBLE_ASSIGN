# Selenium-Gemini Workflow with Local LLM Integration
###https://drive.google.com/file/d/1NTzC2slz20pXu15x_p4HbFo3RDcMqV90/view?usp=drive_link
## Overview
This project began with a locally hosted LLM (Large Language Model) for automated data analysis and interaction. However, scaling the local setup was challenging. To address this, we transitioned to a more scalable solution using Selenium for web interaction and a custom LLM hosted on Gemini. This new approach streamlines web data extraction, processing, and analysis.
https://drive.google.com/file/d/1NTzC2slz20pXu15x_p4HbFo3RDcMqV90/view?usp=drive_link
## How It Works

### 1. Moving from Local to Cloud
Initially, a locally hosted LLM handled processing. While effective for small tasks, it struggled with resource demands. Switching to Gemini's cloud-hosted LLM brought:
- Automated code suggestions.
- HTML and CSS analysis.
- Smarter decisions for pagination and navigation.

### 2. Web Automation with Selenium
Selenium manages web interactions in a Debian environment by:
- Identifying essential elements like buttons, forms, and CSS.
- Analyzing page structures to determine optimal interaction methods.
![image](https://github.com/user-attachments/assets/923b3f10-d178-404c-8590-cf1d2078a2ab)

### 3. CSS and Pagination Management
The Gemini-powered LLM:
- Examines extracted CSS for better pagination strategies.
- Suggests button placements for smoother navigation.

The workflow dynamically selects the most relevant navigation elements to ensure accurate progression through paginated content.

### 4. Fetching Data During Transitions
When navigating between pages (e.g., Page 1 to Page 2):
- Comments and other data are fetched independently via APIs.
- This ensures data loads quickly and doesn’t delay page transitions.
![image](https://github.com/user-attachments/assets/33e53935-e27c-4015-beaf-8393d0a44c1f)

### 5. Cleaning and Exporting Data
Fetched data is:
- Cleaned and preprocessed.
- Exported into an Excel sheet for further analysis.
![image](https://github.com/user-attachments/assets/901cb6ac-fa83-4872-acea-322702d74a69)

### 6. Advanced Analysis with LLM
The Excel data is processed by the LLM to:
- Summarize key topics and trends from comments.
- Create detailed visualizations, such as:
  - **NetworkX graphs:** Highlighting relationships and connections.
  - **Neo4j graphs:** Offering deeper structural insights.
![image](https://github.com/user-attachments/assets/1e73df6a-729b-4513-977c-b2a575a07883)
![image](https://github.com/user-attachments/assets/b24c6b74-2175-4ff9-9171-4ffc6d082a00)

## Key Features
- **Seamless Automation:** Selenium handles web interaction and data extraction efficiently.
- **Smart Integration:** Gemini’s LLM analyzes HTML, CSS, and navigation strategies.
- **Dynamic Data Fetching:** Retrieves comments and content asynchronously during transitions.
- **Insightful Analysis:** Produces topic summaries and advanced visualizations.
- **Scalable Design:** Combines local automation with cloud-based intelligence for high performance.

## Requirements
- **Operating System:** Deb
