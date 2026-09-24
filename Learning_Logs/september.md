# 📓 Daily Learning Log — September 2026

---

### 🗓️ Date: September 24, 2026

**📈 Core Learning: SQL (Product Analytics & Platform Integrity)**

* **Topic:** Relational Schema Architecture, Growth Metrics & Fraud Detection
* **Resource:** Instagram Database Clone (`Instagram-database-clone`)
* **Key Takeaway:** Restructured raw relational dumps into a modular production architecture (`01_schema_and_data_seed.sql` and `02_product_analytics_suite.sql`). Formulated product analytics queries analyzing user churn dormancy via `LEFT JOIN` anti-joins, content virality rankings, platform liquidity (creator conversion rate), and trust-and-safety bot detection using dynamic subqueries (`HAVING COUNT(likes) = total_photos`).

**⌨️ Skill Practice**

* **Focus:** Multi-Repository Workspace Management & Remote Tracking
* **Resource:** Windows PowerShell
* **Duration:** 30 Minutes
* **Key Takeaway:** Diagnosed and corrected nested submodule tracking within the master workspace (`Data Analyst Projects`) by removing root Git tracking, establishing clean subfolder isolation, and deploying standalone remote repositories to GitHub.

---

### 🗓️ Date: September 23, 2026

**📊 Core Learning: SQL (Operations & Logistics Analytics)**

* **Topic:** Star Schema Architecture & Operational Friction Analysis
* **Resource:** Ride-Share Operations Project (`rideshare-operations-analysis`)
* **Key Takeaway:** Designed and implemented a Kimball dimensional model (`fact_trips`, `dim_drivers`, `dim_zones`) with explicit constraints and indexing. Authored advanced analytics queries utilizing Common Table Expressions (CTEs), window functions (`DENSE_RANK`, `NTILE`), and conditional aggregations to isolate dispatch bottlenecks, surge multiplier price elasticity, and platform revenue leakage ($1.0M friction loss).

**⌨️ Skill Practice**

* **Focus:** Git Version Control & Production DDL Deployment
* **Resource:** Windows PowerShell & GitHub CLI
* **Duration:** 30 Minutes
* **Key Takeaway:** Resolved MySQL `DATETIME` syntax conflicts and CRLF staging warnings, establishing clean commit practices and publishing the end-to-end reproducible repository to GitHub.

---

### 🗓️ Date: September 22, 2026

**📊 Core Learning: Power BI & DAX Modeling**

* **Topic:** Operational Dashboard Architecture, Secondary Dual-Axis Scaling & Cross-Filter Contexts
* **Resource:** Ride-Share Operations Project Build (Power BI Desktop)
* **Key Takeaway:** Hardcoded filter contexts inside `CALCULATE` measures (such as `trip_status = "Completed"`) actively overwrite external visual interactions. Utilizing dynamic row counts (`Total Requests`) preserves interactive cross-filtering across categorical slices like cancellation reasons. Properly anchoring secondary Y-axis scales prevents normal operational variance from presenting as false system volatility.

**⌨️ Skill Practice**

* **Focus:** Visual Hierarchy & Report Canvas Layout
* **Resource:** Power BI Desktop Visual Styling
* **Duration:** 45 Minutes
* **Key Takeaway:** Standardized a cohesive enterprise aesthetic across multiple pages using muted neutral backgrounds (`#F4F5F7`), uniform slate tones for volume distributions, and high-contrast alert colors for dropped-demand indicators.

---

### 🗓️ Date: September 21, 2026

**📊 Core Learning: DAX & Business Logic Engineering**

* **Topic:** Operational Friction Metrics & Conditional Filtering
* **Resource:** Power BI Desktop (`rideshare_operations_dashboard.pbix`)
* **Key Takeaway:** Engineered advanced business logic to quantify dispatch breakdowns (`Lost Gross Revenue`, `Cancellation Rate %`) using `CALCULATE` and `SUMX` iterations over surge-multiplied base fares to accurately price lost passenger bookings across dropped trip statuses.

