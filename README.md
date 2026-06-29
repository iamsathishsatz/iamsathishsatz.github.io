
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sathishbabu SG - BI & Analytics Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }
        
        header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 20px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }
        
        header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }
        
        header p {
            font-size: 1.2em;
            margin-bottom: 15px;
            opacity: 0.95;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
            font-size: 0.95em;
            margin-top: 20px;
        }
        
        .contact-info a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
        }
        
        .contact-info a:hover {
            opacity: 0.8;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        section {
            background: white;
            margin: 30px 0;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        h2 {
            color: #667eea;
            font-size: 1.8em;
            margin-bottom: 25px;
            border-bottom: 3px solid #667eea;
            padding-bottom: 10px;
        }
        
        h3 {
            color: #764ba2;
            font-size: 1.3em;
            margin-top: 20px;
            margin-bottom: 10px;
        }
        
        .summary-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .stat-box {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 25px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(102, 126, 234, 0.3);
        }
        
        .stat-box .number {
            font-size: 2em;
            font-weight: bold;
            margin-bottom: 5px;
        }
        
        .stat-box .label {
            font-size: 0.95em;
            opacity: 0.95;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .skill-category {
            background: #f8f9ff;
            padding: 20px;
            border-radius: 8px;
            border-left: 4px solid #667eea;
        }
        
        .skill-category h4 {
            color: #667eea;
            margin-bottom: 10px;
            font-size: 1.05em;
        }
        
        .skill-category ul {
            list-style: none;
        }
        
        .skill-category li {
            padding: 5px 0;
            padding-left: 20px;
            position: relative;
        }
        
        .skill-category li:before {
            content: "→";
            position: absolute;
            left: 0;
            color: #667eea;
            font-weight: bold;
        }
        
        .projects-container {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
        }
        
        .project-card {
            border: 1px solid #e0e0e0;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        }
        
        .project-header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 20px;
        }
        
        .project-header h3 {
            margin: 0 0 10px 0;
            color: white;
            font-size: 1.4em;
        }
        
        .project-meta {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            font-size: 0.9em;
            opacity: 0.9;
        }
        
        .meta-item {
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        .project-content {
            padding: 25px;
        }
        
        .project-description {
            margin-bottom: 20px;
            line-height: 1.8;
        }
        
        /* Image Placeholder Styling */
        .image-placeholder {
            width: 100%;
            height: 350px;
            margin: 20px 0;
            border-radius: 8px;
            border: 2px dashed #667eea;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, #f0f4ff 0%, #e8f0ff 100%);
            flex-direction: column;
            gap: 10px;
            color: #667eea;
            font-size: 1em;
            text-align: center;
            padding: 20px;
            position: relative;
        }
        
        .image-placeholder.filled {
            border: 1px solid #e0e0e0;
            background: transparent;
        }
        
        .image-placeholder.filled img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 6px;
        }
        
        .placeholder-icon {
            font-size: 3em;
            opacity: 0.5;
        }
        
        .placeholder-text {
            font-size: 0.9em;
            opacity: 0.7;
        }
        
        .project-metrics {
            background: #f8f9ff;
            padding: 20px;
            border-radius: 6px;
            margin: 20px 0;
        }
        
        .metrics-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
        }
        
        .metric {
            text-align: center;
        }
        
        .metric-value {
            font-size: 1.6em;
            font-weight: bold;
            color: #667eea;
        }
        
        .metric-label {
            font-size: 0.85em;
            color: #666;
            margin-top: 5px;
        }
        
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 15px 0;
        }
        
        .tech-tag {
            background: #e0e7ff;
            color: #667eea;
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.85em;
            font-weight: 500;
        }
        
        .impact-list {
            list-style: none;
            margin: 15px 0;
        }
        
        .impact-list li {
            padding: 10px 0;
            padding-left: 30px;
            position: relative;
            line-height: 1.6;
        }
        
        .impact-list li:before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #667eea;
            font-weight: bold;
            font-size: 1.2em;
        }
        
        .experience-timeline {
            position: relative;
            padding: 20px 0;
        }
        
        .timeline-item {
            display: flex;
            margin-bottom: 30px;
            position: relative;
        }
        
        .timeline-marker {
            width: 20px;
            height: 20px;
            background: #667eea;
            border-radius: 50%;
            margin-right: 30px;
            margin-top: 5px;
            flex-shrink: 0;
            border: 3px solid white;
            box-shadow: 0 0 0 3px #667eea;
        }
        
        .timeline-item:not(:last-child)::before {
            content: '';
            position: absolute;
            left: 8px;
            top: 40px;
            width: 3px;
            height: calc(100% + 20px);
            background: #e0e0e0;
        }
        
        .timeline-content h4 {
            color: #667eea;
            margin-bottom: 5px;
            font-size: 1.1em;
        }
        
        .timeline-content .role {
            color: #764ba2;
            font-weight: 600;
            margin-bottom: 5px;
        }
        
        .timeline-content .date {
            color: #999;
            font-size: 0.9em;
            margin-bottom: 10px;
        }
        
        .certifications {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
        }
        
        .cert {
            background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%);
            padding: 15px;
            border-radius: 6px;
            border-left: 4px solid #667eea;
        }
        
        .cert-title {
            font-weight: 600;
            color: #667eea;
            margin-bottom: 5px;
        }
        
        .cert-issuer {
            font-size: 0.85em;
            color: #666;
        }
        
        footer {
            text-align: center;
            padding: 20px;
            color: #666;
            margin-top: 40px;
        }
        
        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 12px 30px;
            border-radius: 25px;
            text-decoration: none;
            margin-top: 10px;
            transition: transform 0.3s, box-shadow 0.3s;
            font-weight: 600;
        }
        
        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(102, 126, 234, 0.4);
        }
        
        .info-box {
            background: #e3f2fd;
            border-left: 4px solid #2196F3;
            padding: 15px;
            border-radius: 6px;
            margin: 15px 0;
            font-size: 0.95em;
        }
        
        @media (max-width: 768px) {
            header h1 {
                font-size: 1.8em;
            }
            
            .contact-info {
                gap: 15px;
            }
            
            section {
                padding: 25px;
            }
            
            .project-meta {
                gap: 10px;
            }
            
            .image-placeholder {
                height: 250px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Sathishbabu Selkan Gopinath</h1>
        <p>Lead BI & Analytics Architect</p>
        <p style="font-size: 1em; opacity: 0.85;">Enterprise Data Intelligence | Business Analytics | Data Visualization</p>
        <div class="contact-info">
            <a href="tel:+971503942305">📱 +971 50 394 2305</a>
            <a href="mailto:sathishbabu.s.g@gmail.com">✉️ sathishbabu.s.g@gmail.com</a>
            <a href="https://linkedin.com/in/sathishbabusg" target="_blank">🔗 LinkedIn Profile</a>
            <a href="https://dubai.com">📍 Dubai, UAE</a>
        </div>
    </header>

    <div class="container">
        <!-- Professional Summary -->
        <section>
            <h2>Professional Snapshot</h2>
            <div class="summary-grid">
                <div class="stat-box">
                    <div class="number">15+</div>
                    <div class="label">Years of Enterprise BI Experience</div>
                </div>
                <div class="stat-box">
                    <div class="number">4+</div>
                    <div class="label">BI Platforms Mastered</div>
                </div>
                <div class="stat-box">
                    <div class="number">100%</div>
                    <div class="label">Client Satisfaction Track Record</div>
                </div>
                <div class="stat-box">
                    <div class="number">5K+</div>
                    <div class="label">Active Users Supported</div>
                </div>
            </div>
            <p style="font-size: 1.05em; line-height: 1.8;">
                Results-driven BI & Analytics Professional delivering enterprise-grade reporting, interactive dashboards, and data visualization solutions that transform complex data into actionable business insights. Proven expertise in designing scalable, security-first analytics platforms that drive strategic decision-making across Banking, Financial Services, and Technology domains. Adept at translating business requirements into intelligent, self-service analytics solutions with exceptional performance optimization and governance standards.
            </p>
        </section>

        <!-- Featured Projects -->
        <section>
            <h2>Featured Projects</h2>
            <div class="projects-container">
                
                <!-- Project 1: Marketing Abandonment Retargeting -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Marketing Abandonment Retargeting Dashboard</h3>
                        <div class="project-meta">
                            <span class="meta-item">📊 Tableau</span>
                            <span class="meta-item">🏦 Banking & Financial Services</span>
                            <span class="meta-item">⚡ Real-time Monitoring</span>
                        </div>
                    </div>
                    <div class="project-content">
                        <div class="project-description">
                            <strong>Challenge:</strong> The business needed real-time visibility into customer account abandonment patterns across multiple channels (Web, Android, iOS) to enable targeted retargeting campaigns and improve customer retention.
                        </div>
                        
                         <div class="placeholder-text">Project Dashboard Screenshot</div>
                            <div class="placeholder-text" style="font-size: 0.8em; opacity: 0.5;"><img width="2188" height="1468" alt="Portfolio Abondanor" src="https://github.com/user-attachments/assets/e618fd39-4ecf-4664-8f3c-ffdc2c227f77" />
</div>
                        </div>
                        
                        <div class="project-description">
                            <strong>Solution:</strong> Architected a comprehensive Tableau dashboard providing:
                        </div>
                        
                        <ul class="impact-list">
                            <li>Real-time abandonment tracking across multiple channels (Web, Mobile, App, etc.) with drill-down capabilities</li>
                            <li>Multi-dimensional analysis: total abandons, abandon accounts, and engagement metrics by segment</li>
                            <li>Email campaign performance metrics (sent, bounced, opened, clicked) with comparative trend analysis</li>
                            <li>Business transaction funnel analysis showing conversion rates and financial impact</li>
                            <li>Partner-level filtering and campaign segmentation for targeted optimization</li>
                            <li>Interactive visualizations (donut charts, KPI scorecards, trend lines) enabling stakeholders to identify high-abandonment segments</li>
                        </ul>
                        
                        <div class="tech-stack">
                            <span class="tech-tag">Tableau</span>
                            <span class="tech-tag">Advanced SQL</span>
                            <span class="tech-tag">Data Modeling</span>
                            <span class="tech-tag">Real-time Analytics</span>
                            <span class="tech-tag">Dashboard Design</span>
                            <span class="tech-tag">Performance Optimization</span>
                        </div>
                        
                        <div class="project-description" style="margin-top: 20px;">
                            <strong>Business Impact:</strong>
                            <ul class="impact-list">
                                <li>Enabled targeted retargeting campaigns with improved email engagement through channel performance insights</li>
                                <li>Improved visibility into abandonment patterns across channels, driving strategic decisions on platform investments</li>
                                <li>Automated reporting process, reducing manual effort and enabling near real-time decision making</li>
                                <li>Provided business transaction monitoring with granular filters for scenario analysis and forecasting</li>
                            </ul>
                        </div>
                    </div>
                </div>

                <!-- Project 2: Credit Card Activation Summary -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Credit Card Application Activation Summary Report</h3>
                        <div class="project-meta">
                            <span class="meta-item">📊 Power BI / Tableau</span>
                            <span class="meta-item">💳 Financial Services</span>
                            <span class="meta-item">📈 Funnel Analysis</span>
                        </div>
                    </div>
                    <div class="project-content">
                        <div class="project-description">
                            <strong>Challenge:</strong> Finance and Product teams needed comprehensive visibility into credit card application activation patterns, time-to-activation, and customer behavior post-activation to optimize onboarding processes and improve product performance.
                        </div>
                        
                        <!-- Image Placeholder -->
                        <div class="image-placeholder">
                            <div class="placeholder-icon">💳</div>
                            <div class="placeholder-text">Activation Analysis Dashboard</div>
                            <div class="placeholder-text" style="font-size: 0.8em; opacity: 0.5;"><img width="2447" height="1379" alt="Portfolio Activation Summary" src="https://github.com/user-attachments/assets/be9fec8c-4837-4e42-b763-b34bc0e93fec" />
</div>
                        </div>
                        
                        <div class="info-box">
                            <strong>ℹ️ Image Placeholder:</strong> This space is reserved for your actual Power BI or Tableau dashboard screenshot. Replace with your actual project image.
                        </div>
                        
                        <div class="project-description">
                            <strong>Solution:</strong> Developed a comprehensive multi-dimensional analysis report featuring:
                        </div>
                        
                        <ul class="impact-list">
                            <li>End-to-end activation funnel with stage-wise drop-off analysis and conversion metrics</li>
                            <li>Time-to-activation analysis showing distribution of customers by activation speed</li>
                            <li>Multi-dimensional funnel with Channel Code, Campaign ID, Cell ID, and OB Channel filtering</li>
                            <li>Credit line analysis with approved credit limits and purchase behavior tracking</li>
                            <li>Decision Month filtering for cohort analysis and temporal trend tracking</li>
                            <li>Interactive visualizations showing activation distribution by time interval and channel</li>
                            <li>Detailed transaction table with purchase amounts and credit line metrics</li>
                        </ul>
                        
                        <div class="tech-stack">
                            <span class="tech-tag">Power BI</span>
                            <span class="tech-tag">Tableau</span>
                            <span class="tech-tag">DAX/MDX</span>
                            <span class="tech-tag">Funnel Analysis</span>
                            <span class="tech-tag">Data Storytelling</span>
                            <span class="tech-tag">Executive Reporting</span>
                        </div>
                        
                        <div class="project-description" style="margin-top: 20px;">
                            <strong>Business Impact:</strong>
                            <ul class="impact-list">
                                <li>Identified activation patterns and bottlenecks in customer onboarding journey</li>
                                <li>Revealed optimization opportunities through time-to-activation analysis by segment</li>
                                <li>Enabled credit line optimization strategies based on purchase behavior patterns</li>
                                <li>Supported cohort analysis for different campaign and channel combinations</li>
                                <li>Provided foundation for predictive models on customer lifecycle and purchase propensity</li>
                            </ul>
                        </div>
                    </div>
                </div>

                <!-- Project 3: Notifications Tubemap -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Payments Notifications & Triggers KPI Tubemap</h3>
                        <div class="project-meta">
                            <span class="meta-item">📊 Tableau</span>
                            <span class="meta-item">🔔 Communication Workflows</span>
                            <span class="meta-item">⚙️ SLA Monitoring</span>
                        </div>
                    </div>
                    <div class="project-content">
                        <div class="project-description">
                            <strong>Challenge:</strong> The business required end-to-end visibility into notification request flows, success/failure tracking, and SLA compliance across multiple communication channels and architectures to ensure reliable customer notification delivery.
                        </div>
                        
                        <!-- Image Placeholder -->
                        <div class="image-placeholder">
                            <div class="placeholder-icon">🔔</div>
                            <div class="placeholder-text">Notification Flow Tubemap</div>
                            <div class="placeholder-text" style="font-size: 0.8em; opacity: 0.5;"><img width="2440" height="1334" alt="Portfolio Notification" src="https://github.com/user-attachments/assets/ef81a980-c3ef-4b09-b29e-4da24dd9db0e" />
</div>
                        </div>
                        
                        <div class="info-box">
                            <strong>ℹ️ Image Placeholder:</strong> This space is reserved for your actual Tableau Tubemap visualization or dashboard screenshot. Replace with your actual project image.
                        </div>
                        
                        <div class="project-description">
                            <strong>Solution:</strong> Developed a sophisticated Tableau Tubemap visualization providing:
                        </div>
                        
                        <ul class="impact-list">
                            <li>End-to-end request flow tracking with dual-architecture routing visibility (modern vs. legacy systems)</li>
                            <li>Real-time success/failure monitoring with conversion-style metrics across request pipeline</li>
                            <li>Granular failure analysis: breakdown by failure type, architecture, and communication channel</li>
                            <li>SLA compliance dashboard: clear visualization of met vs. missed SLA targets</li>
                            <li>Notification-level metrics: detailed tracking from request to delivery confirmation</li>
                            <li>Reconciliation tracking: accuracy metrics and discrepancy identification</li>
                            <li>Multi-dimensional filtering: Partner, Notification Type, Channel, and Request Date range analysis</li>
                        </ul>
                        
                        <div class="tech-stack">
                            <span class="tech-tag">Tableau</span>
                            <span class="tech-tag">Tubemap Visualization</span>
                            <span class="tech-tag">SLA Monitoring</span>
                            <span class="tech-tag">Flow Analytics</span>
                            <span class="tech-tag">KPI Dashboarding</span>
                            <span class="tech-tag">Real-time Monitoring</span>
                        </div>
                        
                        <div class="project-description" style="margin-top: 20px;">
                            <strong>Business Impact:</strong>
                            <ul class="impact-list">
                                <li>Identified critical workflow bottlenecks through visual SLA gap analysis—triggered infrastructure optimization initiatives</li>
                                <li>Revealed notification quality issues through accuracy reconciliation tracking—prioritized process improvements</li>
                                <li>Enabled root cause analysis: distinguished between architecture failures, communication failures, and SLA breaches</li>
                                <li>Provided decision makers with clear visibility into notification workflow health and performance bottlenecks</li>
                                <li>Supported incident response and escalation procedures with real-time KPI monitoring</li>
                            </ul>
                        </div>
                    </div>
                </div>

            </div>
        </section>

        <!-- Core Competencies -->
        <section>
            <h2>Core Competencies</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h4>BI & Analytics Platforms</h4>
                    <ul>
                        <li>Tableau (Server, Desktop, Cloud)</li>
                        <li>Power BI (Advanced DAX, Reporting)</li>
                        <li>QlikSense</li>
                        <li>Cognos Analytics</li>
                        <li>Dashboard Design & Optimization</li>
                    </ul>
                </div>
                
                <div class="skill-category">
                    <h4>Data Engineering & Modeling</h4>
                    <ul>
                        <li>Advanced SQL & Query Optimization</li>
                        <li>ETL/ELT Pipeline Design</li>
                        <li>Star/Snowflake Schema</li>
                        <li>OLAP Cube Development</li>
                        <li>Data Warehousing</li>
                    </ul>
                </div>
                
                <div class="skill-category">
                    <h4>Cloud & Modern Data Platforms</h4>
                    <ul>
                        <li>AWS (S3, Athena, Lambda, Glue)</li>
                        <li>Databricks & Apache Spark</li>
                        <li>PySpark</li>
                        <li>Azure</li>
                        <li>Serverless Architectures</li>
                    </ul>
                </div>
                
                <div class="skill-category">
                    <h4>Databases & Storage</h4>
                    <ul>
                        <li>Oracle & Teradata</li>
                        <li>Microsoft SQL Server</li>
                        <li>Advanced Pass-Through SQL</li>
                        <li>Database Performance Tuning</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>Analytics & AI/ML</h4>
                    <ul>
                        <li>Python (Pandas, NumPy, ScikitLearn)</li>
                        <li>Sentiment Analysis & NLP</li>
                        <li>Market Basket Analysis</li>
                        <li>ML Model Testing</li>
                        <li>AI Agent Support</li>
                    </ul>
                </div>
                
                <div class="skill-category">
                    <h4>Business & Consulting</h4>
                    <ul>
                        <li>KPI Design & Reporting</li>
                        <li>Data Storytelling</li>
                        <li>Stakeholder Management</li>
                        <li>Requirements Analysis</li>
                        <li>Executive Reporting</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Professional Experience -->
        <section>
            <h2>Professional Experience</h2>
            
            <div class="experience-timeline">
                <div class="timeline-item">
                    <div class="timeline-marker"></div>
                    <div class="timeline-content">
                        <h4>Barclays Global Service Center</h4>
                        <div class="role">Assistant Vice President — Data Engineering & Analytics</div>
                        <div class="date">Jul 2022 – Present</div>
                        <p>Leading enterprise BI initiatives for USCB Data Analytics & Insights Team. Designing executive dashboards and KPI reporting solutions for Finance, Credit Risk, and Technology stakeholders. Architecting serverless AWS data platforms integrating REST APIs, Lambda, Glue, Step Functions for automated workflows.</p>
                        <ul style="margin-top: 10px; margin-left: 20px;">
                            <li>Delivered enterprise BI dashboards enabling strategic decision-making for Finance and Credit Risk teams</li>
                            <li>Engineered security-first Partner Portals within Salesforce Community Cloud with embedded Tableau Server visualizations</li>
                            <li>Architected serverless AWS data platform (REST APIs, Lambda, Glue, Step Functions, S3, Athena)</li>
                            <li>Led POCs for Databricks, Looker, and Starburst to modernize analytics ecosystem</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-marker"></div>
                    <div class="timeline-content">
                        <h4>DHL IT Services</h4>
                        <div class="role">Principal Application Support Specialist & BI Solution Architect</div>
                        <div class="date">Jun 2019 – Jul 2022</div>
                        <p>Global Service Owner for DGFF FRP Team, managing infrastructure for 10 parallel critical services with 100% CSAT. Established enterprise reporting standards and directed complex Cognos Analytics upgrade for 5K+ active users.</p>
                        <ul style="margin-top: 10px; margin-left: 20px;">
                            <li>Managed infrastructure capacity planning and risk remediation across mission-critical services</li>
                            <li>Established reporting standards and KPI governance for enterprise-wide decision-making</li>
                            <li>Directed Cognos Analytics infrastructure upgrade (v10.2.1.1 → v11.1.4) with zero business disruption</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-marker"></div>
                    <div class="timeline-content">
                        <h4>Barclays Global Service Center</h4>
                        <div class="role">Assistant Manager — BI Development & Analytics</div>
                        <div class="date">Jan 2016 – Jun 2019</div>
                        <p>Designed and maintained enterprise BI dashboards using Tableau, QlikSense, and Power BI. Developed Python-based Sentiment Analysis and Market Basket Analysis models. Automated Global Revenue Reporting, saving 1.5-2.0 FTE hours per cycle.</p>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-marker"></div>
                    <div class="timeline-content">
                        <h4>Cognizant Technology Solutions</h4>
                        <div class="role">Associate — Projects (BI Developer Lead)</div>
                        <div class="date">Apr 2014 – Dec 2015</div>
                        <p>Led large-scale data warehouse migration from Oracle to Teradata. Performed advanced SQL optimization, impact analysis, data validation, and reporting continuity assessments.</p>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-marker"></div>
                    <div class="timeline-content">
                        <h4>Computer Science Corporation (CSC)</h4>
                        <div class="role">Associate Professional — Measurement Specialist</div>
                        <div class="date">Nov 2009 – Apr 2014</div>
                        <p>Developed semantic business layers, metadata models, and OLAP cubes in Cognos Framework Manager. Resolved critical production issues, query degradation, and cube build failures.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Certifications & Education -->
        <section>
            <h2>Certifications & Education</h2>
            
            <div style="margin-bottom: 40px;">
                <h3>Professional Certifications</h3>
                <div class="certifications">
                    <div class="cert">
                        <div class="cert-title">AWS Certified AI Practitioner</div>
                        <div class="cert-issuer">Amazon Web Services • 2025</div>
                    </div>
                    <div class="cert">
                        <div class="cert-title">AWS Certified Cloud Practitioner</div>
                        <div class="cert-issuer">Amazon Web Services • 2023</div>
                    </div>
                    <div class="cert">
                        <div class="cert-title">Career Essentials in Generative AI</div>
                        <div class="cert-issuer">Microsoft & LinkedIn • 2024</div>
                    </div>
                    <div class="cert">
                        <div class="cert-title">IBM Certified Solution Expert — Cognos Analytics 10</div>
                        <div class="cert-issuer">IBM • Active</div>
                    </div>
                    <div class="cert">
                        <div class="cert-title">ITIL V3 Foundation Certified</div>
                        <div class="cert-issuer">IT Service Management • Active</div>
                    </div>
                </div>
            </div>

            <div>
                <h3>Education</h3>
                <div class="timeline-item" style="margin-bottom: 0;">
                    <div class="timeline-marker"></div>
                    <div class="timeline-content">
                        <h4>Bachelor of Technology (B.Tech) — Computer Science & Engineering</h4>
                        <div class="date">SRM University • 2010 – 2014 • Distinction</div>
                    </div>
                </div>
                <div class="timeline-item" style="margin-bottom: 0;">
                    <div class="timeline-marker"></div>
                    <div class="timeline-content">
                        <h4>Diploma in Electronics & Communication Engineering (ECE)</h4>
                        <div class="date">2006 – 2009</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Call to Action -->
        <section style="text-align: center; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white;">
            <h2 style="color: white; border-color: white;">Ready to Transform Your Data Into Intelligence?</h2>
            <p style="font-size: 1.1em; margin-bottom: 20px;">Let's discuss how I can help your organization make smarter, data-driven decisions through enterprise BI solutions and advanced analytics.</p>
            <a href="mailto:sathishbabu.s.g@gmail.com" class="cta-button" style="background: white; color: #667eea; margin-right: 10px;">Get In Touch</a>
            <a href="https://linkedin.com/in/sathishbabusg" target="_blank" class="cta-button" style="background: rgba(255,255,255,0.2);">View LinkedIn Profile</a>
        </section>
    </div>

    <footer>
        <p>© 2025 Sathishbabu SG | Lead BI & Analytics Architect | Dubai, UAE</p>
        <p style="margin-top: 10px; font-size: 0.9em;">Portfolio showcasing enterprise BI solutions, data visualization, and analytics architecture.</p>
    </footer>
</body>
</html>
