---
layout: default
---

<style>
    body {
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        line-height: 1.6;
        color: #2d3748;
    }

    /* Hero Section */
    .hero {
        text-align: center;
        padding: 60px 20px;
        margin-bottom: 60px;
    }

    .hero h1 {
        font-size: 2.5em;
        font-weight: 700;
        margin-bottom: 10px;
        color: #1a202c;
    }

    .hero .tagline {
        font-size: 1.3em;
        color: #667eea;
        font-weight: 500;
        margin-bottom: 15px;
    }

    .hero .subtitle {
        font-size: 1.05em;
        color: #4a5568;
        max-width: 600px;
        margin: 0 auto;
    }

    /* Stats Grid */
    .stats {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
        gap: 20px;
        margin: 50px 0;
    }

    .stat-item {
        text-align: center;
        padding: 25px;
        background: #f7fafc;
        border-radius: 10px;
        transition: transform 0.3s ease;
    }

    .stat-item:hover {
        transform: translateY(-5px);
    }

    .stat-number {
        font-size: 2em;
        font-weight: 700;
        color: #667eea;
        display: block;
    }

    .stat-label {
        font-size: 0.9em;
        color: #718096;
        text-transform: uppercase;
        letter-spacing: 0.5px;
        margin-top: 5px;
    }

    /* Section Titles */
    h2 {
        font-size: 1.8em;
        color: #1a202c;
        margin: 60px 0 30px 0;
        font-weight: 700;
        border-bottom: 3px solid #667eea;
        padding-bottom: 10px;
    }

    /* Experience Cards */
    .experience-item {
        margin-bottom: 40px;
        padding: 25px;
        background: #ffffff;
        border-left: 4px solid #667eea;
        border-radius: 8px;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
    }

    .experience-header {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        margin-bottom: 10px;
        flex-wrap: wrap;
    }

    .experience-item h3 {
        font-size: 1.4em;
        color: #1a202c;
        margin: 0;
        font-weight: 700;
    }

    .company-location {
        color: #718096;
        font-size: 0.9em;
    }

    .period {
        color: #667eea;
        font-weight: 600;
        font-size: 0.9em;
    }

    .role {
        font-size: 1.1em;
        color: #4a5568;
        font-weight: 600;
        margin: 15px 0;
        font-style: italic;
    }

    .experience-item ul {
        margin: 15px 0 0 0;
        padding-left: 20px;
    }

    .experience-item li {
        color: #4a5568;
        margin-bottom: 10px;
        line-height: 1.7;
    }

    /* Skills Grid */
    .skills-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 20px;
        margin-top: 20px;
    }

    .skill-box {
        padding: 20px;
        background: #f7fafc;
        border-radius: 8px;
        border-left: 4px solid #667eea;
    }

    .skill-box h3 {
        font-size: 1.1em;
        color: #667eea;
        margin: 0 0 10px 0;
        font-weight: 700;
    }

    .skill-box p {
        color: #4a5568;
        line-height: 1.6;
        margin: 0;
        font-size: 0.95em;
    }

    /* Project Cards */
    .project {
        margin-bottom: 35px;
        padding: 25px;
        background: #ffffff;
        border-radius: 8px;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
        transition: all 0.3s ease;
    }

    .project:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
    }

    .project-header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 15px;
        flex-wrap: wrap;
        gap: 10px;
    }

    .project h3 {
        font-size: 1.3em;
        color: #1a202c;
        margin: 0;
        font-weight: 700;
    }

    .github-link {
        display: inline-flex;
        align-items: center;
        gap: 6px;
        background: #24292e;
        color: white !important;
        padding: 8px 16px;
        border-radius: 6px;
        text-decoration: none;
        font-size: 0.9em;
        font-weight: 600;
        transition: all 0.3s ease;
    }

    .github-link:hover {
        background: #667eea;
    }

    .tags {
        margin: 10px 0 15px 0;
    }

    .tag {
        display: inline-block;
        background: #e6f0ff;
        color: #667eea;
        padding: 5px 12px;
        border-radius: 15px;
        font-size: 0.85em;
        font-weight: 600;
        margin: 3px 5px 3px 0;
    }

    .project-description {
        color: #4a5568;
        line-height: 1.7;
        margin-bottom: 15px;
    }

    .project-image {
        width: 100%;
        border-radius: 8px;
        margin-top: 15px;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    /* Responsive */
    @media (max-width: 768px) {
        .hero h1 {
            font-size: 2em;
        }

        .hero .tagline {
            font-size: 1.1em;
        }

        h2 {
            font-size: 1.5em;
        }

        .stats {
            grid-template-columns: repeat(2, 1fr);
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
    <div class="subtitle">Transforming data into actionable insights with AI and advanced analytics</div>
</div>

<div class="stats">
    <div class="stat-item">
        <span class="stat-number">3+</span>
        <span class="stat-label">Years Experience</span>
    </div>
    <div class="stat-item">
        <span class="stat-number">12+</span>
        <span class="stat-label">Projects</span>
    </div>
    <div class="stat-item">
        <span class="stat-number">10+</span>
        <span class="stat-label">Technologies</span>
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
        <li>Architected end-to-end <strong>Text-to-SQL system</strong> using <strong>LangChain</strong> and <strong>LangGraph</strong> for 50+ beta users, reducing query creation time by <strong>65%</strong></li>
        <li>Engineered automated <strong>invoice processing pipeline</strong> with LLMs, achieving <strong>85%+ accuracy</strong> across 10,000+ invoices</li>
        <li>Built robust <strong>agentic workflows</strong> with <strong>92% task completion rate</strong> across LLM-powered applications</li>
        <li>Led integration of LLM solutions with cross-functional teams, scaling to handle <strong>500+ daily queries</strong></li>
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
        <li>Developed provider search system using <strong>advanced NLP</strong> and <strong>LLMs</strong>, boosting search efficiency by <strong>30%</strong></li>
        <li>Implemented <strong>NER</strong> and <strong>semantic search</strong> for medical term retrieval, achieving <strong>25%</strong> efficiency enhancement</li>
    </ul>
    <div class="role">Associate II Data Scientist (Jul 2022 – Sept 2022)</div>
    <ul>
        <li>Evaluated patient data using <strong>BigQuery</strong>, improving client understanding by <strong>45%</strong> for 10,000+ patients</li>
        <li>Designed data anomaly detection system adhering to <strong>HIPAA</strong> and <strong>GDPR</strong> compliance</li>
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

<h2>Featured Projects</h2>

<div class="project">
    <div class="project-header">
        <h3>RAG QA Bot</h3>
        <a href="https://github.com/dasdristanta13/RAG-ai-bot" class="github-link" target="_blank">→ GitHub</a>
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
        <a href="https://github.com/dasdristanta13/2.5D-Visual-Sound" class="github-link" target="_blank">→ GitHub</a>
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
        <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Topic_modelling" class="github-link" target="_blank">→ GitHub</a>
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
        <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Resume_Analysis" class="github-link" target="_blank">→ GitHub</a>
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
        <a href="https://github.com/dasdristanta13/Bankruptcy_LDA" class="github-link" target="_blank">→ GitHub</a>
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
        <a href="https://github.com/dasdristanta13/Time-series" class="github-link" target="_blank">→ GitHub</a>
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
        <a href="https://github.com/dasdristanta13/Fifa21EDA/blob/main/README.md" class="github-link" target="_blank">→ GitHub</a>
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
        <a href="https://github.com/dasdristanta13/Zomato_Food_EDA" class="github-link" target="_blank">→ GitHub</a>
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
