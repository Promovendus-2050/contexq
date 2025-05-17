# Contextual News Analysis for Risk Signal Generation

## Overview  
This system ingests news articles from RSS feeds, applies NLP to extract entities/events/sentiment, constructs a knowledge graph, and identifies risk signals through graph analytics. Designed for financial crime, supply chain, and geopolitical risk monitoring.

## Structure  

├── scripts/
│ ├── data_collector.py
│ ├── nlp_processor.py
│ ├── graph_builder.py
│ ├── analysis.py
│ └── visualizer.py
├── data/
├── visualizations/
└── README.md


## Instructions  
1. **Install dependencies**:  
   ```bash  
   pip install -r requirements.txt  
   python -m spacy download en_core_web_trf  

Then run - python main.py

## Output:

Interactive graph: risk_network.html

Risk report: risk_signals.json

## Cloud Deployment - Foreseen Directions
Smarter Implementation choices:

Neo4j Aura DB: Stores graph data persistently with relationship metadata.

PyVis: Generates browser-based interactive visualizations.

Future Integrations:

Zapier MCP Automation:

Trigger pipeline via Slack/email alerts using Zapier webhooks.

Auto-post risk signals to Confluence/Jira for audit trails.

Neo4j Enhancements:

Deploy to Neo4j Aura Cloud for real-time graph queries.

Implement APOC procedures for temporal risk scoring.

AWS Lambda:

Schedule daily RSS scraping with EventBridge.

Use S3 for versioned article storage.

## Enhancements - Foreseen Directions 

Added BERT-based NER for entity extraction (vs basic spaCy).

Implemented Louvain communities for risk cluster detection.

Integrated VADER sentiment with domain-specific lexicons.

PyVis visualization with node centrality/sentiment encoding.
