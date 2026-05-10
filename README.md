

**Anomaly Detection & Digital Forensics**
📌 **About This Project**
The Digital Investigation and E-Discovery project is an academic cybersecurity assessment demonstrating a practical anomaly-based intrusion detection system using machine learning, showcasing SSH authentication log analysis, behavioural feature engineering, and risk classification procedures within a controlled analytical environment using Python and scikit-learn as the core development stack targeting real Linux system login data.

**Technologies Used**
Hardware: MacBook Pro Development Machine, Linux Server (SSH Log Source), Host Network Interface for log collection
Software: Python 3.9, Jupyter Notebook, scikit-learn Isolation Forest, Pandas & NumPy Data Libraries, Matplotlib Visualisation Library, Visual Studio Code IDE, Synthetic Data Generator (custom-built)

**Core Techniques:** Unsupervised Machine Learning (Isolation Forest), Behavioural Feature Engineering, Rule-Based Risk Override, Anomaly Scoring & Classification, SSH Log Parsing & IP Extraction

**Key Features Developed**

**Log Ingestion & Feature Extraction:** Real SSH authentication logs were parsed and converted into structured CSV datasets, extracting behavioural signals including login hour, failed authentication count, new device flags, and previously unseen IP addresses, enabling systematic analysis of login patterns.

**Anomaly Detection Model:** An Isolation Forest algorithm was trained using scikit-learn on extracted behavioural features to establish a baseline of normal login activity, isolating statistically unusual login events without requiring labelled training data, making the system effective against novel attack patterns.

**Risk Scoring & Classification:** A MinMaxScaler-normalised scoring pipeline converted raw anomaly scores into a 0–100 risk scale, with a three-tier classification system assigning every login event a Low, Medium, or High risk label, providing actionable intelligence for security analysts.

**Rule-Based Override Engine:** Domain-specific security rules were layered on top of the ML model to automatically escalate risk scores for high-confidence threat conditions, including failed logins from new IP addresses on new devices occurring between 1–4 AM, ensuring critical events were never under-prioritised.

**Visualisation & Forensic Reporting:** Scatter plots and line graphs were generated using Matplotlib to visualise normal versus anomalous login distributions by hour, average risk scores across time periods, and behavioural outlier patterns, supporting interpretable forensic reporting.

**Project Outcomes**
Successfully demonstrated a complete anomaly detection pipeline from raw SSH log ingestion through feature engineering, unsupervised ML model training, risk scoring, rule-based override, and forensic visualisation, providing a comprehensive practical understanding of machine learning-driven intrusion detection.

Conducted in-depth forensic analysis of two real-world data breach case studies, the Equifax Apache Struts exploitation (2017) and the Capital One SSRF cloud breach (2019), contextualising the detection system within the broader landscape of contemporary cybersecurity threats and attacker evasion techniques.

Established a thorough countermeasures framework addressing anomaly-based IDS deployment, ML-driven log monitoring, proactive patch management, network segmentation, and security certificate maintenance, grounded directly in the attack patterns and detection gaps observed throughout the practical demonstration.