**⌨️ Skill Practice**

* **Focus:** Canvas Scaffolding & Multi-Page UX
* **Resource:** Power BI Visual Layout Engine
* **Duration:** 35 Minutes
* **Key Takeaway:** Established a clear visual boundary between executive commercial health (Page 1) and friction root causes (Page 2), scoping visual interaction filters and preparing dynamic measure bindings across card strips and slicers.

---

### 🗓️ Date: September 20, 2026

**📊 Core Learning: Power BI & Dimensional Modeling**

* **Topic:** Kimball Star Schema Architecture & Baseline DAX Measures
* **Resource:** Power BI Desktop Model View
* **Key Takeaway:** Constructed a clean star schema with 1-to-many, single-direction relationships radiating from dimension tables into `fact_trips`. Formatted a dedicated `_Measures` table housing foundational DAX calculations (`Gross Bookings`, `Fulfillment Rate %`, and `Take Rate %`) while adhering to explicit DAX measure design rather than implicit aggregations.

**⌨️ Skill Practice**

* **Focus:** DAX Syntax & Error Handling
* **Resource:** DAX Formatter / Power BI Modeling Tools
* **Duration:** 30 Minutes
* **Key Takeaway:** Utilized `DIVIDE()` with explicit zero-handling parameters across all rate computations to prevent null display artifacts and runtime divide-by-zero exceptions during report filtering.

---

### 🗓️ Date: September 19, 2026

**🐬 Core Learning: SQL & Relational Analytics**

* **Topic:** Window Functions, CTEs & Revenue Leakage Queries
* **Resource:** `ride_share_operations_analysis.sql`
* **Key Takeaway:** Authored production-grade relational queries utilizing CTEs and ranking window functions (`DENSE_RANK() OVER (PARTITION BY ...)`) to isolate peak-hour dispatch deficits and calculate opportunity loss by municipal sector. Cleaned up duplicate fact table definitions to ensure deterministic join behavior.

**⌨️ Skill Practice**

* **Focus:** Query Optimization & Execution Logic
* **Resource:** SQL Query Workspace
* **Duration:** 40 Minutes
* **Key Takeaway:** Structured filtering predicates inside CTE stages prior to aggregation, preventing accidental Cartesian products during multi-table joins and optimizing scan efficiency across ride records.

---

### 🗓️ Date: September 18, 2026

**🐍 Core Learning: Python & Data Simulation**

* **Topic:** Synthetic Relational Pipeline & Distribution Modeling
* **Resource:** `scripts/generate_data.py` (Local Build)
* **Key Takeaway:** Modeled peak and off-peak trip distributions using weighted categorical sampling in NumPy and Pandas to simulate realistic urban dispatch bottlenecks across relational dimensions (`dim_zones`, `dim_drivers`, `fact_trips`). Ensured foreign key referential integrity between zone classifications and driver fleet entities.

**⌨️ Skill Practice**

* **Focus:** Vectorized Operations & Script Optimization
* **Resource:** VS Code / Python Documentation
* **Duration:** 45 Minutes
* **Key Takeaway:** Replaced iterative row generation loops with vectorized Pandas distributions, cutting synthetic batch creation time across 15,000 records while preserving realistic variance in pricing multipliers and trip status weights.

---

### 🗓️ Date: September 17, 2026

**🛠️ Core Learning: Git Infrastructure & Power BI Schema Architecture**

* **Topic:** Remote Version Control Flushing & Star-Schema Data Modeling
* **Resource:** Git CLI & Power BI Desktop
* **Key Takeaway:** Restructured remote commit tracking to maintain a clean, authentic project history, configured 1-to-many star-schema relationships, and drafted primary DAX operational metrics for dashboard visualization.

**⌨️ Skill Practice**

* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 15 Minutes
* **Key Takeaway:** Preserved high accuracy and consistent mechanical execution.

---

### 🗓️ Date: September 16, 2026

