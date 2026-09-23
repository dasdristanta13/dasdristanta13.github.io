---
layout: default
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@500;600&family=IBM+Plex+Sans:wght@400;500;600;700&display=swap">

<style>
    :root {
        --ink: #0A2342; --ink-2: #1E3F66; --muted: #5D6E85;
        --line: #D9E1EC; --line-soft: #E8EDF4;
        --ground: #F4F7FB; --card: #FFFFFF;
        --c1: #2563EB; --c1i: #1D4ED8; --c1t: #EFF4FF;
        --c2: #7C3AED; --c2i: #6D28D9; --c2t: #F5F0FE;
        --c3: #059669; --c3i: #047857; --c3t: #E9F7F1;
        --c4: #EA7317; --c4i: #B45309; --c4t: #FDF3E7;
        --c5: #0E8C99; --c5i: #0B6E78; --c5t: #E6F4F6;
        --c6: #1E4FA3; --c6i: #173F84; --c6t: #EDF2FB;
        --c7: #C2185B; --c7i: #A0154B; --c7t: #FCEDF3;
        --sans: 'IBM Plex Sans', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
        --mono: 'IBM Plex Mono', 'Cascadia Mono', Consolas, monospace;
    }

    body {
        font-family: var(--sans);
        line-height: 1.6;
        color: var(--ink-2);
        background: var(--ground);
    }

    /* Top accent spine */
    .spine {
        height: 5px;
        margin: 0 0 30px 0;
        border-radius: 3px;
        background: linear-gradient(90deg, var(--c1) 0%, var(--c2) 17%, var(--c3) 34%, var(--c4) 50%, var(--c5) 66%, var(--c6) 83%, var(--c7) 100%);
    }

    /* Hero */
    .hero {
        text-align: center;
        padding: 20px 20px 40px;
        margin-bottom: 40px;
    }

    .hero .kicker {
        font-family: var(--mono);
        font-size: 0.78em;
        font-weight: 600;
        letter-spacing: .18em;
        text-transform: uppercase;
        color: var(--c2i);
        margin-bottom: 10px;
    }

    .hero h1 {
        font-size: 2.2em;
        font-weight: 700;
        letter-spacing: -.01em;
        margin-bottom: 8px;
        color: var(--ink);
    }

    .hero .tagline {
        font-size: 1.1em;
        color: var(--ink-2);
        margin-bottom: 8px;
        font-weight: 500;
    }

    .hero .subtitle {
        font-size: 0.95em;
        color: var(--muted);
    }

    /* Stats */
    .stats {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 15px;
        margin: 40px 0 50px 0;
        max-width: 760px;
        margin-left: auto;
        margin-right: auto;
    }

    .stat-item {
        text-align: center;
        padding: 18px 10px;
        background: var(--card);
        border: 1px solid var(--line);
        border-top: 3px solid var(--c);
        border-radius: 8px;
    }

    .stat-number {
        font-family: var(--mono);
        font-size: 1.7em;
        font-weight: 600;
        color: var(--ink);
        display: block;
    }

    .stat-label {
        font-family: var(--mono);
        font-size: 0.72em;
        letter-spacing: .06em;
        text-transform: uppercase;
        color: var(--muted);
        margin-top: 4px;
    }

    /* Sections */
    .sec-kicker {
        font-family: var(--mono);
        font-size: 0.78em;
        font-weight: 600;
        letter-spacing: .18em;
        text-transform: uppercase;
        color: var(--c);
        margin: 50px 0 4px 0;
    }

    h2 {
        font-size: 1.5em;
        color: var(--ink);
        margin: 0 0 22px 0;
        font-weight: 700;
        padding-bottom: 10px;
        border-bottom: 3px solid var(--c);
        display: inline-block;
    }

    h3.group-heading {
        font-family: var(--mono);
        font-size: 0.85em;
        font-weight: 600;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: var(--muted);
        margin: 34px 0 16px 0;
        padding-top: 10px;
        border-top: 1px dashed var(--line);
    }

    /* Experience */
    .experience-item {
        margin-bottom: 22px;
        padding: 18px 20px;
        background: var(--card);
        border: 1px solid var(--line);
        border-left: 4px solid var(--c);
        border-radius: 8px;
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
        color: var(--ink);
        margin: 0;
        font-weight: 700;
    }

    .company-location {
        color: var(--muted);
        font-size: 0.9em;
    }

    .period {
        font-family: var(--mono);
        color: var(--muted);
        font-size: 0.82em;
        font-weight: 600;
    }

    .role {
        font-size: 1em;
        color: var(--ink-2);
        font-weight: 600;
        margin: 10px 0;
    }

    .experience-item ul {
        margin: 10px 0 0 0;
        padding-left: 18px;
    }

    .experience-item li {
        color: var(--ink-2);
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
        padding: 15px 16px;
        background: var(--card);
        border: 1px solid var(--line);
        border-top: 3px solid var(--c);
        border-radius: 8px;
    }

    .skill-box h3 {
        font-family: var(--mono);
        font-size: 0.85em;
        letter-spacing: .08em;
        text-transform: uppercase;
        color: var(--ink);
        margin: 0 0 8px 0;
        font-weight: 600;
    }

    .skill-box p {
        color: var(--muted);
        line-height: 1.5;
        margin: 0;
        font-size: 0.9em;
    }

    /* Projects */
    .project {
        margin-bottom: 22px;
        padding: 20px 22px 18px;
        background: var(--card);
        border: 1px solid var(--line);
        border-top: 4px solid var(--c);
        border-radius: 8px;
    }

    .project-header {
        display: flex;
        justify-content: space-between;
        align-items: baseline;
        margin-bottom: 10px;
        flex-wrap: wrap;
        gap: 10px;
    }

    .project h3 {
        font-size: 1.15em;
        color: var(--ink);
        margin: 0;
        font-weight: 700;
    }

    .github-link, .project-label {
        color: var(--ci) !important;
        text-decoration: none;
        font-family: var(--mono);
        font-size: 0.78em;
        font-weight: 600;
        letter-spacing: .04em;
        transition: color 0.2s;
        white-space: nowrap;
    }

    .github-link:hover {
        color: var(--c) !important;
    }

    .project-label {
        background: var(--ct);
        border: 1px solid var(--line);
        border-radius: 4px;
        padding: 3px 8px;
    }

    .tags {
        margin: 6px 0 12px 0;
    }

    .tag {
        display: inline-block;
        font-family: var(--mono);
        color: var(--ink-2);
        background: var(--ground);
        padding: 3px 8px;
        border: 1px solid var(--line);
        border-radius: 4px;
        font-size: 0.75em;
        margin: 3px 5px 3px 0;
    }

    .project-description {
        color: var(--ink-2);
        line-height: 1.6;
        margin-bottom: 14px;
        font-size: 0.95em;
    }

    .project-metrics {
        display: flex;
        flex-wrap: wrap;
        gap: 8px 22px;
        padding: 12px 0 2px;
        border-top: 1px dashed var(--line);
        margin-top: 4px;
    }

    .project-metrics .metric {
        display: flex;
        align-items: baseline;
        gap: 6px;
    }

    .project-metrics .metric b {
        font-family: var(--mono);
        font-size: 1.05em;
        font-weight: 700;
        color: var(--ci);
    }

    .project-metrics .metric span {
        font-size: 0.82em;
        color: var(--muted);
    }

    .project-image {
        width: 100%;
        border-radius: 4px;
        margin-top: 15px;
        border: 1px solid var(--line);
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

        .project-metrics {
            gap: 6px 16px;
        }
    }
