# Automated Data Intake & Cleansing Pipeline

A no-code automation workflow built with Make.com that intercepts inbound form data, automatically strips raw HTML formatting, and logs clean, structured data into a Google Sheets database.

##  Architecture & Workflow
<img width="917" height="410" alt="image" src="https://github.com/user-attachments/assets/1a11eff7-dd64-486f-996d-d38de2c5273a" />


**Modules Used:**
* Google Forms (Trigger)
* HTML to Text (Data Transformation)
* Google Sheets (Data Storage)

##  How It Works
1. **Trigger:** A user submits a response via a Google Form containing raw HTML text.
2. **Transformation:** The Make.com HTML module intercepts the payload and parses the raw HTML tags (`<p>`, `<strong>`, etc.) into clean, readable plain text.
3. **Action:** The clean text is mapped and appended as a new row in a centralized Google Sheets database.

##  Business Value
* Eliminates manual data entry and formatting errors.
* Ensures downstream databases receive clean, standardized text.
* Reduces administrative time spent cleaning raw web data.

##  How to Import
1. Log in to your [Make.com](https://www.make.com/) account.
2. Create a new Scenario.
3. Click the menu (three dots) in the top right -> **Import blueprint**.
4. Upload the `blueprint.json` file from this repository.
5. Re-authenticate your Google account connections and map your specific Google Sheet columns.