**📊 Core Learning: Python Data Engineering & Schema Design**

* **Topic:** Relational Synthetic Data Pipeline & Dispatch Logic
* **Resource:** Custom Python Pipeline (`generate_data.py`) & SQL Architecture Design
* **Key Takeaway:** Programmed automated generation of relational datasets (`dim_zones`, `dim_drivers`, `fact_trips`) incorporating surge multipliers, realistic take-rates, and cancellation friction while resolving OS-level relative path handling.

**⌨️ Skill Practice**

* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 15 Minutes
* **Key Takeaway:** Maintained baseline typing cadence and muscle memory.

---

### 🗓️ Date: September 15, 2026

**🔄 Core Learning: Workflow Calibration & Portfolio Strategy**

* **Topic:** Strategic Curriculum Pivot & Project Roadmap Definition
* **Resource:** Professional Career Transition Strategy
* **Key Takeaway:** Audited the current learning curriculum and executed a strategic pivot, pruning non-essential web development tracks to concentrate 100% of execution bandwidth on high-value data analytics portfolio assets (SQL, Power BI, and advanced Pandas data models).

**⌨️ Skill Practice**

* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 15 Minutes
* **Key Takeaway:** Maintained baseline mechanical touch-typing execution during operational planning and workflow realignment.

---

### 🗓️ Date: September 14, 2026

**🧘 Core Learning: Scheduled Rest & Cultural Observance**
* **Topic:** Holiday Observance & Scheduled Reset
* **Resource:** N/A (Personal Day)
* **Key Takeaway:** Observed the holiday quietly and took a planned low-friction day away from active screen time to recharge mental bandwidth ahead of upcoming technical sprints.

**⌨️ Skill Practice**
* **Focus:** Rest & Recovery
* **Resource:** N/A
* **Duration:** 0 Minutes
* **Key Takeaway:** Paused daily keyboard drills for scheduled holiday reset.

---

### 🗓️ Date: September 13, 2026

**🧘 Core Learning: Scheduled Rest & Recovery**
* **Topic:** Weekend Recovery & Mental Bandwidth Recharge
* **Resource:** N/A (Rest Day)
* **Key Takeaway:** Took a planned Sunday rest day to decompress after intensive communication recording sessions and clear mental bandwidth ahead of the upcoming week's technical coding blocks.

**⌨️ Skill Practice**
* **Focus:** Rest & Recovery
* **Resource:** N/A
* **Duration:** 0 Minutes
* **Key Takeaway:** Scheduled weekend break from daily keyboard drills to support full cognitive and physical reset.

---

### 🗓️ Date: September 12, 2026

**🗣️ Core Learning: Professional Communication & Video Pitch Delivery**
* **Topic:** High-Stakes Scenario Framing, On-Camera Delivery, Body Language (Gesture Integration), and Unscripted Technical Self-Introductions
* **Resource:** The Complete Communication Skills Master Class for Life (TJ Walker) & Self-Recording Video Practice
* **Key Takeaway:** Executed iterative on-camera speaking drills (8 recorded takes) applying the high-stakes scenario hook for a data analyst introduction. Overcame word-for-word memorization stalls by speaking to core concepts, eliminated duplicate opening greetings for a sharper pivot into identity, incorporated natural hand gestures to release shoulder tension, and sustained locked lens eye contact to deliver a confident, conversational 45-second value proposition.

**⌨️ Skill Practice**
* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 10 Minutes
* **Key Takeaway:** Maintained daily touch-typing baseline consistency alongside video recording drills.

---

### 🗓️ Date: September 11, 2026

**📋 Core Learning: Personal Leave**
* **Topic:** Personal Commitments & Transition Back to Workflow
* **Resource:** N/A (Personal Leave)
* **Key Takeaway:** Concluded a multi-day personal leave window; finalized off-desk commitments and established scheduling priorities to prepare for technical workflow re-entry.

