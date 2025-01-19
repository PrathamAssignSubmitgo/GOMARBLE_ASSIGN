# GOMARBLE_ASSIGN

README: Selenium-Gemini Workflow with Local LLM Integration

Overview

This project initially began with the use of a locally hosted LLM (Large Language Model) for automated data analysis and interaction. However, hosting and scaling the LLM locally presented challenges, leading to the development of a more robust workflow leveraging Selenium for web interaction and a custom LLM hosted on Gemini. This approach improves scalability and automates complex web data extraction, processing, and analysis tasks.

Workflow Description

1. Initial Setup

The project initially relied on a locally hosted LLM for processing. While effective for small-scale tasks, issues with hosting resources and accessibility prompted a shift to a cloud-based solution. Now, Gemini powers the LLM, enabling:

Automated code generation.

Analysis of HTML structures and CSS.

Dynamic decision-making for pagination and navigation.

2. Web Interaction Using Selenium

Selenium is used to interact with web pages running on a Debian environment. The workflow involves:

Identifying the critical HTML elements, including buttons, forms, and CSS styles.

Extracting and analyzing page structures for optimal interaction strategies.

3. CSS and Pagination Handling

The Gemini-powered LLM evaluates the extracted CSS and provides solutions for:

Pagination.

Placement of necessary elements for seamless navigation.

The workflow dynamically selects the most appropriate button for navigation, ensuring accurate traversal through paginated content.

4. Transition Management and Data Fetching

During page transitions (e.g., from Page 1 to Page 2):

Comments and related data are fetched independently through APIs.

This asynchronous fetching ensures data is displayed as soon as the page loads.

5. Data Cleaning and Export

Once the comments are fetched, the following steps are performed:

Cleaning and preprocessing of comment data.

Exporting cleaned data to an Excel sheet for further analysis.

6. LLM-Based Analysis

The exported Excel sheet is processed by the LLM to:

Provide a general overview of the comments, identifying key topics and trends.

Generate detailed visualizations, including:

NetworkX graphs for understanding relationships and interactions.

Neo4j graphs for deeper insights into data structure and connectivity.

Features

Selenium Automation: Seamlessly handles web interactions, extracting critical data with precision.

Gemini Integration: Custom LLM provides context-aware decision-making and analysis.

Dynamic Data Fetching: Independently retrieves comments and other content during page transitions.

Advanced Data Analysis: Generates insights and visualizations using network analysis tools.

Scalable Architecture: Combines local automation with cloud-based intelligence for a robust solution.

System Requirements

Operating System: Debian-based environment.

Software:

Selenium WebDriver.

Gemini (for LLM integration).

Python libraries: pandas, NetworkX, Neo4j, etc.

APIs: Endpoint for fetching comments and related data.

Usage Instructions

Setup:

Install required dependencies (Selenium, Python libraries, Gemini integration setup).

Configure API endpoints for data fetching.

Run Workflow:

Execute the Selenium script to start web interaction.

Monitor Gemini LLM outputs for structure analysis and navigation suggestions.

Data Processing:

Allow the workflow to fetch and clean comment data.

Export results to an Excel sheet.

Analysis:

Load the Excel sheet into the LLM for summary and topic analysis.

Generate NetworkX and Neo4j graphs for visualizing relationships.
