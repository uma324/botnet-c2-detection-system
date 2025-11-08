# botnet-c2-detection-system
A graph-based botnet detection project using Python and network analysis to identify C2 communication patterns.
🔐 About the Project

This project is a hands-on implementation of a botnet detection system that analyzes network communication patterns using graph theory and machine learning.

It represents each device as a node and each network connection as an edge. By studying the relationships between nodes, the system can identify suspicious or abnormal behavior that may indicate bot-infected devices or Command-and-Control (C2) servers.

This project helped me understand how mathematical models and network analysis can uncover hidden cyber threats that are not visible through traditional rule-based detection.

🎯 Objectives

Build a graph-based model of network communications.

Detect anomalous nodes using unsupervised learning (Isolation Forest).

Visualize communication networks and highlight potential botnet activity.

Understand how graph metrics reveal hidden structures of attacks.

🧠 Key Concepts Used

Graph Theory – modeling communication relationships in a network.

NetworkX – for creating and visualizing network graphs.

Isolation Forest – to detect unusual or suspicious communication patterns.

Data Preprocessing – cleaning and scaling synthetic data for model training.

Visualization – using Matplotlib to display network anomalies and suspicious nodes.

⚙️ Tools and Technologies
Category	Tools Used
Programming	Python 3
Libraries	Pandas, NumPy, NetworkX, Matplotlib, Scikit-learn
Environment	macOS (Intel Architecture)
IDE	Jupyter Notebook / VS Code / Terminal
Dataset	Synthetic Network Traffic (self-generated)
🧩 Project Workflow
graph TD
A[Data Generation] --> B[Graph Construction]
B --> C[Feature Extraction]
C --> D[Anomaly Detection]
D --> E[Visualization & Results]


Explanation:

The synthetic data simulates real network traffic.

Graphs are built from communication flows.

Graph-based features are extracted and analyzed.

Unsupervised algorithms detect abnormal nodes.

Finally, results are visualized for easy interpretation.

📂 Folder Structure
botnet_c2_detection/
│
├── data/
│   └── synthetic_flows.csv
├── src/
│   ├── generate_synthetic.py
│   ├── features_detect.py
│   ├── detector.py
│   ├── run_detection.py
│   ├── eval_run.py
│   └── visualize_results.py
├── results/
│   ├── node_scores.csv
│   ├── final_graph.png
│   └── top_suspicious_nodes.png
└── venv/

🚀 How to Run the Project
1️⃣ Setup Environment
git clone https://github.com/<your-username>/botnet-c2-detection-system.git
cd botnet-c2-detection-system
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

2️⃣ Generate Synthetic Network Data
python src/generate_synthetic.py

3️⃣ Run Detection Pipeline
python src/run_detection.py

4️⃣ Evaluate Model
python src/eval_run.py

5️⃣ Visualize Results
python src/visualize_results.py
open results/final_graph.png
open results/top_suspicious_nodes.png

📊 Example Output
🕸 Network Graph Visualization

Red nodes → Suspicious or anomalous devices

Blue nodes → Normal devices

Saved as: results/final_graph.png

📈 Top Suspicious Nodes

Bar chart showing nodes ranked by anomaly score

Saved as: results/top_suspicious_nodes.png

💡 Results Summary
Metric	Score
Precision	0.20
Recall	0.08
F1-Score	0.11
AUC	0.89

Even though the project uses synthetic traffic, it successfully detected repetitive and centralized communication patterns that resemble real botnet activity.
