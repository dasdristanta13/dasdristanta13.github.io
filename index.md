---
layout: default
---

<style>
    body {
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
        line-height: 1.6;
        color: #333;
    }

    /* Hero */
    .hero {
        text-align: center;
        padding: 40px 20px;
        margin-bottom: 50px;
    }

    .hero h1 {
        font-size: 2.2em;
        font-weight: 600;
        margin-bottom: 8px;
        color: #000;
    }

    .hero .tagline {
        font-size: 1.1em;
        color: #666;
        margin-bottom: 8px;
    }

    .hero .subtitle {
        font-size: 0.95em;
        color: #888;
    }

    /* Stats */
    .stats {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 15px;
        margin: 40px 0 50px 0;
        max-width: 700px;
        margin-left: auto;
        margin-right: auto;
    }

    .stat-item {
        text-align: center;
        padding: 20px 10px;
        background: #f8f9fa;
        border-radius: 6px;
    }

    .stat-number {
        font-size: 1.8em;
        font-weight: 600;
        color: #000;
        display: block;
    }

    .stat-label {
        font-size: 0.85em;
        color: #666;
        margin-top: 3px;
    }

    /* Sections */
    h2 {
        font-size: 1.5em;
        color: #000;
        margin: 50px 0 20px 0;
        font-weight: 600;
        border-bottom: 2px solid #000;
        padding-bottom: 8px;
    }

    /* Experience */
    .experience-item {
        margin-bottom: 30px;
        padding-bottom: 30px;
        border-bottom: 1px solid #e0e0e0;
    }

    .experience-item:last-child {
        border-bottom: none;
    }

    .experience-header {
        display: flex;
        justify-content: space-between;
        align-items: baseline;
        margin-bottom: 8px;
        flex-wrap: wrap;
        gap: 10px;
    }

    .experience-item h3 {
        font-size: 1.2em;
        color: #000;
        margin: 0;
        font-weight: 600;
    }

    .company-location {
        color: #888;
        font-size: 0.9em;
    }

    .period {
        color: #666;
        font-size: 0.9em;
        font-weight: 500;
    }

    .role {
        font-size: 1em;
        color: #444;
        font-weight: 500;
        margin: 10px 0;
    }

    .experience-item ul {
        margin: 10px 0 0 0;
        padding-left: 18px;
    }

    .experience-item li {
        color: #555;
        margin-bottom: 8px;
        line-height: 1.6;
        font-size: 0.95em;
    }

    /* Skills */
    .skills-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 15px;
        margin-top: 20px;
    }

    .skill-box {
        padding: 15px;
        background: #f8f9fa;
        border-radius: 6px;
    }

    .skill-box h3 {
        font-size: 1em;
        color: #000;
        margin: 0 0 8px 0;
        font-weight: 600;
    }

    .skill-box p {
        color: #666;
        line-height: 1.5;
        margin: 0;
        font-size: 0.9em;
    }

    /* Projects */
    .project {
        margin-bottom: 30px;
        padding-bottom: 30px;
        border-bottom: 1px solid #e0e0e0;
    }

    .project:last-child {
        border-bottom: none;
    }

    .project-header {
        display: flex;
        justify-content: space-between;
        align-items: baseline;
        margin-bottom: 12px;
        flex-wrap: wrap;
        gap: 10px;
    }

    .project h3 {
        font-size: 1.15em;
        color: #000;
        margin: 0;
        font-weight: 600;
    }

    .github-link {
        color: #666 !important;
        text-decoration: none;
        font-size: 0.9em;
        font-weight: 500;
        transition: color 0.2s;
    }

    .github-link:hover {
        color: #000 !important;
    }

    .tags {
        margin: 8px 0 12px 0;
    }

    .tag {
        display: inline-block;
        color: #666;
        padding: 3px 10px;
        border: 1px solid #ddd;
        border-radius: 3px;
        font-size: 0.8em;
        margin: 3px 5px 3px 0;
    }

    .project-description {
        color: #555;
        line-height: 1.6;
        margin-bottom: 15px;
        font-size: 0.95em;
    }

    .project-image {
        width: 100%;
        border-radius: 4px;
        margin-top: 15px;
        border: 1px solid #e0e0e0;
    }

    /* Responsive */
    @media (max-width: 768px) {
        .hero h1 {
            font-size: 1.8em;
        }

        h2 {
            font-size: 1.3em;
        }

        .stats {
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
        }

        .skills-grid {
            grid-template-columns: 1fr;
        }

        .experience-header,
        .project-header {
            flex-direction: column;
            align-items: flex-start;
        }
    }
