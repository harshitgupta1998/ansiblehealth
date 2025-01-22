# Markdown to Google Docs Converter

This repository provides a Colab notebook that converts Markdown-based meeting notes into a well-formatted Google Doc. It handles:
- Creating a new Google Doc via the Google Docs API
- Applying the correct heading styles (H1, H2, H3)
- Maintaining nested bullet points (including checkboxes)
- Preserving `@mentions` in bold or color
- Adding footer information with distinct styling (italic, smaller font, gray color, etc.)

## Brief Description

The script reads Markdown content (either from a string variable or a `.md` file), parses headings, bullets, and checkboxes, then programmatically creates a new Google Doc. It updates text style using batch requests so that headings, bullets, mentions, and footers match the specified formats.

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/harshitgupta1998/ansiblehealth.git

2. **Enable Google Docs API**:
Go to your Google Cloud Console, create or select a project, and ensure the Google Docs API is enabled.

2. **Obtain Credentials**:
Create an OAuth 2.0 Client ID (Desktop or Web Application) in Google Cloud Console.

## Required Dependencies

The primary dependencies are:

re
markdown
google.colab 
googleapiclient.discovery
google.auth

##  How to run in Colab

1. Open Google Colab.
2. Upload the notebook file (convert_markdown_to_google_doc.ipynb) and your credentials.json file in the same Colab session.
3. Install the required libraries in a Colab cell:
4. !pip install google-api-python-client google-auth google-auth-oauthlib google-auth-httplib2 markdown
5. Authenticate by running the authentication cell (it will prompt you to sign in with your Google account).
6. Run all the cells in order.
7. Observe the output which includes a link to the newly created Google Doc.
  
