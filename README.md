
# 🕷️ AI-Powered Web Scraper with Local LLaMA

This project is an **AI-enhanced web scraper** built with Python that can extract structured data from any website based on natural language prompts. It combines **Selenium** for scraping, **BeautifulSoup** for cleaning HTML, and **LangChain + Ollama** to run **open-source LLaMA models locally**, giving you powerful data extraction capabilities without using paid APIs like OpenAI.

---

## 🚀 Features

- 🌐 Scrape any website (even dynamic ones rendered with JavaScript)
- 🛡️ Bypass captchas and IP bans using Bright Data's remote browser
- 🧹 Clean and filter the HTML using BeautifulSoup
- 🧠 Use local LLaMA models (via Ollama) to extract specific data based on user prompts
- 📄 Chunk content automatically to fit within LLM token limits
- 🖥️ Streamlit-based user interface

---

## 📸 Demo

<img src="https://github.com/your-username/AI-Web-Scraper/assets/demo-screenshot.png" width="600"/>

---

## 🔧 How It Works

1. **User enters a URL** in the Streamlit interface.
2. The app uses **Selenium** with **Bright Data's scraping browser** to load and capture the website.
3. The HTML is cleaned using **BeautifulSoup** to remove scripts, styles, and noise.
4. Cleaned content is split into manageable chunks.
5. Each chunk is passed to a **locally running LLaMA model** using **LangChain** and **Ollama**.
6. The AI parses the content based on the user’s prompt and returns the result.

---

## 🧪 Example Prompts

- `List all product names and prices.`
- `Summarize the content of this page.`
- `Extract all links to property listings.`

---

## 📦 Installation

### 1. Clone the repo

```bash
git clone https://github.com/your-username/AI-Web-Scraper.git
cd AI-Web-Scraper


### 2. Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set up `.env` file

Create a `.env` file in the root directory and add your Bright Data WebDriver URL:

```env
SBR_WEBDRIVER=https://brd.superproxy.io:9222/session/YOUR_SESSION_ID
```

### 5. Install and run Ollama (LLaMA)

Download and install [Ollama](https://ollama.com/) on your system and run the LLaMA model locally:

```bash
ollama run llama3
```

---

## ▶️ Running the App

Once everything is set up, launch the Streamlit app:

```bash
streamlit run main.py
```

---

## 📁 Project Structure

```
AI-Web-Scraper/
├── main.py             # Streamlit UI
├── scrape.py           # Web scraping logic
├── parse.py            # AI parsing logic with LangChain & Ollama
├── requirements.txt    # Dependencies
├── .env                # Environment variables (not uploaded to GitHub)
├── chromedriver        # Optional local Selenium driver
```

---

## 📌 Requirements

* Python 3.8+
* Chrome or Chromium
* [Ollama](https://ollama.com/)
* Bright Data scraping browser session (free trial available)

---

## 🧠 Future Improvements

* Async processing for faster chunk parsing
* Add OpenAI/GPT support as fallback
* Support for paginated or multi-page scraping
* Deployable version on HuggingFace or Streamlit Cloud

---

## 🙋‍♂️ Author

**Akash Routh**
Passionate about AI, automation, and making the web smarter.
🔗 [GitHub](https://github.com/AkashRouth001)

---

## 🛡️ License

This project is licensed under the MIT License.

```

---

Let me know if you'd like:
- A version with advanced features documented
- Markdown badges (build, stars, license, etc.)
- A `demo.mp4` or GIF if you want to include a quick visual demo

I can also help create a short **demo video** script or thumbnail if you're planning to showcase this online.
```
