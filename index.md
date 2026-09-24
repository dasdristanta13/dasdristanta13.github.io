---
layout: default
---

<section class="hero">
  <div class="wrap hero-grid">
    <div>
      <p class="hero-role">Senior Data Scientist at Genpact &middot; Bengaluru</p>
      <h1>I turn slow, manual data workflows into governed, self-service ones.</h1>
      <p class="hero-copy">
        I design and ship <strong>Text-to-SQL</strong>, <strong>RAG</strong> and <strong>agentic</strong> systems
        with LangChain, LangGraph and PyTorch. Before Genpact, at UST, I built the provider search system
        (NER plus semantic search) that lifted search efficiency by 30%, still the result I'm asked about most.
      </p>
      <div class="hero-actions">
        <a class="btn" href="pdf/Dristanta_Das_Senior_Data_Scientist.pdf" target="_blank" rel="noopener">Download resume</a>
        <a href="https://www.linkedin.com/in/dasdristanta13/" target="_blank" rel="noopener">LinkedIn</a>
        <a href="https://github.com/dasdristanta13" target="_blank" rel="noopener">GitHub</a>
        <a href="mailto:dasdristanta13@gmail.com">Email</a>
      </div>
    </div>
    <img class="portrait" src="images/logo.jpg" width="208" height="208" alt="Portrait of Dristanta Das">
  </div>
</section>

<section class="section" id="work">
  <div class="wrap">
    <div class="section-head">
      <h2>Production systems</h2>
      <p class="section-note">Three systems used by real teams, with the measured result for each.</p>
    </div>

    <article class="case">
      <div>
        <h3>Conversational analytics: Text-to-SQL platform</h3>
        <p class="where">Genpact</p>
        <p class="what">An agentic Text-to-SQL platform over a certified semantic layer. Business teams ask in plain English and get a governed, explained answer instead of waiting on a data-team ticket.</p>
        <ul class="tags">
          <li>LangChain</li><li>LangGraph</li><li>Azure OpenAI</li><li>Agentic AI</li><li>Postgres</li>
        </ul>
      </div>
      <dl class="metrics">
        <div><dt>faster query formulation</dt><dd>65%</dd></div>
        <div><dt>weekly queries from 50+ beta users</dt><dd>500+</dd></div>
        <div><dt>agent task-completion rate</dt><dd>92%</dd></div>
        <div><dt>cross-functional teams onboarded</dt><dd>12+</dd></div>
      </dl>
    </article>

    <article class="case">
      <div>
        <h3>Invoice processing pipeline</h3>
        <p class="where">Genpact</p>
        <p class="what">An LLM extraction pipeline for multi-format invoices across EMEA and NAM. Structured-output validation and a human-review queue for low-confidence fields replace blind automation.</p>
        <ul class="tags">
          <li>LangChain</li><li>Azure OpenAI</li><li>Prompt engineering</li><li>Structured output</li>
        </ul>
      </div>
      <dl class="metrics">
        <div><dt>field-extraction accuracy</dt><dd>85%+</dd></div>
        <div><dt>invoices processed</dt><dd>10,000+</dd></div>
        <div><dt>less manual processing time</dt><dd>60%</dd></div>
        <div><dt>languages across EMEA and NAM</dt><dd>8+</dd></div>
      </dl>
    </article>

    <article class="case">
      <div>
        <h3>Provider search system</h3>
        <p class="where">UST</p>
        <p class="what">An NLP and semantic-search system that maps layperson symptom descriptions to standardized medical terminology, so search resolves meaning rather than keywords. Built on NER and vector retrieval, before the GenAI wave.</p>
        <ul class="tags">
          <li>NLP</li><li>NER</li><li>Semantic search</li><li>Open-source LLMs</li>
        </ul>
      </div>
      <dl class="metrics">
        <div><dt>boost in search efficiency</dt><dd>30%</dd></div>
        <div><dt>faster data-preparation tasks</dt><dd>40%</dd></div>
        <div><dt>gain in operational efficiency</dt><dd>25%</dd></div>
      </dl>
    </article>
  </div>
