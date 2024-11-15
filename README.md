# mangiproject
A custom query LLM based interpreter that takes csv file or google sheet link as input and provides web scraped data as requested by query in new csv with processed results in new column


BreakoutAI

Project Description  
BreakoutAI is a powerful tool designed to automate data processing and information retrieval. It integrates seamlessly with Google Sheets and CSV files, allowing users to input data, run SEO-optimized queries, extract targeted information, and save the results efficiently.  

---

Setup Instructions  

Step 0: Clone the Repository and Install Requirements  
1. Clone the repository:  
   ```
   git clone https://github.com/MadGod29/BreakoutAI.git  
   cd BreakoutAI  
   ```  
2. Install the required dependencies:  
   ```
   pip install -r requirements.txt  
   ```  

Step 1: Set Up Google Cloud for Sheets API  
1. Open the Google Cloud Console (https://console.cloud.google.com/).  
2. Create a new project.  
3. Enable the Google Sheets API for your project.  
4. Create credentials:  
   - Select Service Account.  
   - Skip the rest of the setup steps.  
5. Open the Credentials section, create a new key in JSON format, and download it.  
6. Save the JSON file in the root of the cloned repository.  

Step 2: Prepare the `.env` File  
1. Create a `.env` file in the root of the repository.  
2. Add the following environment variables:  
   ```
   SERP_API_KEY=your_serp_api_key  
   TOGETHER_API_KEY=your_together_api_key  
   CREDENTIALS_PATH=path/to/your/credentials.json  
   ```  
   - SERP_API_KEY: Sign up on SERP API (https://serpapi.com/) to get your API key.  
   - TOGETHER_API_KEY: Sign up on Together API (https://togetherapi.com/) to get your API key.  
   - CREDENTIALS_PATH: The path to the Google Sheets credentials JSON file downloaded in Step 1.  

Step 3: Run the Application  
Start the Streamlit application:  
```
streamlit run app.py  
```  

---

Usage Guide  

1. Load Data  
   - Upload a CSV file or provide a Google Sheets URL.  
2. Customize Query  
   - Select the column containing names/identifiers and customize the search query template.  
3. Process Data  
   - Click Start Processing to run the queries and extract information.  
4. Save Results  
   - Save the results as a CSV file or back to a Google Sheet.  

---

API Keys and Environment Variables  

- SERP_API_KEY: Required for search queries.  
- TOGETHER_API_KEY: Needed for advanced functionalities.  
- CREDENTIALS_PATH: Google Sheets API credentials in JSON format.  

---

Follow these instructions carefully to set up and use BreakoutAI. If you encounter any issues, feel free to raise an issue in the GitHub repository.  


