## 🚀 Company Brochure Generator – AI-Powered Web Scraping & Summarization  

### 📌 Overview  
This Jupyter Notebook automates the process of generating a company brochure using **OpenAI’s API** and **web scraping**. It extracts key details from a company’s website, including landing page content and relevant links, and then crafts a concise, well-structured brochure in **Markdown format**.  

### 🎯 Features  
✅ **Automated Web Scraping** – Extracts relevant text from a company’s landing page and linked pages.  
✅ **AI-Powered Summarization** – Uses OpenAI to process and condense the extracted information into a compelling brochure.  
✅ **Dynamic Link Filtering** – Filters out irrelevant links (e.g., Terms of Service, Privacy Policy).  
✅ **Markdown Output** – Generates a brochure in a clean, readable format.  

### 🔧 How It Works  
1. **Extract Links**: `get_links(url)` retrieves relevant links using OpenAI.  
2. **Fetch Page Content**: `get_all_details(url)` scrapes content from the main page and linked pages.  
3. **Generate Brochure**: `create_brochure(company_name, url)` structures the content into a formatted markdown brochure.  

### 🛠 Setup Instructions  
1. Install dependencies:  
   ```bash
   pip install openai beautifulsoup4 markdown
   ```
2. Ensure you have an OpenAI API key and set it in your environment.  
3. Run the notebook and call:  
   ```python
   create_brochure("Company Name", "https://companywebsite.com")
   ```

### 🐞 Troubleshooting  
- If you encounter a **KeyError: 'links'**, ensure `get_links(url)` correctly formats its output as `{ "links": [...] }`.  
- Some sites may block automated scrapers; consider adding headers to mimic a real browser request.  

### 📜 License  
This project is for educational and research purposes. Use responsibly.  

💡 **Contribute & Improve**: Feel free to modify the notebook to enhance link filtering and improve AI responses! 🚀