**⌨️ Skill Practice**
* **Focus:** Scheduled Rest
* **Resource:** N/A
* **Duration:** 0 Minutes
* **Key Takeaway:** Paused keyboard practice during personal leave.

---

### 🗓️ Date: September 10, 2026

**📋 Core Learning: Personal Leave**
* **Topic:** Scheduled Personal Leave
* **Resource:** N/A (Personal Leave)
* **Key Takeaway:** Stepped away from development modules to attend to planned personal and family responsibilities.

**⌨️ Skill Practice**
* **Focus:** Scheduled Rest
* **Resource:** N/A
* **Duration:** 0 Minutes
* **Key Takeaway:** Paused typing practice during personal leave.

---

### 🗓️ Date: September 09, 2026

**📋 Core Learning: Personal Leave**
* **Topic:** Scheduled Personal Leave
* **Resource:** N/A (Personal Leave)
* **Key Takeaway:** Allocated time away from study sprints to manage off-desk family matters.

**⌨️ Skill Practice**
* **Focus:** Scheduled Rest
* **Resource:** N/A
* **Duration:** 0 Minutes
* **Key Takeaway:** Paused typing practice during personal leave.

---

### 🗓️ Date: September 08, 2026

**📋 Core Learning: Personal Leave**
* **Topic:** Unscheduled Personal Leave & Travel
* **Resource:** N/A (Personal Leave)
* **Key Takeaway:** Paused technical study blocks to manage sudden personal commitments and related travel.

**⌨️ Skill Practice**
* **Focus:** Scheduled Rest
* **Resource:** N/A
* **Duration:** 0 Minutes
* **Key Takeaway:** Paused typing practice due to unscheduled personal leave.

---

### 🗓️ Date: September 07, 2026

**🕷️ Core Learning: Python & Web Scraping (Beautiful Soup 4)**
* **Topic:** HTML Parsing (`html.parser`), DOM Tree Traversal (`find`, `find_all`, `select`), CSS Selectors, Live Web Scraping (Hacker News), and Archival Data Ingestion (Empire 100 Movies)
* **Resource:** Python Study Curriculum (Day 45: Web Scraping with Beautiful Soup)
* **Key Takeaway:** Learned how to extract unstructured web data and transform it into clean datasets using Beautiful Soup 4 and Requests. Practiced navigating DOM hierarchies using tag names and CSS selectors (`.select_one()`), scraped live articles and upvotes from Y Combinator Hacker News, and built an automated scraper that pulls archival ranking data from the Wayback Machine to generate a clean, sequentially ordered text file.

**⌨️ Skill Practice**
* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 10 Minutes
* **Key Takeaway:** Maintained baseline typing consistency and accuracy while navigating tag extraction syntax, nested loops, and file I/O operations.

---

### 🗓️ Date: September 06, 2026

**🧘 Core Learning: Scheduled Rest & Recovery**
* **Topic:** Weekend Recovery & Cognitive Recharge
* **Resource:** N/A (Rest Day)
* **Key Takeaway:** Took a planned Sunday rest day to step away from the desk, recharge mental bandwidth, and reset focus ahead of incoming web scraping and data extraction pipelines.

**⌨️ Skill Practice**
* **Focus:** Rest & Recovery
* **Resource:** N/A
* **Duration:** 0 Minutes
* **Key Takeaway:** Scheduled weekend break from daily keyboard drills to support full mental and physical recovery.

---

### 🗓️ Date: September 05, 2026

**🎨 Core Learning: CSS & Web Styling**
* **Topic:** CSS Layout Mechanics, Selectors & Visual Design
* **Resource:** Web Development Bootcamp (CSS Styling Modules)
* **Key Takeaway:** Practiced fundamental CSS rules and styling mechanisms to manipulate page structure, refine element alignment, and reinforce clean styling architecture for web applications.

**🗣️ Core Learning: Communication Skills**
* **Topic:** Quick Communication Tactics, Message Framing & Delivery
* **Resource:** The Complete Communication Skills Master Class for Life
* **Key Takeaway:** Reviewed actionable, high-impact communication strategies centered on verbal clarity, direct message framing, active listening, and reducing communicative friction in everyday interactions.