</style>

<div class="spine"></div>

<div class="hero">
    <div class="kicker">Senior Data Scientist &middot; GenAI &amp; Agentic Systems</div>
    <h1>Dristanta Das</h1>
    <div class="tagline">Building production NLP, search &amp; agentic GenAI systems</div>
    <div class="subtitle">Turning slow, manual, human-in-the-middle workflows into governed, self-service ones</div>
</div>

<div class="stats">
    <div class="stat-item" style="--c:var(--c1)">
        <span class="stat-number">4+</span>
        <span class="stat-label">Years</span>
    </div>
    <div class="stat-item" style="--c:var(--c2)">
        <span class="stat-number">11+</span>
        <span class="stat-label">Projects</span>
    </div>
    <div class="stat-item" style="--c:var(--c4)">
        <span class="stat-number">10+</span>
        <span class="stat-label">Tech Stack</span>
    </div>
    <div class="stat-item" style="--c:var(--c5)">
        <span class="stat-number">&infin;</span>
        <span class="stat-label">Learning</span>
    </div>
</div>

<div class="sec-kicker" style="--c:var(--c2i)">&middot; Professional Timeline</div>
<h2 style="--c:var(--c2)">Experience</h2>

<div class="experience-item" style="--c:var(--c2)">
    <div class="experience-header">
        <div>
            <h3>Genpact</h3>
            <div class="company-location">Bengaluru, Karnataka</div>
        </div>
        <div class="period">Apr 2025 &ndash; Present</div>
    </div>
    <div class="role">Senior Data Scientist</div>
    <ul>
        <li>Architected and deployed an end-to-end Conversational Analytics (Text-to-SQL) platform using LangChain and LangGraph, cutting query-formulation time by 65% for 50+ beta users across 10 concurrent sessions</li>
        <li>Engineered agentic workflows with state management, error handling and dynamic routing at a 92% task-completion rate, scaling to 500+ weekly queries in production with 12+ cross-functional teams</li>
        <li>Spearheaded an automated invoice-processing pipeline with LangChain and Azure OpenAI, reaching 85%+ extraction accuracy across 10,000+ invoices in 8+ languages and cutting manual processing time by 60%</li>
    </ul>
