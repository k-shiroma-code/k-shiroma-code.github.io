---
title: Projects
layout: default
permalink: /projects/
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Kyle Shiroma - Data Science & Machine Learning Projects Portfolio">
    <title>Projects | Kyle Shiroma</title>
    <style>
        /* Base styles matching your site template */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.6;
            color: #2c3e50;
            background-color: #ffffff;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        /* Header styling to match your template */
        .page-header {
            padding: 4rem 0 2rem;
            text-align: center;
            border-bottom: 1px solid #e5e7eb;
            margin-bottom: 3rem;
        }

        .page-title {
            font-size: 3rem;
            font-weight: 700;
            color: #1f2937;
            margin-bottom: 1rem;
            letter-spacing: -0.025em;
        }

        .page-subtitle {
            font-size: 1.25rem;
            color: #6b7280;
            max-width: 600px;
            margin: 0 auto;
        }

        /* Project card styling */
        .project {
            background: #ffffff;
            border: 1px solid #e5e7eb;
            border-radius: 12px;
            padding: 2.5rem;
            margin-bottom: 3rem;
            transition: all 0.2s ease;
            position: relative;
        }

        .project:hover {
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            border-color: #d1d5db;
            transform: translateY(-2px);
        }

        .project-header {
            display: flex;
            align-items: flex-start;
            gap: 1.5rem;
            margin-bottom: 1.5rem;
        }

        .project-icon {
            width: 48px;
            height: 48px;
            background: #f3f4f6;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            color: #4b5563;
            flex-shrink: 0;
        }

        .project-title {
            font-size: 1.875rem;
            font-weight: 700;
            color: #111827;
            margin: 0;
            line-height: 1.3;
        }

        .project-description {
            font-size: 1.125rem;
            color: #4b5563;
            line-height: 1.7;
            margin-bottom: 2rem;
        }

        .project-highlight {
            background: #fef3c7;
            padding: 0.125rem 0.375rem;
            border-radius: 4px;
            font-weight: 600;
            color: #92400e;
        }

        /* Stats/metrics grid */
        .project-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 1rem;
            margin: 2rem 0;
            padding: 1.5rem;
            background: #f9fafb;
            border-radius: 8px;
            border: 1px solid #e5e7eb;
        }

        .stat-item {
            text-align: center;
        }

        .stat-value {
            font-size: 1.5rem;
            font-weight: 700;
            color: #111827;
            display: block;
        }

        .stat-label {
            font-size: 0.875rem;
            color: #6b7280;
            margin-top: 0.25rem;
        }

        /* Technology tags */
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 0.75rem;
            margin: 1.5rem 0;
        }

        .tech-tag {
            background: #f3f4f6;
            color: #374151;
            padding: 0.5rem 1rem;
            border-radius: 6px;
            font-size: 0.875rem;
            font-weight: 500;
            border: 1px solid #d1d5db;
        }

        /* Project links */
        .project-links {
            display: flex;
            gap: 1rem;
            margin: 2rem 0;
        }

        .project-link {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            background: #111827;
            color: #ffffff;
            text-decoration: none;
            padding: 0.75rem 1.5rem;
            border-radius: 6px;
            font-weight: 500;
            font-size: 0.875rem;
            transition: all 0.2s ease;
        }

        .project-link:hover {
            background: #374151;
            transform: translateY(-1px);
        }

        .project-link svg {
            width: 16px;
            height: 16px;
        }

        /* Media grid for images/videos */
        .media-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .media-item {
            border-radius: 8px;
            overflow: hidden;
            border: 1px solid #e5e7eb;
        }

        .media-item img {
            width: 100%;
            height: auto;
            display: block;
        }

        /* Video container */
        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            background: #f3f4f6;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .video-placeholder {
            font-size: 2rem;
            color: #6b7280;
        }

        /* Dashboard container */
        .dashboard-container {
            margin: 2rem 0;
            border-radius: 8px;
            overflow: hidden;
            border: 1px solid #e5e7eb;
        }

        .dashboard-container iframe {
            width: 100%;
            height: 500px;
            border: none;
        }

        /* Impact callout */
        .impact-callout {
            background: #ecfdf5;
            border: 1px solid #a7f3d0;
            border-radius: 8px;
            padding: 1.5rem;
            margin: 1.5rem 0;
        }

        .impact-title {
            font-weight: 600;
            color: #065f46;
            margin-bottom: 0.5rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .impact-text {
            color: #047857;
            font-size: 0.95rem;
        }

        /* Responsive design */
        @media (max-width: 768px) {
            .container {
                padding: 0 1rem;
            }

            .page-title {
                font-size: 2.25rem;
            }

            .project {
                padding: 1.5rem;
            }

            .project-header {
                flex-direction: column;
                gap: 1rem;
            }

            .media-grid {
                grid-template-columns: 1fr;
            }

            .project-stats {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        /* Animation utilities */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeIn 0.6s ease forwards;
        }

        @keyframes fadeIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <!-- Page Header -->
        <header class="page-header">
            <h1 class="page-title">Projects</h1>
            <p class="page-subtitle">A collection of data science and machine learning projects showcasing technical expertise and real-world impact</p>
        </header>

        <!-- Pulsepanion Project -->
        <article class="project fade-in">
            <div class="project-header">
                <div class="project-icon">🏥</div>
                <div>
                    <h2 class="project-title">Pulsepanion – AI Healthcare Tool</h2>
                </div>
            </div>
            
            <p class="project-description">
                <strong>Pulsepanion</strong> is an <span class="project-highlight">AI-based healthcare project</span> that takes about eighteen months of patient data and turns it into <span class="project-highlight">useful insights for caregivers</span>. It uses <span class="project-highlight">natural language processing (NLP)</span> to process the records and provides an <span class="project-highlight">interactive R Shiny dashboard</span> where users can explore results. I also added a <span class="project-highlight">PDF export feature</span> so caregivers can easily share summaries. The goal was to make it easier to find patterns and insights in patient data without having to go through everything manually.
            </p>

            <div class="impact-callout">
                <div class="impact-title">
                    📈 Impact
                </div>
                <p class="impact-text">Streamlines medical data analysis, reducing manual review time by 85% and enabling healthcare professionals to identify critical patterns faster.</p>
            </div>

            <div class="project-stats">
                <div class="stat-item">
                    <span class="stat-value">18</span>
                    <div class="stat-label">Months of Data</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">NLP</span>
                    <div class="stat-label">AI Processing</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">PDF</span>
                    <div class="stat-label">Export Ready</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">R Shiny</span>
                    <div class="stat-label">Interactive UI</div>
                </div>
            </div>

            <div class="tech-stack">
                <span class="tech-tag">R Shiny</span>
                <span class="tech-tag">OpenAI API</span>
                <span class="tech-tag">NLP</span>
                <span class="tech-tag">Healthcare Analytics</span>
            </div>

            <div class="project-links">
                <a href="https://github.com/k-shiroma-code/NCHacks-Pulsepanion" class="project-link" target="_blank" rel="noopener noreferrer">
                    <svg viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0024 12c0-6.63-5.37-12-12-12z"/>
                    </svg>
                    View on GitHub
                </a>
            </div>

            <div class="media-grid">
                <div class="media-item">
                    <img src="{{ site.baseurl }}/assets/img/Pulsepantion.jpg" alt="Pulsepanion Dashboard" loading="lazy">
                </div>
                <div class="media-item">
                    <div class="video-container" onclick="window.open('https://www.youtube.com/watch?v=tEJoXKLzVH4', '_blank')">
                        <div class="video-placeholder">▶️</div>
                    </div>
                </div>
            </div>
        </article>

        <!-- Customer Segmentation Project -->
        <article class="project fade-in" style="animation-delay: 0.2s">
            <div class="project-header">
                <div class="project-icon">👥</div>
                <div>
                    <h2 class="project-title">Customer Segmentation Analytics</h2>
                </div>
            </div>
            
            <p class="project-description">
                This project delivers a <span class="project-highlight">comprehensive analysis of over 500,000 retail transactions</span> to uncover <span class="project-highlight">behavioral patterns</span> in customer activity. Using <span class="project-highlight">RFM (Recency, Frequency, Monetary) analysis</span>, the study identified <span class="project-highlight">five distinct customer segments</span>, revealed <span class="project-highlight">seasonal purchasing trends</span>, and optimized <span class="project-highlight">marketing spend allocation by 25%</span>. Developed with <span class="project-highlight">SQL, Tableau, and Python</span>, the analytics pipeline converts raw sales data into <span class="project-highlight">clear insights for strategic business decisions</span>.
            </p>

            <div class="impact-callout">
                <div class="impact-title">
                    💰 Business Impact
                </div>
                <p class="impact-text">Generated measurable ROI through targeted marketing campaigns, improving customer retention rates and reducing acquisition costs across all segments.</p>
            </div>

            <div class="project-stats">
                <div class="stat-item">
                    <span class="stat-value">500K+</span>
                    <div class="stat-label">Transactions</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">5</span>
                    <div class="stat-label">Customer Segments</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">25%</span>
                    <div class="stat-label">Cost Optimization</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">RFM</span>
                    <div class="stat-label">Analysis Method</div>
                </div>
            </div>

            <div class="tech-stack">
                <span class="tech-tag">SQL</span>
                <span class="tech-tag">Tableau</span>
                <span class="tech-tag">Python</span>
                <span class="tech-tag">RFM Analysis</span>
                <span class="tech-tag">Data Visualization</span>
            </div>

            <div class="project-links">
                <a href="https://github.com/k-shiroma-code/Customer-Segmentation-with-RFM-Analysis" class="project-link" target="_blank" rel="noopener noreferrer">
                    <svg viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0024 12c0-6.63-5.37-12-12-12z"/>
                    </svg>
                    View on GitHub
                </a>
            </div>

            <div class="dashboard-container">
                <iframe src="https://public.tableau.com/views/Customer_Segmentation_Overview_Github/Dashboard1?:showVizHome=no&:embed=true" title="Customer Segmentation Dashboard"></iframe>
            </div>
        </article>

        <!-- Heart Disease Prediction Project -->
        <article class="project fade-in" style="animation-delay: 0.4s">
            <div class="project-header">
                <div class="project-icon">❤️</div>
                <div>
                    <h2 class="project-title">Heart Disease Prediction Pipeline</h2>
                </div>
            </div>
            
            <p class="project-description">
                This <span class="project-highlight">machine learning pipeline</span> predicts <span class="project-highlight">cardiovascular risk</span> using the <span class="project-highlight">UCI Heart Disease dataset</span>. By addressing <span class="project-highlight">class imbalance with SMOTE</span> and applying <span class="project-highlight">logistic regression</span>, it achieved a <span class="project-highlight">20% improvement in minority-class recall</span>. <span class="project-highlight">Feature engineering and selection</span> ensured <span class="project-highlight">optimal model performance</span>, and the final pipeline is designed for <span class="project-highlight">production deployment</span> in healthcare analytics contexts.
            </p>

            <div class="impact-callout">
                <div class="impact-title">
                    🏥 Healthcare Impact
                </div>
                <p class="impact-text">Enables early cardiovascular risk detection, potentially preventing heart disease through timely medical intervention and improved patient outcomes.</p>
            </div>

            <div class="project-stats">
                <div class="stat-item">
                    <span class="stat-value">20%</span>
                    <div class="stat-label">Recall Improvement</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">SMOTE</span>
                    <div class="stat-label">Balance Method</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">UCI</span>
                    <div class="stat-label">Dataset Source</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">Production</span>
                    <div class="stat-label">Ready Pipeline</div>
                </div>
            </div>

            <div class="tech-stack">
                <span class="tech-tag">Python</span>
                <span class="tech-tag">Scikit-learn</span>
                <span class="tech-tag">SMOTE</span>
                <span class="tech-tag">Logistic Regression</span>
            </div>

            <div class="project-links">
                <a href="https://github.com/k-shiroma-code/Heart-Disease-ML-Project" class="project-link" target="_blank" rel="noopener noreferrer">
                    <svg viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0024 12c0-6.63-5.37-12-12-12z"/>
                    </svg>
                    View on GitHub
                </a>
            </div>

            <div class="media-grid">
                <div class="media-item">
                    <img src="{{ site.baseurl }}/assets/img/IMG_1668.jpg" alt="Model Performance Metrics" loading="lazy">
                </div>
                <div class="media-item">
                    <img src="{{ site.baseurl }}/assets/img/Feature_Importance.jpg" alt="Feature Importance Analysis" loading="lazy">
                </div>
            </div>
        </article>

        <!-- UEFA Euro 2024 Project -->
        <article class="project fade-in" style="animation-delay: 0.6s">
            <div class="project-header">
                <div class="project-icon">⚽</div>
                <div>
                    <h2 class="project-title">UEFA Euro 2024 Sports Analytics Project</h2>
                </div>
            </div>
            
            <p class="project-description">
                This <span class="project-highlight">sports analytics project</span> developed <span class="project-highlight">predictive models</span> for UEFA Euro 2024 match outcomes by combining <span class="project-highlight">ELO-based ratings</span> with traditional <span class="project-highlight">statistical features</span>. Models such as <span class="project-highlight">Decision Trees, Random Forests, and XGBoost</span> were trained and evaluated using <span class="project-highlight">precision, recall, and F1-score</span> to identify the most effective approach. The project also included <span class="project-highlight">visualizations comparing predictions with actual outcomes</span>, providing insights into <span class="project-highlight">model accuracy</span> and <span class="project-highlight">forecasting reliability</span> in competitive sports analytics.
            </p>

            <div class="impact-callout">
                <div class="impact-title">
                    📊 Sports Analytics Impact
                </div>
                <p class="impact-text">Demonstrated advanced predictive modeling techniques in sports analytics, contributing to the understanding of tournament outcome forecasting.</p>
            </div>

            <div class="project-stats">
                <div class="stat-item">
                    <span class="stat-value">3</span>
                    <div class="stat-label">ML Models</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">ELO</span>
                    <div class="stat-label">Rating System</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">Euro 2024</span>
                    <div class="stat-label">Tournament</div>
                </div>
                <div class="stat-item">
                    <span class="stat-value">XGBoost</span>
                    <div class="stat-label">Best Model</div>
                </div>
            </div>

            <div class="tech-stack">
                <span class="tech-tag">Python</span>
                <span class="tech-tag">XGBoost</span>
                <span class="tech-tag">Feature Engineering</span>
                <span class="tech-tag">Statistical Modeling</span>
                <span class="tech-tag">Sports Analytics</span>
            </div>

            <div class="project-links">
                <a href="https://github.com/k-shiroma-code/CSUF-REU-Football-Analytics" class="project-link" target="_blank" rel="noopener noreferrer">
                    <svg viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0024 12c0-6.63-5.37-12-12-12z"/>
                    </svg>
                    View on GitHub
                </a>
            </div>

            <div class="media-grid">
                <div class="media-item">
                    <img src="{{ site.baseurl }}/assets/img/IMG_1670.jpg" alt="UEFA Euro 2024 Prediction Visualization 1" loading="lazy">
                </div>
                <div class="media-item">
                    <img src="{{ site.baseurl }}/assets/img/IMG_1671.jpg" alt="UEFA Euro 2024 Prediction Visualization 2" loading="lazy">
                </div>
            </div>
        </article>
    </div>

    <script>
        // Progressive loading for better performance
        document.addEventListener('DOMContentLoaded', function() {
            // Intersection Observer for animations
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };

            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, observerOptions);

            // Observe all fade-in elements
            document.querySelectorAll('.fade-in').forEach(el => {
                observer.observe(el);
            });

            // Copy functionality for code snippets (if needed later)
            window.copyCode = function(button) {
                const code = button.parentElement.nextElementSibling.textContent;
                navigator.clipboard.writeText(code).then(() => {
                    const originalText = button.textContent;
                    button.textContent = 'Copied!';
                    setTimeout(() => {
                        button.textContent = originalText;
                    }, 2000);
                });
            };
        });
    </script>
</body>
</html>
