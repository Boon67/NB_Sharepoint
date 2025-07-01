# SharePoint File Manager Notebook

This Snowflake notebook provides a user interface for managing SharePoint files directly from Snowflake using Streamlit.

## Features

* Connect to SharePoint using site URL and credentials
* Browse files in the default document library
* Download selected files to local storage
* Secure access through Snowflakes network rules and external access integration

## Prerequisites

* Access to a Snowflake account with appropriate permissions
* SharePoint site URL and valid credentials
* Required Python packages:
  - streamlit
  - office365-runtime
  - office365-sharepoint

## Setup

The notebook consists of two main components:

1. **Network Configuration (SQL)**
   * Creates network rules for SharePoint domains
   * Sets up external access integration for secure communication
2. **User Interface (Python)**
   * Provides a Streamlit-based interface for:
     - SharePoint authentication
     - File browsing
     - File downloading

## Usage

1. Enter your SharePoint site URL
2. Provide your username (email)
3. Enter your password
4. Click "Connect" to authenticate
5. Select a file from the displayed list
6. Click "Download Selected File" to save the file locally

## Security Notes

* Credentials are handled securely through Streamlits password input
* Network access is restricted to SharePoint domains
* External access integration ensures secure communication