</div>

<div class="experience-item" style="--c:var(--c6)">
    <div class="experience-header">
        <div>
            <h3>UST</h3>
            <div class="company-location">Kolkata, West Bengal</div>
        </div>
        <div class="period">Jul 2022 &ndash; Mar 2025</div>
    </div>
    <div class="role">Associate III Data Scientist (Oct 2022 &ndash; Mar 2025)</div>
    <ul>
        <li>Developed a client-facing provider search system using advanced NLP and open-source LLMs, boosting search efficiency by 30% and accelerating data-preparation tasks by 40%</li>
        <li>Implemented NER and semantic (vector-based) search to map layperson language to medical terms, achieving a 25% improvement in operational efficiency</li>
    </ul>
    <div class="role">Associate II Data Scientist (Jul 2022 &ndash; Sept 2022)</div>
    <ul>
        <li>Evaluated patient data using BigQuery, improving the client's understanding of adherence drivers by 45% for 10,000+ patients</li>
        <li>Designed a data anomaly-detection system for categorical healthcare data, adhering to HIPAA and GDPR compliance</li>
    </ul>
</div>

<div class="sec-kicker" style="--c:var(--c4i)">&middot; Capabilities</div>
<h2 style="--c:var(--c4)">Skills</h2>

<div class="skills-grid">
    <div class="skill-box" style="--c:var(--c1)">
        <h3>AI / ML</h3>
        <p>NLP, LLMs, NER, RAG, Agentic AI, Machine Learning, Deep Learning, Statistical Modeling</p>
    </div>
    <div class="skill-box" style="--c:var(--c2)">
        <h3>Frameworks</h3>
        <p>LangChain, LangGraph, PyTorch, Hugging Face, Scikit-learn, XGBoost, FastAPI, spaCy</p>
    </div>
    <div class="skill-box" style="--c:var(--c5)">
        <h3>Tools &amp; Cloud</h3>
        <p>Python, R, SQL, Git, Docker, BigQuery, Vector DBs, AWS, Azure (Azure OpenAI)</p>
    </div>
    <div class="skill-box" style="--c:var(--c7)">
        <h3>Design</h3>
        <p>Architecture Design, Data Flow Modeling, UML, Anomaly Detection, HIPAA &amp; GDPR Compliance</p>
    </div>
</div>

<div class="sec-kicker" style="--c:var(--c5i)">&middot; Featured Builds</div>
<h2 style="--c:var(--c5)">Projects</h2>

<h3 class="group-heading">Enterprise Production Systems</h3>

<div class="project" style="--c:var(--c2);--ci:var(--c2i);--ct:var(--c2t)">
    <div class="project-header">
        <h3>Conversational Analytics &mdash; Text-to-SQL Platform</h3>
        <span class="project-label">Genpact &middot; Production</span>
    </div>
    <div class="tags">
        <span class="tag">LangChain</span>
        <span class="tag">LangGraph</span>
        <span class="tag">Azure OpenAI</span>
        <span class="tag">Agentic AI</span>
        <span class="tag">Postgres</span>
    </div>
    <div class="project-description">
        Agentic Text-to-SQL platform over a certified semantic layer &mdash; business teams ask in plain English and get a governed, explained answer back instead of waiting on a data-team ticket.
    </div>
    <div class="project-metrics">
        <div class="metric"><b>65%</b><span>faster query-formulation time</span></div>
        <div class="metric"><b>500+</b><span>weekly queries, 50+ beta users</span></div>
        <div class="metric"><b>92%</b><span>agent task-completion rate</span></div>
        <div class="metric"><b>12+</b><span>cross-functional teams onboarded</span></div>
    </div>
</div>