**⌨️ Skill Practice**
* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 10 Minutes
* **Key Takeaway:** Maintained daily touch-typing rhythm and muscle memory alongside frontend styling drills and communication review.

---

### 🗓️ Date: September 04, 2026

**🎨 Core Learning: CSS3 & Box Model Architecture**
* **Topic:** CSS Box Model (Margins, Padding, Borders), Typography & Font Properties, Color Models (RGB, Hex, Named), DevTools CSS Inspection & Layout Debugging (Pesticide)
* **Resource:** Web Development Bootcamp (Day 44: CSS Box Model & Motivational Poster Project)
* **Key Takeaway:** Mastered foundational CSS layout mechanics centered on the Box Model, configuring content dimensions, interior padding, structural borders, and exterior margin spacing. Explored color systems (RGB, Hex, named values), customized typography using web fonts and CSS font properties, used Chrome DevTools and Pesticide to inspect layout box calculations, and integrated these concepts to build and center a responsive motivational poster webpage.

**⌨️ Skill Practice**
* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 10 Minutes
* **Key Takeaway:** Maintained daily touch-typing execution baseline alongside CSS property-value drafting and layout debugging.

---

### 🗓️ Date: September 03, 2026

**🤝 Core Learning: Professional Networking & Industry Analysis**
* **Topic:** Tech Market Dynamics, Workforce Volatility & Skill Hedging
* **Resource:** Professional Peer Discussion & Industry Analysis
* **Key Takeaway:** Dedicated the session to evaluating corporate restructuring trends and tech workforce movements through peer dialogue. Reinforced the strategic priority of technical independence, hands-on portfolio engineering, and cross-functional data skillsets in mitigating broader employment market risks.

**⌨️ Skill Practice**
* **Focus:** Professional Development
* **Resource:** N/A
* **Duration:** 0 Minutes
* **Key Takeaway:** Paused keyboard practice for scheduled professional discussions and industry evaluation.

---

### 🗓️ Date: September 02, 2026

**🎨 Core Learning: HTML5 & CSS3 Fundamentals**
* **Topic:** Semantic HTML (Lists, Nesting, Anchor Tags, Image Elements) & CSS Core (Syntax, Selectors, Styling & Color Vocab Project)
* **Resource:** Web Development Bootcamp (Days 42 & 43: Birthday Invite & Color Vocab Projects)
* **Key Takeaway:** Expanded HTML proficiency by mastering ordered/unordered lists, indentation nesting hierarchy, hyperlinks (`<a>`), and relative/absolute image paths (`<img>`) in the Birthday Invite project. Progressed into CSS fundamentals, implementing external stylesheets, class vs. element selectors, and CSS color vocabularies to transition from raw structural markup to responsive visual design.

**⌨️ Skill Practice**
* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 10 Minutes
* **Key Takeaway:** Maintained clean touch-typing rhythm alongside rapid syntax drafting across HTML tags and CSS property blocks.

---

### 🗓️ Date: September 01, 2026

**🌐 Core Learning: HTML5 & Web Fundamentals**
* **Topic:** Document Structuring, Heading Hierarchy (`<h1>`–`<h6>`), Paragraph Blocks (`<p>`), Void Elements (`<hr/>`), and Live Server Workflow
* **Resource:** Web Development Bootcamp (HTML Fundamentals: Movie Ranking Project)
* **Key Takeaway:** Began frontend fundamentals by constructing semantic HTML pages. Established structured information architecture using proper heading hierarchies, section dividers via self-closing void elements, and verified layout rendering using the local VS Code Live Preview environment.

**⌨️ Skill Practice**
* **Focus:** Typing Speed & Accuracy
* **Resource:** Keybr
* **Duration:** 10 Minutes
* **Key Takeaway:** Maintained daily touch-typing practice baseline while transitioning into web development markup.

---
