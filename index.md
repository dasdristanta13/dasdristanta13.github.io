---
layout: default
---

<style>
    /* Modern Portfolio Styling */
    body {
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        line-height: 1.6;
        color: #2d3748;
    }

    /* Animated gradient background for header */
    .portfolio-hero {
        background: linear-gradient(-45deg, #667eea, #764ba2, #f093fb, #4facfe);
        background-size: 400% 400%;
        animation: gradientShift 15s ease infinite;
        color: white;
        padding: 80px 40px;
        text-align: center;
        border-radius: 20px;
        margin: -20px -20px 50px -20px;
        box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
        position: relative;
        overflow: hidden;
    }

    @keyframes gradientShift {
        0% { background-position: 0% 50%; }
        50% { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }

    .portfolio-hero::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: url('data:image/svg+xml,<svg width="100" height="100" xmlns="http://www.w3.org/2000/svg"><defs><pattern id="grid" width="100" height="100" patternUnits="userSpaceOnUse"><path d="M 100 0 L 0 0 0 100" fill="none" stroke="rgba(255,255,255,0.1)" stroke-width="1"/></pattern></defs><rect width="100" height="100" fill="url(%23grid)"/></svg>');
        opacity: 0.3;
    }

    .portfolio-hero h1 {
        font-size: 3.5em;
        font-weight: 800;
        margin-bottom: 15px;
        text-shadow: 3px 3px 6px rgba(0, 0, 0, 0.3);
        position: relative;
        z-index: 1;
        letter-spacing: -1px;
    }

    .portfolio-hero .tagline {
        font-size: 1.4em;
        opacity: 0.95;
        font-weight: 300;
        position: relative;
        z-index: 1;
        margin-top: 10px;
    }

    .portfolio-hero .subtitle {
        font-size: 1.1em;
        opacity: 0.9;
        margin-top: 20px;
        position: relative;
        z-index: 1;
        font-weight: 400;
    }

    /* Stats counter section */
    .stats-section {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 20px;
        margin: 40px 0 60px 0;
    }

    .stat-card {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        color: white;
        padding: 30px;
        border-radius: 15px;
        text-align: center;
        box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
        transition: transform 0.3s ease;
    }

    .stat-card:hover {
        transform: translateY(-5px);
    }

    .stat-number {
        font-size: 2.5em;
        font-weight: 700;
        display: block;
        margin-bottom: 5px;
    }

    .stat-label {
        font-size: 0.9em;
        opacity: 0.9;
        text-transform: uppercase;
        letter-spacing: 1px;
    }

    /* Section styling */
    .section {
        margin-bottom: 80px;
        animation: fadeInUp 0.6s ease-out;
    }

    @keyframes fadeInUp {
        from {
            opacity: 0;
            transform: translateY(30px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .section-title {
        font-size: 2.5em;
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        margin-bottom: 40px;
        padding-bottom: 20px;
        border-bottom: 4px solid #667eea;
        font-weight: 700;
        position: relative;
        display: inline-block;
    }

    .section-title::after {
        content: '';
        position: absolute;
        bottom: -4px;
        left: 0;
        width: 0;
        height: 4px;
        background: #764ba2;
        transition: width 0.5s ease;
    }

    .section:hover .section-title::after {
        width: 100%;
    }

    /* Experience section */
    .experience-card {
        background: white;
        border-radius: 20px;
        padding: 35px;
        margin-bottom: 35px;
        border: 2px solid #e2e8f0;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
        position: relative;
        overflow: hidden;
        transition: all 0.4s ease;
    }

    .experience-card::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 5px;
        height: 100%;
        background: linear-gradient(180deg, #667eea 0%, #764ba2 100%);
    }

    .experience-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 15px 35px rgba(102, 126, 234, 0.2);
        border-color: #667eea;
    }

    .experience-header {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        margin-bottom: 15px;
        flex-wrap: wrap;
        gap: 10px;
    }

    .company-info h3 {
        font-size: 1.8em;
        color: #1a202c;
        margin: 0 0 5px 0;
        font-weight: 700;
    }

    .company-location {
        color: #718096;
        font-size: 0.95em;
        font-weight: 500;
    }

    .experience-period {
        color: #667eea;
        font-weight: 600;
        font-size: 0.95em;
        white-space: nowrap;
    }

    .job-title {
        font-size: 1.2em;
        color: #4a5568;
        font-weight: 600;
        margin-bottom: 20px;
        font-style: italic;
    }

    .experience-card ul {
        list-style: none;
        padding: 0;
        margin: 0;
    }

    .experience-card li {
        color: #4a5568;
        font-size: 1.05em;
        line-height: 1.8;
        margin-bottom: 15px;
        padding-left: 30px;
        position: relative;
    }

    .experience-card li::before {
        content: '▸';
        position: absolute;
        left: 10px;
        color: #667eea;
        font-weight: 700;
        font-size: 1.2em;
    }

    /* Enhanced project cards */
    .project-card {
        background: white;
        border-radius: 20px;
        padding: 35px;
        margin-bottom: 35px;
        transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        border: 2px solid #e2e8f0;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
        position: relative;
        overflow: hidden;
    }

    .project-card::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 5px;
        height: 100%;
        background: linear-gradient(180deg, #667eea 0%, #764ba2 100%);
        transform: scaleY(0);
        transition: transform 0.3s ease;
    }

    .project-card:hover::before {
        transform: scaleY(1);
    }

    .project-card:hover {
        transform: translateY(-10px) scale(1.02);
        box-shadow: 0 20px 40px rgba(102, 126, 234, 0.25);
        border-color: #667eea;
    }

    .project-header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin-bottom: 20px;
        flex-wrap: wrap;
        gap: 15px;
    }

    .project-title {
        font-size: 1.75em;
        color: #1a202c;
        font-weight: 700;
        margin: 0;
        flex: 1;
        transition: color 0.3s ease;
    }

    .project-card:hover .project-title {
        color: #667eea;
    }

    /* Enhanced GitHub badge */
    .github-badge {
        display: inline-flex;
        align-items: center;
        gap: 8px;
        background: linear-gradient(135deg, #24292e 0%, #1a1f24 100%);
        color: white !important;
        padding: 12px 24px;
        border-radius: 10px;
        text-decoration: none;
        font-weight: 600;
        transition: all 0.3s ease;
        font-size: 0.95em;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        position: relative;
        overflow: hidden;
    }

    .github-badge::before {
        content: "⚡";
        font-size: 1.3em;
        transition: transform 0.3s ease;
    }

    .github-badge::after {
        content: '';
        position: absolute;
        top: 50%;
        left: 50%;
        width: 0;
        height: 0;
        border-radius: 50%;
        background: rgba(255, 255, 255, 0.2);
        transform: translate(-50%, -50%);
        transition: width 0.5s ease, height 0.5s ease;
    }

    .github-badge:hover::after {
        width: 300px;
        height: 300px;
    }

    .github-badge:hover {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        transform: translateY(-2px);
        box-shadow: 0 6px 15px rgba(102, 126, 234, 0.4);
    }

    .github-badge:hover::before {
        transform: scale(1.2) rotate(10deg);
    }

    /* Skill labels */
    .label {
        display: inline-block;
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        color: white;
        padding: 8px 18px;
        border-radius: 25px;
        font-size: 0.85em;
        font-weight: 600;
        margin: 5px 5px 15px 0;
        box-shadow: 0 3px 10px rgba(102, 126, 234, 0.3);
        transition: transform 0.2s ease;
    }

    .label:hover {
        transform: scale(1.05);
    }

    .project-description {
        color: #4a5568;
        font-size: 1.08em;
        line-height: 1.9;
        margin-bottom: 25px;
        text-align: justify;
    }

    /* Enhanced image styling */
    .project-image {
        width: 100%;
        border-radius: 15px;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
        margin-top: 25px;
        display: block;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .project-image:hover {
        transform: scale(1.03);
        box-shadow: 0 15px 40px rgba(102, 126, 234, 0.3);
    }

    /* Category icons */
    .category-icon {
        display: inline-block;
        margin-right: 15px;
        font-size: 2em;
        vertical-align: middle;
    }

    /* Skills section */
    .skills-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 25px;
        margin-top: 30px;
    }

    .skill-category {
        background: white;
        padding: 25px;
        border-radius: 15px;
        border: 2px solid #e2e8f0;
        transition: all 0.3s ease;
    }

    .skill-category:hover {
        border-color: #667eea;
        box-shadow: 0 10px 25px rgba(102, 126, 234, 0.15);
        transform: translateY(-5px);
    }

    .skill-category h4 {
        color: #667eea;
        font-size: 1.2em;
        margin-bottom: 15px;
        font-weight: 700;
    }

    .skill-category p {
        color: #4a5568;
        line-height: 1.8;
        margin: 0;
    }

    /* Responsive design */
    @media (max-width: 768px) {
        .portfolio-hero {
            padding: 50px 20px;
            margin: -10px -10px 30px -10px;
        }

        .portfolio-hero h1 {
            font-size: 2.2em;
        }

        .portfolio-hero .tagline {
            font-size: 1.1em;
        }

        .stats-section {
            grid-template-columns: 1fr;
            gap: 15px;
        }

        .section-title {
            font-size: 1.9em;
        }

        .project-card, .experience-card {
            padding: 25px;
        }

        .project-title {
            font-size: 1.4em;
        }

        .project-header, .experience-header {
            flex-direction: column;
            align-items: flex-start;
        }

        .category-icon {
            font-size: 1.5em;
        }

        .company-info h3 {
            font-size: 1.5em;
        }

        .skills-grid {
            grid-template-columns: 1fr;
        }
    }

    /* Smooth scrolling */
    html {
        scroll-behavior: smooth;
    }

    /* Link styling */
    a {
        color: #667eea;
        transition: color 0.3s ease;
    }

    a:hover {
        color: #764ba2;
    }
</style>

<div class="portfolio-hero">
    <h1>🚀 Portfolio</h1>
    <div class="tagline">Data Science & Machine Learning Engineer</div>
    <div class="subtitle">Transforming Data into Actionable Insights with AI</div>
</div>

<div class="stats-section">
    <div class="stat-card">
        <span class="stat-number">3+</span>
        <span class="stat-label">Years Experience</span>
    </div>
    <div class="stat-card">
        <span class="stat-number">12+</span>
        <span class="stat-label">Projects</span>
    </div>
    <div class="stat-card">
        <span class="stat-number">10+</span>
        <span class="stat-label">Technologies</span>
    </div>
    <div class="stat-card">
        <span class="stat-number">∞</span>
        <span class="stat-label">Learning</span>
    </div>
</div>

<section class="section">
    <h2 class="section-title"><span class="category-icon">💼</span>Professional Experience</h2>
    
    <div class="experience-card">
        <div class="experience-header">
            <div class="company-info">
                <h3>Genpact</h3>
                <div class="company-location">Bengaluru, Karnataka</div>
            </div>
            <div class="experience-period">Apr 2025 – Present</div>
        </div>
        <div class="job-title">Assistant Manager - Data Science</div>
        <ul>
            <li>Architected and deployed an end-to-end <strong>Text-to-SQL system</strong> using <strong>LangChain</strong> and <strong>LangGraph</strong> for <strong>50+ beta users</strong>, supporting <strong>10 concurrent users</strong> and enabling natural language querying of complex databases, reducing query creation time by <strong>65%</strong>.</li>
            <li>Engineered an automated <strong>invoice processing pipeline</strong> leveraging <strong>LLMs</strong> for document parsing and information extraction, achieving <strong>85%+ accuracy</strong> across <strong>10,000+ invoices</strong> and reducing manual processing time by <strong>60%</strong>.</li>
            <li>Built robust <strong>agentic workflows</strong> with state management, error handling, and dynamic routing capabilities, achieving <strong>92% task completion rate</strong> and delivering superior user experience across LLM-powered applications.</li>
            <li>Spearheaded integration of LLM-powered solutions into production systems with cross-functional teams of <strong>12+ members</strong>, ensuring scalability to handle <strong>500+ daily queries</strong> and alignment with business requirements.</li>
        </ul>
    </div>

    <div class="experience-card">
        <div class="experience-header">
            <div class="company-info">
                <h3>UST</h3>
                <div class="company-location">Kolkata, West Bengal</div>
            </div>
            <div class="experience-period">Jul 2022 – Mar 2025</div>
        </div>
        <div class="job-title">Associate III Data Scientist (Oct 2022 – Mar 2025)</div>
        <ul>
            <li>Orchestrated development of a client-facing provider search system using <strong>advanced NLP techniques</strong> and open-source <strong>LLMs</strong>, boosting search efficiency by <strong>30%</strong> and accelerating data preparation tasks by <strong>40%</strong>.</li>
            <li>Implemented <strong>NER</strong> and <strong>semantic search</strong> capabilities for retrieving medical terms from layperson language, achieving <strong>25%</strong> enhancement in operational efficiency and improving service quality for end-users.</li>
        </ul>
        <div class="job-title">Associate II Data Scientist (Jul 2022 – Sept 2022)</div>
        <ul>
            <li>Conducted evaluation of patient data using <strong>BigQuery</strong> with comprehensive data transformations and statistical analysis, enhancing client understanding of adherence drivers by <strong>45%</strong> and improving outreach to over <strong>10,000 patients</strong>.</li>
            <li>Designed and implemented a data anomaly detection system for categorical healthcare data, adhering to <strong>HIPAA</strong> and <strong>GDPR</strong> compliance standards.</li>
        </ul>
    </div>
</section>

<section class="section">
    <h2 class="section-title"><span class="category-icon">🛠️</span>Technical Skills</h2>
    
    <div class="skills-grid">
        <div class="skill-category">
            <h4>AI/ML</h4>
            <p>Natural Language Processing (NLP), Large Language Models (LLMs), Named Entity Recognition (NER), Retrieval-Augmented Generation (RAG), Machine Learning, Deep Learning, Statistical & Predictive Modeling</p>
        </div>
        <div class="skill-category">
            <h4>Frameworks & Libraries</h4>
            <p>LangChain, LangGraph, PyTorch, Hugging Face Transformers, Scikit-learn, XGBoost, FastAPI, Spacy</p>
        </div>
        <div class="skill-category">
            <h4>Tools & Cloud</h4>
            <p>Python, R, SQL, Git (GitHub, GitLab, Bitbucket), Docker, BigQuery, Vector Databases, AWS, Azure, VS Code</p>
        </div>
        <div class="skill-category">
            <h4>Design & Compliance</h4>
            <p>High-Level Architecture Design, Data Flow Modeling, UML Diagrams, Anomaly Detection, HIPAA & GDPR Compliance</p>
        </div>
    </div>
</section>

<section class="section">
    <h2 class="section-title"><span class="category-icon">🤖</span>AI & LLM Projects</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Retrieval-Augmented Generation (RAG) QA Bot</h3>
            <a href="https://github.com/dasdristanta13/RAG-ai-bot" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div>
            <span class="label">RAG</span>
            <span class="label">LangChain</span>
            <span class="label">BM25</span>
            <span class="label">DPR</span>
            <span class="label">LLMs</span>
        </div>
        <div class="project-description">
            Engineered a Python-based QA bot with hybrid retrieval using BM25 and DPR, achieving 40% higher answer accuracy compared to traditional search methods. Integrated GPT-3.5-turbo, Phi-2, and Llama3 with contextual compression to reduce hallucinations by 60%; optimized performance using SQLite caching and Slack integration.
        </div>
    </div>

    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">2.5D Visual Sound</h3>
            <a href="https://github.com/dasdristanta13/2.5D-Visual-Sound" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div>
            <span class="label">Audio Processing</span>
            <span class="label">Computer Vision</span>
            <span class="label">Deep Learning</span>
        </div>
        <div class="project-description">
            Binaural audio provides a listener with 3D sound sensation, allowing a rich perceptual experience of the scene. However, binaural recordings are scarcely available and require nontrivial expertise and equipment to obtain. We propose to convert common monaural audio into binaural audio by leveraging video.
        </div>
        <img src="images/ML_Project_report.png" alt="2.5D Visual Sound Project" class="project-image">
    </div>
</section>

<section class="section">
    <h2 class="section-title"><span class="category-icon">💬</span>Natural Language Processing</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Topic Modelling of NLP Repositories</h3>
            <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Topic_modelling" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div>
            <span class="label">Topic Modeling</span>
            <span class="label">GitHub API</span>
            <span class="label">spaCy</span>
        </div>
        <div class="project-description">
            Used the GitHub API to return popular NLP-related repositories, then used spaCy and other NLP libraries to analyze the GitHub descriptions. In this way, we can attempt to get a sense of how NLP libraries are being used.
        </div>
        <img src="images/Topic_modelling.png" alt="Topic Modelling Project" class="project-image">
    </div>

    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Resume Analysis with Spacy</h3>
            <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Resume_Analysis" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div>
            <span class="label">NLP</span>
            <span class="label">Information Extraction</span>
            <span class="label">Spacy</span>
        </div>
        <div class="project-description">
            Developed an intelligent resume scoring system using Spacy for automated candidate evaluation and ranking based on job requirements.
        </div>
    </div>
</section>

<section class="section">
    <h2 class="section-title"><span class="category-icon">📊</span>Statistical Data Analysis</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Linear Discriminant Analysis of Bankruptcy Dataset</h3>
            <a href="https://github.com/dasdristanta13/Bankruptcy_LDA" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div>
            <span class="label">LDA</span>
            <span class="label">Statistical Modeling</span>
            <span class="label">Classification</span>
        </div>
        <div class="project-description">
            This project majorly focuses on statistical data analysis (LDA) of bankruptcy data, implementing advanced dimensionality reduction techniques to predict financial distress in companies.
        </div>
        <img src="images/Rplot4.png" alt="Bankruptcy Analysis" class="project-image">
    </div>
</section>

<section class="section">
    <h2 class="section-title"><span class="category-icon">📈</span>Time Series Forecasting</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Financial Data Forecasting</h3>
            <a href="https://github.com/dasdristanta13/Time-series" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div>
            <span class="label">Time Series</span>
            <span class="label">Financial Analysis</span>
            <span class="label">ARIMA</span>
        </div>
        <div class="project-description">
            Comprehensive time series forecasting analysis of major global stock indices including Nifty 50, Dax, Dow Jones, and Nikkei. Implemented ARIMA models to predict future price movements with high accuracy.
        </div>
        <img src="images/Nifty_Forecast.png" alt="Financial Forecasting" class="project-image">
    </div>
</section>

<section class="section">
    <h2 class="section-title"><span class="category-icon">🔍</span>Exploratory Data Analysis</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">FIFA 21 Game Data Analysis</h3>
            <a href="https://github.com/dasdristanta13/Fifa21EDA/blob/main/README.md" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div>
            <span class="label">Data Visualization</span>
            <span class="label">Sports Analytics</span>
            <span class="label">Python</span>
        </div>
        <div class="project-description">
            Comprehensive exploratory data analysis of FIFA 21 player statistics, uncovering insights about player attributes, market values, and performance metrics. Analyzed player characteristics including age, nationality, overall rating, potential, club affiliations, wages, playing positions, and physical attributes to identify trends in modern football.
        </div>
        <img src="images/football.png" alt="FIFA 21 Analysis" class="project-image">
    </div>

    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Zomato Food Data Analysis</h3>
            <a href="https://github.com/dasdristanta13/Zomato_Food_EDA" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div>
            <span class="label">Data Visualization</span>
            <span class="label">R & Python</span>
            <span class="label">Business Intelligence</span>
        </div>
        <div class="project-description">
            In-depth exploratory data analysis of Zomato's restaurant and food delivery data using both R and Python. Derived actionable insights about customer preferences, pricing strategies, and restaurant ratings across different cuisines and locations.
        </div>
        <img src="images/zomato.png" alt="Zomato Analysis" class="project-image">
    </div>
</section>

<meta http-equiv='cache-control' content='no-cache'> 
<meta http-equiv='expires' content='0'> 
<meta http-equiv='pragma' content='no-cache'>