<div class="project" style="--c:var(--c4);--ci:var(--c4i);--ct:var(--c4t)">
    <div class="project-header">
        <h3>Invoice Processing Pipeline</h3>
        <span class="project-label">Genpact &middot; Production</span>
    </div>
    <div class="tags">
        <span class="tag">LangChain</span>
        <span class="tag">Azure OpenAI</span>
        <span class="tag">Prompt Engineering</span>
        <span class="tag">Structured Output</span>
    </div>
    <div class="project-description">
        LLM-based extraction pipeline for multi-format invoices across EMEA and NAM, with structured-output validation and a human-review queue for low-confidence fields instead of blind automation.
    </div>
    <div class="project-metrics">
        <div class="metric"><b>85%+</b><span>field-extraction accuracy</span></div>
        <div class="metric"><b>10,000+</b><span>invoices processed</span></div>
        <div class="metric"><b>60%</b><span>less manual processing time</span></div>
        <div class="metric"><b>8+</b><span>languages, EMEA &amp; NAM</span></div>
    </div>
</div>

<div class="project" style="--c:var(--c6);--ci:var(--c6i);--ct:var(--c6t)">
    <div class="project-header">
        <h3>Provider Search System</h3>
        <span class="project-label">UST &middot; Production</span>
    </div>
    <div class="tags">
        <span class="tag">NLP</span>
        <span class="tag">NER</span>
        <span class="tag">Semantic Search</span>
        <span class="tag">Open-Source LLMs</span>
    </div>
    <div class="project-description">
        My most-cited win: an NLP + semantic-search system that maps layperson symptom descriptions to standardized medical terminology, so search resolves meaning rather than keywords. Predates the GenAI wave &mdash; built on NER and vector retrieval.
    </div>
    <div class="project-metrics">
        <div class="metric"><b>30%</b><span>boost in search efficiency</span></div>
        <div class="metric"><b>40%</b><span>faster data-preparation tasks</span></div>
        <div class="metric"><b>25%</b><span>gain in operational efficiency</span></div>
    </div>
</div>

<h3 class="group-heading">Personal &amp; Academic Projects</h3>

<div class="project" style="--c:var(--c1);--ci:var(--c1i);--ct:var(--c1t)">
    <div class="project-header">
        <h3>RAG QA Bot</h3>
        <a href="https://github.com/dasdristanta13/RAG-ai-bot" class="github-link" target="_blank">GitHub &rarr;</a>
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
    <div class="project-metrics">
        <div class="metric"><b>40%</b><span>higher accuracy vs. traditional search</span></div>
        <div class="metric"><b>60%</b><span>fewer hallucinations</span></div>
    </div>
</div>

<div class="project" style="--c:var(--c3);--ci:var(--c3i);--ct:var(--c3t)">
    <div class="project-header">
        <h3>2.5D Visual Sound</h3>
        <a href="https://github.com/dasdristanta13/2.5D-Visual-Sound" class="github-link" target="_blank">GitHub &rarr;</a>
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

<div class="project" style="--c:var(--c7);--ci:var(--c7i);--ct:var(--c7t)">
    <div class="project-header">
        <h3>Topic Modelling of NLP Repositories</h3>
        <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Topic_modelling" class="github-link" target="_blank">GitHub &rarr;</a>
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

<div class="project" style="--c:var(--c5);--ci:var(--c5i);--ct:var(--c5t)">
    <div class="project-header">
        <h3>Resume Analysis with Spacy</h3>
        <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Resume_Analysis" class="github-link" target="_blank">GitHub &rarr;</a>
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

<div class="project" style="--c:var(--c2);--ci:var(--c2i);--ct:var(--c2t)">
    <div class="project-header">
        <h3>Bankruptcy Prediction with LDA</h3>
        <a href="https://github.com/dasdristanta13/Bankruptcy_LDA" class="github-link" target="_blank">GitHub &rarr;</a>
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

<div class="project" style="--c:var(--c4);--ci:var(--c4i);--ct:var(--c4t)">
    <div class="project-header">
        <h3>Financial Time Series Forecasting</h3>
        <a href="https://github.com/dasdristanta13/Time-series" class="github-link" target="_blank">GitHub &rarr;</a>
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

<div class="project" style="--c:var(--c6);--ci:var(--c6i);--ct:var(--c6t)">
    <div class="project-header">
        <h3>FIFA 21 Data Analysis</h3>
        <a href="https://github.com/dasdristanta13/Fifa21EDA/blob/main/README.md" class="github-link" target="_blank">GitHub &rarr;</a>
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

<div class="project" style="--c:var(--c1);--ci:var(--c1i);--ct:var(--c1t)">
    <div class="project-header">
        <h3>Zomato Food Data Analysis</h3>
        <a href="https://github.com/dasdristanta13/Zomato_Food_EDA" class="github-link" target="_blank">GitHub &rarr;</a>
    </div>
    <div class="tags">
        <span class="tag">Data Visualization</span>
        <span class="tag">R &amp; Python</span>
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
