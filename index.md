---
layout: default
---

<style>
    body {
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        line-height: 1.6;
        color: #333;
    }

    .portfolio-header {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        color: white;
        padding: 60px 40px;
        text-align: center;
        border-radius: 15px;
        margin-bottom: 50px;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    }

    .portfolio-header h1 {
        font-size: 3em;
        font-weight: 700;
        margin-bottom: 10px;
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
    }

    .portfolio-header p {
        font-size: 1.2em;
        opacity: 0.95;
    }

    .section {
        margin-bottom: 70px;
    }

    .section-title {
        font-size: 2.2em;
        color: #667eea;
        margin-bottom: 35px;
        padding-bottom: 15px;
        border-bottom: 3px solid #667eea;
        font-weight: 600;
    }

    .project-card {
        background: #f8f9fa;
        border-radius: 15px;
        padding: 30px;
        margin-bottom: 30px;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
        border: 2px solid transparent;
    }

    .project-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 30px rgba(102, 126, 234, 0.2);
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
        font-size: 1.6em;
        color: #2d3748;
        font-weight: 600;
        margin: 0;
        flex: 1;
    }

    .github-badge {
        display: inline-flex;
        align-items: center;
        gap: 8px;
        background: #24292e;
        color: white !important;
        padding: 10px 20px;
        border-radius: 8px;
        text-decoration: none;
        font-weight: 500;
        transition: background 0.3s ease;
        font-size: 0.9em;
    }

    .github-badge:hover {
        background: #667eea;
    }

    .github-badge::before {
        content: "⚡";
        font-size: 1.2em;
    }

    .label {
        display: inline-block;
        background: #667eea;
        color: white;
        padding: 5px 15px;
        border-radius: 20px;
        font-size: 0.85em;
        font-weight: 600;
        margin-bottom: 15px;
    }

    .project-description {
        color: #4a5568;
        font-size: 1.05em;
        line-height: 1.8;
        margin-bottom: 25px;
        text-align: justify;
    }

    .project-image {
        width: 100%;
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        margin-top: 20px;
        display: block;
    }

    @media (max-width: 768px) {
        .portfolio-header {
            padding: 40px 20px;
        }

        .portfolio-header h1 {
            font-size: 2em;
        }

        .section-title {
            font-size: 1.8em;
        }

        .project-card {
            padding: 20px;
        }

        .project-title {
            font-size: 1.3em;
        }

        .project-header {
            flex-direction: column;
            align-items: flex-start;
        }
    }
</style>

<div class="portfolio-header">
    <h1>Portfolio</h1>
    <p>Data Science & Machine Learning Projects</p>
</div>

<section class="section">
    <h2 class="section-title">Machine Learning</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">2.5D Visual Sound</h3>
            <a href="https://github.com/dasdristanta13/2.5D-Visual-Sound" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div class="label">Audio Processing • Computer Vision</div>
        <div class="project-description">
            Binaural audio provides a listener with 3D sound sensation, allowing a rich perceptual experience of the scene. However, binaural recordings are scarcely available and require nontrivial expertise and equipment to obtain. We propose to convert common monaural audio into binaural audio by leveraging video.
        </div>
        <img src="images/ML_Project_report.png" alt="2.5D Visual Sound Project" class="project-image">
    </div>
</section>

<section class="section">
    <h2 class="section-title">Natural Language Processing</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Topic Modelling of NLP Repositories</h3>
            <a href="https://github.com/dasdristanta13/NLP_work/tree/main/Topic_modelling" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div class="label">Topic Modeling • GitHub API • spaCy</div>
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
        <div class="label">NLP • Information Extraction</div>
        <div class="project-description">
            Made a resume scoring system using Spacy.
        </div>
    </div>
</section>

<section class="section">
    <h2 class="section-title">Statistical Data Analysis</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Linear Discriminant Analysis of Bankruptcy Dataset</h3>
            <a href="https://github.com/dasdristanta13/Bankruptcy_LDA" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div class="label">LDA • Statistical Modeling</div>
        <div class="project-description">
            This project majorly focuses on statistical data analysis (LDA) of a bankruptcy data.
        </div>
        <img src="images/Rplot4.png" alt="Bankruptcy Analysis" class="project-image">
    </div>
</section>

<section class="section">
    <h2 class="section-title">Time Series Forecasting</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Financial Data Forecasting</h3>
            <a href="https://github.com/dasdristanta13/Time-series" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div class="label">Time Series • Financial Analysis</div>
        <div class="project-description">
            This repository contains Time Series Forecasting of Nifty 50, Dax, Dow Jones and Nikkei stock prices.
        </div>
        <img src="images/Nifty_Forecast.png" alt="Financial Forecasting" class="project-image">
    </div>
</section>

<section class="section">
    <h2 class="section-title">Exploratory Data Analysis</h2>
    
    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">FIFA 21 Game Data Analysis</h3>
            <a href="https://github.com/dasdristanta13/Fifa21EDA/blob/main/README.md" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div class="label">Data Visualization • Sports Analytics</div>
        <div class="project-description">
            This project focuses on visualizing the FIFA 21 game data and getting inference out of that. Data includes latest edition FIFA 2021 players attributes like Age, Nationality, Overall, Potential, Club, Value, Wage, Preferred Foot, International Reputation, Weak Foot, Skill Moves, Work Rate, Position, Jersey Number, Joined, Loaned From, Contract Valid Until, Height, Weight etc.
        </div>
        <img src="images/football.png" alt="FIFA 21 Analysis" class="project-image">
    </div>

    <div class="project-card">
        <div class="project-header">
            <h3 class="project-title">Zomato Food Data Analysis</h3>
            <a href="https://github.com/dasdristanta13/Zomato_Food_EDA" class="github-badge" target="_blank">View on GitHub</a>
        </div>
        <div class="label">Data Visualization • R & Python</div>
        <div class="project-description">
            This project focuses on visualizing the Zomato food data and getting inference out of it both using R and Python.
        </div>
        <img src="images/zomato.png" alt="Zomato Analysis" class="project-image">
    </div>
</section>

<meta http-equiv='cache-control' content='no-cache'> 
<meta http-equiv='expires' content='0'> 
<meta http-equiv='pragma' content='no-cache'>
