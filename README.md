# Awesome-Document-AI-Platform

## Top Document AI Platform Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Intelligent Document Processing, OCR & Structured Data Extraction*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Document AI**. These tools extract, classify, and structure data from documents such as invoices, receipts, contracts, and forms — enabling automation for finance, legal, healthcare, and enterprise operations.



**Examples** include Hyperscience, Rossum, Nanonets, ABBYY, Google Document AI, Azure AI Document Intelligence, Amazon Textract, Veryfi, Klippa, and Docsumo (the category leaders).



**Open-source emphasis**: This section is expanded with active projects for self-hosting, custom extraction schemas, and transparent document processing — ideal for developers, researchers, and enterprises building vendor-independent document intelligence pipelines. The open-source ecosystem in 2026 is anchored by **Docling** (IBM Research), **lift** (Datalab), and **PaddleOCR-VL** (Baidu), with strong coverage in vision-language models, schema-constrained extraction, and layout-aware parsing.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Hyperscience](https://www.hyperscience.com/)**  

  Enterprise intelligent document processing platform with human-in-the-loop automation for complex document workflows.



- **[Rossum](https://rossum.ai/)**  

  AI-powered document automation platform specializing in invoice and purchase order processing with a focus on transactional documents.



- **[Nanonets](https://nanonets.com/)**  

  No-code AI document processing platform for extracting data from invoices, receipts, and forms with pre-built and custom models.



- **[ABBYY](https://www.abbyy.com/)**  

  Comprehensive document AI and process intelligence platform with OCR, IDP, and content intelligence capabilities.



- **[Google Document AI](https://cloud.google.com/document-ai)**  

  Cloud-based document understanding platform with pre-trained models for invoices, receipts, forms, and custom extraction.



- **[Azure AI Document Intelligence](https://azure.microsoft.com/en-us/products/ai-services/ai-document-intelligence)**  

  Microsoft's document processing service with pre-built models and custom extraction for forms, invoices, and receipts.



- **[Amazon Textract](https://aws.amazon.com/textract/)**  

  AWS's document text and data extraction service using machine learning for forms, tables, and structured data.



- **[Veryfi](https://www.veryfi.com/)**  

  Real-time document extraction API for receipts, invoices, and financial documents with mobile SDKs.



- **[Klippa](https://www.klippa.com/)**  

  Document automation platform with OCR and data extraction for receipts, invoices, and identity documents.



- **[Docsumo](https://www.docsumo.com/)**  

  AI-powered document processing platform with focus on financial documents and automated data extraction.



## Open-Source GitHub Projects



- **[Docling](https://github.com/docling-project/docling)**  

  The leading open-source document processing framework from IBM Research, described by Thoughtworks Technology Radar as "an open-source, self-hostable alternative to proprietary cloud-managed services such as Azure Document Intelligence, Amazon Textract and Google Document AI" . Converts complex PDFs and scanned documents into structured JSON and Markdown using computer vision-based layout and semantic understanding . Strong for RAG pipelines with reading order preservation, table structure recognition, and visual grounding. MIT licensed, integrates with LangChain and LangGraph .



- **[lift](https://huggingface.co/datalab-to/lift)**  

  Structured extraction model from Datalab that pulls structured JSON from PDFs and images using schema-constrained decoding to guarantee valid, well-typed output . Pass any JSON schema and lift returns a matching JSON object, handling multi-page documents and values spanning pages. 9B parameter model achieves 90.2% field accuracy with 9.5s median latency — outperforming Gemini Flash 3.5 (91.3%) on speed and Azure Content Understanding (83.4%) on accuracy . Apache 2.0 code with modified OpenRAIL-M weights.



- **[PaddleOCR-VL-1.6](https://huggingface.co/PaddlePaddle/PaddleOCR-VL-1.6)**  

  Baidu's compact document parsing model achieving **96.33% on OmniDocBench v1.6** — state-of-the-art among open-source solutions . 1B parameter model with region-aware optimization for weak areas, progressive post-training with RL, and significant improvements in table recognition, Chinese ancient documents, rare characters, and seal/stamp recognition . Fully compatible with v1.5 for zero-cost migration. Apache 2.0 licensed.



- **[Qianfan-OCR](https://huggingface.co/rootlocalghost/Qianfan-OCR)**  

  Baidu Qianfan Team's 4B-parameter end-to-end document intelligence model that unifies document parsing, layout analysis, and document understanding . **#1 end-to-end model on OmniDocBench v1.5** (93.12 overall), surpassing DeepSeek-OCR-v2 (91.09) and Gemini-3 Pro (90.33). Includes innovative "Layout-as-Thought" phase for structured layout recovery via ⟨think⟩ tokens. 192 languages supported. Achieves 1.024 pages/second with W8A8 quantization on single A100 .



- **[NuExtract3](https://huggingface.co/numind/NuExtract3)**  

  NuMind's structured extraction model supporting in-context examples for ambiguous schemas . Features template generation from natural language descriptions and reasoning mode for harder extraction tasks. Supports Markdown OCR mode. 81.5% field accuracy in benchmarks, with 8.3s median latency (fastest local model tested) .



- **[Qwen2.5-VL](https://huggingface.co/Qwen/Qwen2.5-VL-7B-Instruct)**  

  Alibaba's general-purpose vision-language model family (3B, 7B, 72B) with strong OCR capabilities . Not purpose-built for documents but excels at targeted field extraction when prompted — extract specific fields as JSON, tables as markdown, or describe structure in natural language. 7B model runs on consumer GPUs (~6GB VRAM); 72B competes with GPT-4o on document benchmarks. Apache 2.0 licensed .



- **[olmOCR](https://github.com/allenai/olmocr)**  

  Allen AI's industrial-scale PDF digitization tool achieving **82.4% on olmOCR-bench** . The headline number: converts **one million PDF pages for ~$190** using optimized SGLang inference — roughly 1/32nd the cost of GPT-4o . 7B model requires NVIDIA GPU with 16GB+ VRAM. Supports automatic page rendering, rotation correction, and retry logic for heterogeneous documents.



- **[TinyDoc-VLM](https://pypi.org/project/tinydoc-vlm/)**  

  256M-parameter document-specialist VLM that runs on **CPU, Raspberry Pi 5, or MacBook Air** with <1GB VRAM . SigLIP vision encoder + SmolLM2 decoder architecture. Handles invoices, receipts, forms, tables, and charts. Apache 2.0 licensed with ONNX export. LoRA fine-tuning with only 2.7M trainable params (0.93%) .



- **[Kreuzberg (xberg)](https://pkg.go.dev/github.com/kreuzberg-dev/kreuzberg)**  

  Document extraction engine supporting **101 formats across 115 file extensions** . Features intelligent format detection, OCR for images, MCP server for AI agent integration (9 tools, 3 prompts, 4 resources), and REST API server. CLI with 12 commands including extract, batch, detect, and serve. Docker deployment available .



- **[AlienTables](https://pypi.org/project/AlienTables/)**  

  Local, privacy-first PDF-to-Excel extraction engine with adaptive OCR fallback (pytesseract + pdf2image) . Built for batch processing thousands of same-template PDFs (invoices, purchase orders, shipping manifests). Generates per-file Excel output with detailed audit CSVs (audit.csv, orphan_pages.csv, review.csv) . Fully local — no cloud upload.



- **[DocTR](https://github.com/mindee/doctr)**  

  OCR library supporting PyTorch and TensorFlow with **structured JSON output** (blocks, lines, words, bounding boxes) . Ideal when OCR is the first step in a larger document automation pipeline — richer output reduces downstream parsing complexity. Requires more setup than basic OCR but enables table reconstruction, field detection, and region-based grouping .



- **[Receipt Wrangler](https://github.com/Receipt-Wrangler/receipt-wrangler)**  

  Self-hosted receipt tracking with OCR (Tesseract offline) and optional AI provider integration (OpenAI, Gemini, Ollama) . Extracts merchant, date, total, and line items; categorizes, tags, and splits receipts across groups. Web app + iOS/Android apps. AGPL-3.0 licensed with one-click Railway deployment .



### Additional Strong Open-Source Options



- **Tesseract OCR** — The foundational open-source OCR engine, still widely used for basic text extraction .

- **EasyOCR** — Popular Python OCR library supporting 80+ languages with simple API .

- **Surya** — Document OCR, layout, and tables via a 0.7B parameter model with modified license .

- **MonkeyOCRv2** — 0.8B parsing model with smaller and larger variants .

- **MinerU2.5** — OpenDataLab's 1.2B structured JSON/Markdown extraction pipeline .

- **VerifyDoc** — Trust layer for AI document extraction adding per-field confidence, source grounding, and accept/review abstention .



**Frameworks for building custom Document AI pipelines**: Combine **Docling** for layout-aware parsing and RAG-ready output, **lift** or **NuExtract3** for schema-constrained structured extraction, and **PaddleOCR-VL-1.6** or **Qianfan-OCR** for state-of-the-art parsing accuracy . Use **TinyDoc-VLM** for CPU-only or edge deployments . Integrate **VerifyDoc** as a trust layer to add per-field confidence and abstention to any extractor . For high-volume digitization, **olmOCR** delivers industrial-scale cost efficiency ($190/million pages) with GPU infrastructure . Note that true enterprise Document AI platforms with managed scaling, pre-built industry models, and compliance certifications remain primarily commercial territory; open-source stacks provide strong parsing, extraction, and validation foundations that require integration for complete document automation.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Document AI tools process sensitive business and personal data. Self-hosted solutions require proper security hardening, encryption at rest and in transit, and compliance with data privacy regulations (GDPR, CCPA, HIPAA).

- Model accuracy varies by document type, language, and quality. Benchmark results should not be interpreted as guarantees of production performance on your specific documents.

- The open-source ecosystem provides strong parsing, extraction, and validation foundations, but enterprise-grade managed scaling, industry-specific pre-trained models, and compliance certifications remain primarily commercial offerings.



---



**Made for document processing engineers, automation architects, finance operations teams, and AI developers.**

Let's make Document AI more open, transparent, and accessible.
