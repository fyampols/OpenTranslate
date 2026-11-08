# OpenTranslate
An open-source, AI-powered document translation platform designed to translate large documents, datasets, and knowledge repositories into English while preserving structure, formatting, and context. 

OpenTranslate 

An open-source, AI-powered document translation platform designed to translate large documents, datasets, and knowledge repositories into English while preserving structure, formatting, and context. 

Mission 

Make high-quality document translation accessible, transparent, and self-hostable. 

OpenTranslate enables organizations, researchers, governments, educators, and individuals to translate large volumes of content without being locked into a specific vendor or AI provider. 

Key Features 

Document Translation 

PDF translation 

DOCX translation 

Excel translation 

CSV translation 

TXT translation 

HTML translation 

JSON translation 

Large-Scale Processing 

Handles multi-hundred-page documents 

Streaming translation pipeline 

Intelligent chunking 

Parallel processing 

Background job execution 

Recovery from failed jobs 

Multiple Translation Engines 

Supported providers: 

OpenAI 

Azure OpenAI 

Azure Translator 

DeepL 

Ollama 

LibreTranslate 

Custom Plugins 

OCR Support 

Scanned PDFs 

Images 

Screenshots 

Multi-language OCR 

Translation Memory 

Reuse existing translations automatically to improve consistency and reduce cost. 

Glossary Management 

Create project-specific terminology dictionaries. 

Example: 

Source, Translation 

CRM, Customer Relationship Management 

SKU, Stock Keeping Unit 

Privacy First 

Deploy entirely on-premises using local models. 

Supported local AI: 

Llama 

Qwen 

Mistral 

Gemma 

No internet connection required. 

 

Architecture 

                User 
                   │ 
                   ▼ 
           Next.js Frontend 
                   │ 
                   ▼ 
              FastAPI API 
                   │ 
       ┌───────────┼───────────┐ 
       ▼           ▼           ▼ 
   Parser     OCR Engine   Job Queue 
       │           │           │ 
       └───────► Translation ◄─┘ 
                         │ 
                         ▼ 
                Output Generator 
                         │ 
                         ▼ 
                   Download 
