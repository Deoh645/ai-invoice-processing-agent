# AI-Powered Invoice Processing Agent

An automated, production-ready backend pipeline built to eliminate manual accounting data entry by intelligently extracting, parsing, and centralizing financial documents.

## 🚀 System Architecture
- **Trigger**: Monitors inbound project files and document streams for incoming invoice documents.
- **AI Core**: Integrates an LLM Content Extractor to dynamically parse unstructured PDFs, isolating key fields: `Vendor Name`, `Invoice Number`, `Invoice Date`, and `Amount Due`.
- **Database/Warehouse**: Automatically streams and logs structured data into Google Sheets in real-time.

## 🛠️ Resiliency & Error Handling
- **Data Stream Optimization**: Configured custom cell formatting inputs (`RAW` transmission data mapping) to eliminate API grid caching bugs.
- **Self-Healing Fault Tolerance**: Implemented a proactive `Skip` error directive on the destination module to handle external API timeouts or network blips seamlessly, guaranteeing maximum system uptime without manual engineering triage.

## 📁 Repository Contents
- `blueprint.json`: The complete architectural layout of the Make.com scenario (importable back into any Make environment).

## 📄 License
MIT License