</style>

<div class="hero">
    <h1>Dristanta Das</h1>
    <div class="tagline">Data Science & Machine Learning Engineer</div>
    <div class="subtitle">Transforming data into actionable insights</div>
</div>

<div class="stats">
    <div class="stat-item">
        <span class="stat-number">3+</span>
        <span class="stat-label">Years</span>
    </div>
    <div class="stat-item">
        <span class="stat-number">12+</span>
        <span class="stat-label">Projects</span>
    </div>
    <div class="stat-item">
        <span class="stat-number">10+</span>
        <span class="stat-label">Tech Stack</span>
    </div>
    <div class="stat-item">
        <span class="stat-number">∞</span>
        <span class="stat-label">Learning</span>
    </div>
</div>

<h2>Experience</h2>

<div class="experience-item">
    <div class="experience-header">
        <div>
            <h3>Genpact</h3>
            <div class="company-location">Bengaluru, Karnataka</div>
        </div>
        <div class="period">Apr 2025 – Present</div>
    </div>
    <div class="role">Assistant Manager - Data Science</div>
    <ul>
        <li>Architected end-to-end Text-to-SQL system using LangChain and LangGraph for 50+ users, reducing query creation time by 65%</li>
        <li>Engineered automated invoice processing pipeline with LLMs, achieving 85%+ accuracy across 10,000+ invoices</li>
        <li>Built agentic workflows with 92% task completion rate across LLM-powered applications</li>
        <li>Led integration of LLM solutions with cross-functional teams, scaling to 500+ daily queries</li>
    </ul>
</div>

<div class="experience-item">
    <div class="experience-header">
        <div>
            <h3>UST</h3>
            <div class="company-location">Kolkata, West Bengal</div>
        </div>
        <div class="period">Jul 2022 – Mar 2025</div>
    </div>
    <div class="role">Associate III Data Scientist (Oct 2022 – Mar 2025)</div>
    <ul>
        <li>Developed provider search system using advanced NLP and LLMs, boosting search efficiency by 30%</li>
        <li>Implemented NER and semantic search for medical term retrieval, achieving 25% efficiency enhancement</li>
    </ul>
    <div class="role">Associate II Data Scientist (Jul 2022 – Sept 2022)</div>
    <ul>
        <li>Evaluated patient data using BigQuery, improving client understanding by 45% for 10,000+ patients</li>
        <li>Designed data anomaly detection system adhering to HIPAA and GDPR compliance</li>
    </ul>
</div>

<h2>Skills</h2>

<div class="skills-grid">
    <div class="skill-box">
        <h3>AI/ML</h3>
        <p>NLP, LLMs, NER, RAG, Machine Learning, Deep Learning, Statistical Modeling</p>
    </div>
    <div class="skill-box">
        <h3>Frameworks</h3>
        <p>LangChain, LangGraph, PyTorch, Hugging Face, Scikit-learn, XGBoost, FastAPI, Spacy</p>
    </div>
    <div class="skill-box">
        <h3>Tools & Cloud</h3>
        <p>Python, R, SQL, Git, Docker, BigQuery, Vector DBs, AWS, Azure</p>
    </div>
    <div class="skill-box">
        <h3>Design</h3>
        <p>Architecture Design, Data Flow Modeling, UML, Anomaly Detection, HIPAA & GDPR</p>
    </div>
</div>

<h2>Projects</h2>

<div class="project">
    <div class="project-header">
        <h3>RAG QA Bot</h3>
        <a href="https://github.com/dasdristanta13/RAG-ai-bot" class="github-link" target="_blank">GitHub →</a>
    </div>
    <div class="tags">
        <span class="tag">RAG</span>
        <span class="tag">LangChain</span>
        <span class="tag">BM25</span>
        <span class="tag">DPR</span>
        <span class="tag">LLMs</span>
    </div>
    <div class="project-description">
        Python-based QA bot with hybrid retrieval using BM25 and DPR, achieving 40% higher accuracy. Integrated GPT-3.5-turbo, Phi-2, and Llama3 with contextual compression to reduce hallucinations by 60%.
    </div>
</div>

