# Lead-Generator-Bot-n8n-Automation-Project-_Google-Maps-Scrapper
A no-code automation workflow built in n8n that collects business leads from Google Maps based on user input, filters duplicates, and stores structured data in Google Sheets. Designed to simplify lead generation with seamless data extraction, transformation, and storage.

# 🧠 Lead Generator Bot (n8n Automation Project)

### Author: **Mohammad Nehal**  
### Institution: **IIM Ranchi**  
### Date: **November 2025**

---

## 📋 Overview

The **Lead Generator Bot** is a no-code automation project built using **n8n**.  
It automatically collects business leads (e.g., *“Eye Hospitals in Churchgate”*) from Google Maps, processes the data, and appends structured lead information to a **Google Sheet**.

This workflow demonstrates how to integrate **data scraping**, **data cleaning**, and **cloud storage** seamlessly using n8n.

---

## ⚙️ High-Level Design

The system consists of four main components:

1. 🧾 **User Form** — collects the search query input (e.g., “Eye Hospitals in Mumbai”).  
2. 🌐 **HTTP Request Node** — fetches business details from a Google Maps scraping API.  
3. 🧩 **Split & Filter Nodes** — process and clean the data, removing duplicates and invalid entries.  
4. 📊 **Google Sheets Integration** — appends validated leads into a structured sheet for analysis.


---

## 🧱 Low-Level Workflow Design

### Step-by-Step:
1. **Form Trigger:** Starts the workflow when a user submits a search term.  
2. **HTTP Request:** Calls an API endpoint (Google Maps scraper) to fetch lead data.  
3. **Split Out:** Breaks JSON arrays into individual items for processing.  
4. **Filter:** Ensures only valid and unique entries are retained.  
5. **Append Row:** Saves the clean data to a connected Google Sheet.

---

## 🧩 Workflow Screenshots

| Workflow | Form Input | Google Sheet Output |
|-----------|-------------|----------------------|


*(Replace with actual image paths if you rename your screenshots folder.)*

---

## 📊 Results

The workflow produces a clean, structured list of business leads that includes:
- **Name**
- **Address**
- **Place**
- **State**
- **Phone**
- **Email**
- **Website**
- **Source URL**

Example output (Google Sheets):

| Name | Place | Phone | Website |
|------|--------|--------|---------|
| Shroff Eye Clinic | Mumbai | 918850104077 | https://www.shroffeye.org/ |
| Eyeris Eye Clinic | Mumbai | 919372475889 | http://www.eyeriscenter.com/ |

---

## ⚠️ Challenges Faced

During development, several issues were encountered:

- **Google API Authentication:** Setting up OAuth credentials correctly.  
- **API Rate Limits:** The scraping API sometimes limited requests.  
- **Data Normalization:** Ensuring consistent address and contact formats.  
- **Duplicate Entries:** Preventing repeated data when re-running workflows.  

These challenges were resolved using **filter logic**, **delay nodes**, and **validation checks** in n8n.

---

## ✅ Conclusion

The **Lead Generator Bot** automates lead generation efficiently using **n8n** and **Google Sheets**.  
It eliminates manual data collection, ensuring accuracy and scalability.  
The workflow can be easily adapted for other domains (e.g., restaurants, schools, real estate).

---

## 🚀 Future Improvements

- Add email or WhatsApp automation for outreach.  
- Integrate a CRM (e.g., HubSpot or Airtable).  
- Deploy using a local n8n instance for unlimited usage.

---

## 🧑‍💻 Technologies Used

- **n8n (No-code automation)**
- **Google Sheets API**
- **HTTP Request Node**
- **Data Filtering & Transformation**

---

## 📜 License

This project is open-sourced under the **MIT License**.

---

> Created by **Mohammad Nehal**, IIM Ranchi  
> For educational and demonstration purposes.

**Architecture Flow:**

