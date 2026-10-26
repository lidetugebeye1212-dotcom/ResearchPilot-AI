# 🔬 ResearchPilot AI

**AI-powered research assistant that searches the web, extracts evidence, evaluates source quality indicators, and generates structured research reports with citations.**

## 📌 Overview

ResearchPilot AI helps users investigate research questions more efficiently. It searches for relevant web sources, extracts available webpage content, and uses a large language model to produce an organized report based on the collected evidence.

Instead of relying only on a generated answer, ResearchPilot AI provides source references, highlights evidence gaps, and displays source quality indicators to help users assess the material.

## ✨ Features

- **🔎 Web Search:** Find relevant sources for a research question.
- **📄 Evidence Extraction:** Retrieve webpage text where available, with search snippets as a fallback.
- **🤖 AI Research Reports:** Generate structured reports using Groq-powered language models.
- **🔗 Source Citations:** Connect findings to collected source references.
- **🛡️ Source Quality Indicators:** Examine visible metadata and text-completeness indicators.
- **📊 Evidence Gaps and Limitations:** Highlight missing information and limitations in the available evidence.
- **📥 Report Export:** Download the generated research report as a Markdown file.
- **🎚️ Research Depth:** Choose Quick, Standard, or Deep research modes.
- **💻 Interactive Interface:** Use the Streamlit web interface to run research queries.

## 🛠️ Technology Stack

- **Python** — application logic
- **Streamlit** — interactive web interface
- **Groq API** — AI-generated research reports
- **DuckDuckGo Search (`ddgs`)** — web search
- **Requests** — webpage requests
- **BeautifulSoup** — HTML text extraction

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd researchpilot
```

If you already have the project folder, open a terminal in that folder instead.

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the environment

**Windows PowerShell:**

```powershell
.\.venv\Scripts\Activate.ps1
```

**Windows Command Prompt:**

```bat
.venv\Scripts\activate.bat
```

### 4. Install dependencies

Install the packages used by the application:

```bash
pip install streamlit groq ddgs requests beautifulsoup4
```

If your project has a `requirements.txt` file, you can instead run:

```bash
pip install -r requirements.txt
```

### 5. Configure the Groq API key

Create or obtain an API key through the Groq developer console.

Enter the key in the application's API key field if your current interface supports it. Keep API keys private, and never commit them to a public repository.

### 6. Run the application

```bash
python -m streamlit run app.py
```

Streamlit will display a local URL in the terminal, typically:

```text
http://localhost:8501
```

Open that URL in your browser.

## 🚀 How to Use

1. Launch ResearchPilot AI.
2. Enter a research question.
3. Select a research depth: Quick, Standard, or Deep.
4. Start the research process.
5. Review the generated report and citations.
6. Expand the source entries to inspect available evidence and source quality indicators.
7. Download the report in Markdown format.

## 📝 Report Structure

Depending on the available evidence, a generated report may contain:

- Executive Summary
- Key Findings
- Cross-Source Comparison
- Evidence Gaps
- Limitations
- Conclusion and Next Steps
- Source Citations

The report should distinguish sourced findings from interpretations and identify areas where evidence is insufficient.

## 🛡️ Source Quality and Limitations

ResearchPilot AI checks visible source information, such as source type, author or institution indicators, date information, methodological details, and the amount of substantive text available.

**Important:** These indicators are preliminary checks, not a verified measure of source accuracy, trustworthiness, or bias. A website's domain alone does not establish that its claims are correct.

Other limitations include:

- Some webpages may block automated access or provide little readable text.
- Search results may be incomplete or change over time.
- AI-generated reports may contain mistakes or misinterpret evidence.
- Citation quality depends on the sources collected and how accurately findings are linked to them.
- API usage limits and availability depend on the selected provider and account.

Always consult original sources before relying on important research findings.

## 🔐 Security

- Never publish your Groq API key.
- Do not commit `.env` files or other files containing secrets.
- Add `.venv/` and other local development artifacts to `.gitignore`.
- Avoid uploading confidential research material to services without checking their data policies.

## 🗺️ Future Improvements

Potential future features include:

- Evidence comparison matrix
- Automatic identification of conflicting claims
- More advanced source verification
- Research history and saved reports
- PDF export
- Improved source metadata extraction
- Support for academic papers and scholarly databases

## 🤝 Contributing

Contributions, suggestions, and bug reports are welcome. Fork the repository, create a feature branch, and submit a pull request.

## 📄 License

Choose and add a license before distributing the project publicly. For example, an MIT License can be added by including a `LICENSE` file containing the appropriate license text.

---

**ResearchPilot AI — From research questions to evidence-based insights.**