</section>

<section class="section" id="projects">
  <div class="wrap">
    <div class="section-head">
      <h2>More projects</h2>
      <p class="section-note">Personal and academic work across retrieval, audio, NLP, statistics and forecasting. Each links to its repository.</p>
    </div>

    <div class="bento">
      <article class="tile s7">
        <h3><a href="https://github.com/dasdristanta13/RAG-ai-bot" target="_blank" rel="noopener">RAG QA bot<span class="arrow" aria-hidden="true">&#8599;</span></a></h3>
        <p>A Python QA bot with hybrid retrieval using BM25 and DPR. It integrates GPT-3.5-turbo, Phi-2 and Llama 3, with contextual compression to cut hallucinations.</p>
        <div class="tile-metrics">
          <div><b>40%</b><span>higher accuracy than traditional search</span></div>
          <div><b>60%</b><span>fewer hallucinations</span></div>
        </div>
        <ul class="tags"><li>RAG</li><li>LangChain</li><li>BM25</li><li>DPR</li><li>LLMs</li></ul>
      </article>

      <article class="tile s5">
        <h3><a href="https://github.com/dasdristanta13/2.5D-Visual-Sound" target="_blank" rel="noopener">2.5D Visual Sound<span class="arrow" aria-hidden="true">&#8599;</span></a></h3>
        <img class="shot" src="images/ML_Project_report.png" loading="lazy" alt="Project report figure for 2.5D Visual Sound">
        <p>Converts monaural audio to binaural by using the video, giving listeners a 3D sound sensation.</p>
        <ul class="tags"><li>Audio processing</li><li>Computer vision</li><li>Deep learning</li></ul>
      </article>

      <article class="tile s4">
        <h3><a href="https://github.com/dasdristanta13/NLP_work/tree/main/Topic_modelling" target="_blank" rel="noopener">Topic modelling of NLP repositories<span class="arrow" aria-hidden="true">&#8599;</span></a></h3>
        <img class="shot" src="images/Topic_modelling.png" loading="lazy" alt="Topic model visualization of popular NLP repositories">
        <p>Uses the GitHub API and spaCy to see how NLP libraries are used across the community.</p>
        <ul class="tags"><li>Topic modeling</li><li>GitHub API</li><li>spaCy</li></ul>
      </article>

      <article class="tile s4">
        <h3><a href="https://github.com/dasdristanta13/NLP_work/tree/main/Resume_Analysis" target="_blank" rel="noopener">Resume analysis with spaCy<span class="arrow" aria-hidden="true">&#8599;</span></a></h3>
        <p>A resume scoring system that evaluates and ranks candidates against job requirements using spaCy.</p>
        <ul class="tags"><li>NLP</li><li>Information extraction</li><li>spaCy</li></ul>
      </article>

      <article class="tile s4">
        <h3><a href="https://github.com/dasdristanta13/Bankruptcy_LDA" target="_blank" rel="noopener">Bankruptcy prediction with LDA<span class="arrow" aria-hidden="true">&#8599;</span></a></h3>
        <img class="shot" src="images/Rplot4.png" loading="lazy" alt="Linear discriminant analysis plot for bankruptcy prediction">
        <p>Linear Discriminant Analysis with dimensionality reduction to predict financial distress in companies.</p>
        <ul class="tags"><li>LDA</li><li>Statistical modeling</li><li>Classification</li></ul>
      </article>

      <article class="tile s7">
        <h3><a href="https://github.com/dasdristanta13/Time-series" target="_blank" rel="noopener">Financial time-series forecasting<span class="arrow" aria-hidden="true">&#8599;</span></a></h3>
        <img class="shot" src="images/Nifty_Forecast.png" loading="lazy" alt="ARIMA forecast chart for the Nifty 50 index">
        <p>ARIMA forecasts for major global indices: Nifty 50, DAX, Dow Jones and Nikkei.</p>
        <ul class="tags"><li>Time series</li><li>ARIMA</li><li>Financial analysis</li></ul>
      </article>

      <article class="tile s5">
        <h3><a href="https://github.com/dasdristanta13/Fifa21EDA/blob/main/README.md" target="_blank" rel="noopener">FIFA 21 data analysis<span class="arrow" aria-hidden="true">&#8599;</span></a></h3>
        <img class="shot" src="images/football.png" loading="lazy" alt="FIFA 21 player statistics chart">
        <p>Player attributes, market values and performance across positions and nationalities.</p>
        <ul class="tags"><li>EDA</li><li>Sports analytics</li><li>Python</li></ul>
      </article>

      <article class="tile s12 wide">
        <img class="shot" src="images/zomato.png" loading="lazy" alt="Zomato restaurant data analysis chart">
        <div class="copy">
          <h3><a href="https://github.com/dasdristanta13/Zomato_Food_EDA" target="_blank" rel="noopener">Zomato food data analysis<span class="arrow" aria-hidden="true">&#8599;</span></a></h3>
          <p>Analysis of Zomato restaurant and delivery data covering customer preferences, pricing strategy and ratings.</p>
          <ul class="tags"><li>Data visualization</li><li>R and Python</li><li>Business intelligence</li></ul>
        </div>
      </article>
    </div>
  </div>