<div class="project">
    <div class="project-header">
        <h3>2.5D Visual Sound</h3>
        <a href="https://github.com/dasdristanta13/2.5D-Visual-Sound" class="github-link" target="_blank">GitHub →</a>
    </div>
    <div class="tags">
        <span class="tag">Audio Processing</span>
        <span class="tag">Computer Vision</span>
        <span class="tag">Deep Learning</span>
    </div>
    <div class="project-description">
        Converting monaural audio into binaural audio by leveraging video, providing listeners with 3D sound sensation and rich perceptual experience.
    </div>
    <img src="images/ML_Project_report.png" alt="2.5D Visual Sound" class="project-image">
</div>

<div class="project">
    <div class="project-header">
        <h3>Topic Modelling of NLP Repositories</h3>
        <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Topic_modelling" class="github-link" target="_blank">GitHub →</a>
    </div>
    <div class="tags">
        <span class="tag">Topic Modeling</span>
        <span class="tag">GitHub API</span>
        <span class="tag">spaCy</span>
    </div>
    <div class="project-description">
        Analyzed popular NLP repositories using GitHub API and spaCy to understand how NLP libraries are being used in the community.
    </div>
    <img src="images/Topic_modelling.png" alt="Topic Modelling" class="project-image">
</div>

<div class="project">
    <div class="project-header">
        <h3>Resume Analysis with Spacy</h3>
        <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Resume_Analysis" class="github-link" target="_blank">GitHub →</a>
    </div>
    <div class="tags">
        <span class="tag">NLP</span>
        <span class="tag">Information Extraction</span>
        <span class="tag">Spacy</span>
    </div>
    <div class="project-description">
        Intelligent resume scoring system using Spacy for automated candidate evaluation and ranking based on job requirements.
    </div>
</div>

<div class="project">
    <div class="project-header">
        <h3>Bankruptcy Prediction with LDA</h3>
        <a href="https://github.com/dasdristanta13/Bankruptcy_LDA" class="github-link" target="_blank">GitHub →</a>
    </div>
    <div class="tags">
        <span class="tag">LDA</span>
        <span class="tag">Statistical Modeling</span>
        <span class="tag">Classification</span>
    </div>
    <div class="project-description">
        Statistical data analysis using Linear Discriminant Analysis with advanced dimensionality reduction to predict financial distress in companies.
    </div>
    <img src="images/Rplot4.png" alt="Bankruptcy Analysis" class="project-image">
</div>

<div class="project">
    <div class="project-header">
        <h3>Financial Time Series Forecasting</h3>
        <a href="https://github.com/dasdristanta13/Time-series" class="github-link" target="_blank">GitHub →</a>
    </div>
    <div class="tags">
        <span class="tag">Time Series</span>
        <span class="tag">ARIMA</span>
        <span class="tag">Financial Analysis</span>
    </div>
    <div class="project-description">
        Comprehensive forecasting analysis of major global stock indices including Nifty 50, Dax, Dow Jones, and Nikkei using ARIMA models.
    </div>
    <img src="images/Nifty_Forecast.png" alt="Financial Forecasting" class="project-image">
</div>

<div class="project">
    <div class="project-header">
        <h3>FIFA 21 Data Analysis</h3>
        <a href="https://github.com/dasdristanta13/Fifa21EDA/blob/main/README.md" class="github-link" target="_blank">GitHub →</a>
    </div>
    <div class="tags">
        <span class="tag">EDA</span>
        <span class="tag">Sports Analytics</span>
        <span class="tag">Python</span>
    </div>
    <div class="project-description">
        Comprehensive analysis of FIFA 21 player statistics, uncovering insights about attributes, market values, and performance metrics across different positions and nationalities.
    </div>
    <img src="images/football.png" alt="FIFA 21 Analysis" class="project-image">
</div>

<div class="project">
    <div class="project-header">
        <h3>Zomato Food Data Analysis</h3>
        <a href="https://github.com/dasdristanta13/Zomato_Food_EDA" class="github-link" target="_blank">GitHub →</a>
    </div>
    <div class="tags">
        <span class="tag">Data Visualization</span>
        <span class="tag">R & Python</span>
        <span class="tag">Business Intelligence</span>
    </div>
    <div class="project-description">
        In-depth analysis of Zomato's restaurant and food delivery data, deriving insights about customer preferences, pricing strategies, and restaurant ratings.
    </div>
    <img src="images/zomato.png" alt="Zomato Analysis" class="project-image">
</div>

<meta http-equiv='cache-control' content='no-cache'> 
<meta http-equiv='expires' content='0'> 
<meta http-equiv='pragma' content='no-cache'>