</section>

<section class="section" id="experience">
  <div class="wrap">
    <div class="section-head">
      <h2>Experience</h2>
    </div>

    <div class="role-row">
      <div>
        <h3>Genpact</h3>
        <p class="place">Bengaluru, Karnataka</p>
        <p class="period">Apr 2025 &ndash; Present</p>
      </div>
      <div>
        <p class="role-title">Senior Data Scientist</p>
        <ul>
          <li>Architected and deployed the conversational analytics (Text-to-SQL) platform on LangChain and LangGraph, used by 50+ beta users across 10 concurrent sessions.</li>
          <li>Engineered the agentic workflows behind it: state management, error handling and dynamic routing, scaled to 12+ cross-functional teams.</li>
          <li>Led the automated invoice-processing pipeline on LangChain and Azure OpenAI. Results for both systems are in <a href="#work">Production systems</a>.</li>
        </ul>
      </div>
    </div>

    <div class="role-row">
      <div>
        <h3>UST</h3>
        <p class="place">Kolkata, West Bengal</p>
        <p class="period">Jul 2022 &ndash; Mar 2025</p>
      </div>
      <div>
        <p class="role-title">Associate III Data Scientist <small>Oct 2022 &ndash; Mar 2025</small></p>
        <ul>
          <li>Developed a client-facing provider search system with NLP and open-source LLMs, boosting search efficiency by 30% and speeding data-preparation tasks by 40%.</li>
          <li>Implemented NER and semantic (vector-based) search to map layperson language to medical terms, improving operational efficiency by 25%.</li>
        </ul>
        <p class="role-title">Associate II Data Scientist <small>Jul 2022 &ndash; Sep 2022</small></p>
        <ul>
          <li>Evaluated patient data in BigQuery, improving the client's understanding of adherence drivers by 45% across 10,000+ patients.</li>
          <li>Designed a data anomaly-detection system for categorical healthcare data, in line with HIPAA and GDPR.</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section class="section" id="skills">
  <div class="wrap">
    <div class="section-head">
      <h2>Skills</h2>
    </div>
    <dl class="skills">
      <div><dt>AI and ML</dt><dd>NLP, LLMs, NER, RAG, agentic AI, machine learning, deep learning, statistical modeling</dd></div>
      <div><dt>Frameworks</dt><dd>LangChain, LangGraph, PyTorch, Hugging Face, scikit-learn, XGBoost, FastAPI, spaCy</dd></div>
      <div><dt>Tools and cloud</dt><dd>Python, R, SQL, Git, Docker, BigQuery, vector databases, AWS, Azure (Azure OpenAI)</dd></div>
      <div><dt>Design and governance</dt><dd>Architecture design, data-flow modeling, UML, anomaly detection, HIPAA and GDPR compliance</dd></div>
    </dl>
  </div>
</section>
