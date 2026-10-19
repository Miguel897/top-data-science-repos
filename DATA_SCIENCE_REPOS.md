# Top Data Science Repositories

A curated list of popular data-science repositories on GitHub, organized by field and by business application. The focus is on **systems, implementations, examples, and ready-to-run projects** rather than bare libraries.

## Criteria

- **Popularity:** at least **20k GitHub stars**.
- **Star counts** are approximate, rounded values read from the public GitHub pages on 2026-10-19. They change over time.
- **Python packages** that are not the most famous ones (pandas, scikit-learn, etc.) are grouped in their own section at the end. Repos are listed once, in the field where they fit best, and the Python section links back to them.
- Each entry is tagged with its type: **System**, **Implementation**, **Examples**, **Course**, **Library**, or **Reference**.

## Field map

| Field | Business applications | Section |
|---|---|---|
| Recommendation systems | Product recommendations, personalization, e-commerce | [1](#1-recommendation-systems) |
| RAG & LLM applications | Internal knowledge bases, document Q&A, support copilots, AI agents | [2](#2-rag--llm-applications) |
| Computer vision | Quality inspection, object detection, segmentation, video analytics | [3](#3-computer-vision) |
| OCR & document AI | Invoice and form extraction, digitizing archives, feeding documents to LLMs | [4](#4-ocr--document-ai) |
| Big data & batch processing | ETL at scale, PySpark batch jobs, pipeline orchestration | [5](#5-big-data--batch-processing) |
| Time series forecasting | Demand, sales, and capacity forecasting | [6](#6-time-series-forecasting) |
| BI & data apps | Dashboards, internal tools, ML demos | [7](#7-bi--data-apps) |
| MLOps | Experiment tracking, model registry, deployment | [8](#8-mlops) |
| Speech | Call-center transcription, voice interfaces | [9](#9-speech) |
| Learning & reference | Learning ML in practice, deep learning, ML in production | [10](#10-learning--reference) |
| Python packages | Pip-installable libraries that are not the most famous | [Python packages](#python-packages-not-the-most-famous) |

---

## 1. Recommendation systems

- **[microsoft/recommenders](https://github.com/microsoft/recommenders)** (~22.0k) · *Examples*
  Best-practice notebooks and utilities covering collaborative filtering, content-based, and deep learning recommenders, plus evaluation. Under the Linux Foundation for AI & Data.

## 2. RAG & LLM applications

- **[infiniflow/ragflow](https://github.com/infiniflow/ragflow)** (~92.4k) · *System*
  Open-source RAG engine that combines retrieval with agent capabilities to build a context layer for LLMs. Ready to deploy for document-grounded assistants.
- **[Mintplex-Labs/anything-llm](https://github.com/Mintplex-Labs/anything-llm)** (~67.3k) · *System*
  Local-first app for chatting with your documents and running agents. Good reference for an internal knowledge-base product.
- **[Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps)** (~142.3k) · *Examples*
  100+ runnable AI agent and RAG apps. Folders include `rag_tutorials/`, `starter_ai_agents/`, `advanced_ai_agents/`, and `voice_ai_agents/`.
- **[NirDiamant/RAG_Techniques](https://github.com/NirDiamant/RAG_Techniques)** (~29.9k) · *Implementation*
  Notebooks that walk through advanced RAG techniques (retrieval strategies, reranking, query transformation, evaluation).
- **[NirDiamant/GenAI_Agents](https://github.com/NirDiamant/GenAI_Agents)** (~24.6k) · *Implementation*
  50+ tutorials from basic conversational bots to multi-agent systems.
- **[rasbt/LLMs-from-scratch](https://github.com/rasbt/LLMs-from-scratch)** (~106.8k) · *Implementation*
  Builds a ChatGPT-like LLM in PyTorch, step by step. Useful for understanding what a RAG or agent system relies on.
- **[mlabonne/llm-course](https://github.com/mlabonne/llm-course)** (~84.2k) · *Course*
  Roadmap and Colab notebooks for LLM engineering.
- **[microsoft/generative-ai-for-beginners](https://github.com/microsoft/generative-ai-for-beginners)** (~121.6k) · *Course*
  21 lessons on building generative AI applications.
- **[dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide)** (~79.3k) · *Reference*
  Guides, papers, and notebooks on prompt engineering, context engineering, RAG, and agents.

## 3. Computer vision

- **[ultralytics/ultralytics](https://github.com/ultralytics/ultralytics)** (~62.6k) · *Library* · see [Python packages](#python-packages-not-the-most-famous)
  YOLO models for detection, segmentation, classification, pose estimation, and tracking. Production-oriented and easy to adopt.
- **[facebookresearch/segment-anything](https://github.com/facebookresearch/segment-anything)** (~55.0k) · *Implementation*
  Inference code, checkpoints, and example notebooks for the Segment Anything Model (SAM). Useful for labeling and object-segmentation workflows.
- **[facebookresearch/detectron2](https://github.com/facebookresearch/detectron2)** (~34.9k) · *System*
  Platform for object detection, segmentation, and other visual recognition tasks.
- **[opencv/opencv](https://github.com/opencv/opencv)** (~91.2k) · *Library*
  The foundational open-source computer vision library. Used as a building block in most CV pipelines.
- **[roboflow/supervision](https://github.com/roboflow/supervision)** (~51.2k) · *Library* · see [Python packages](#python-packages-not-the-most-famous)
  Reusable tools for detections, tracking, annotation, and video analytics.

## 4. OCR & document AI

- **[PaddlePaddle/PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)** (~91.4k) · *System*
  Turns PDFs and images into structured data. Ready-to-use OCR with a strong multilingual focus.
- **[tesseract-ocr/tesseract](https://github.com/tesseract-ocr/tesseract)** (~77.1k) · *System*
  The classic open-source OCR engine. Lightweight and widely deployed.
- **[microsoft/markitdown](https://github.com/microsoft/markitdown)** (~191.0k) · *Library*
  Converts Office documents, PDFs, and other files to Markdown, a common preprocessing step before RAG.
- **[DS4SD/docling](https://github.com/DS4SD/docling)** (~69.1k) · *Library*
  Parses documents (PDF, DOCX, and more) into structured data for generative AI pipelines.
- **[JaidedAI/EasyOCR](https://github.com/JaidedAI/EasyOCR)** (~30.1k) · *Library* · see [Python packages](#python-packages-not-the-most-famous)
  Ready-to-use OCR with 80+ languages and many writing systems.

## 5. Big data & batch processing

- **[apache/spark](https://github.com/apache/spark)** (~44.2k) · *System*
  Unified analytics engine for large-scale data processing. **PySpark** (the `python/` directory) is the standard way to run batch jobs from Python.
- **[apache/airflow](https://github.com/apache/airflow)** (~47.2k) · *System*
  Platform to author, schedule, and monitor data pipelines. The usual orchestrator for nightly batch jobs.
- **Ray, Polars, DuckDB** are covered in [Python packages](#python-packages-not-the-most-famous) as alternatives for distributed or single-machine batch processing.

## 6. Time series forecasting

- **[facebook/prophet](https://github.com/facebook/prophet)** (~20.4k) · *Library* · see [Python packages](#python-packages-not-the-most-famous)
  Forecasting tool for series with multiple seasonality and linear or non-linear growth.

> **Note:** this was the only time-series repository I could verify at or above 20k stars. Others I checked are well below the threshold, such as `Nixtla/statsforecast` (~4.9k). Forecasting is a field where a 20k-star list is thin, so treat this section as incomplete.

## 7. BI & data apps

- **[apache/superset](https://github.com/apache/superset)** (~75.2k) · *System*
  Data visualization and exploration platform for dashboards over SQL databases. A self-hosted BI tool.
- **[metabase/metabase](https://github.com/metabase/metabase)** (~49.7k) · *System*
  Business intelligence and embedded analytics tool that lets non-technical users query data.
- **[streamlit/streamlit](https://github.com/streamlit/streamlit)** (~46.0k) · *Library*
  Build and share data apps in Python. Common for internal tools and model demos.
- **[gradio-app/gradio](https://github.com/gradio-app/gradio)** (~43.8k) · *Library*
  Build and share ML apps and demos in Python.

## 8. MLOps

- **[mlflow/mlflow](https://github.com/mlflow/mlflow)** (~28.4k) · *System*
  Open-source AI engineering platform for experiment tracking, model registry, and evaluation of agents, LLMs, and ML models.

## 9. Speech

- **[openai/whisper](https://github.com/openai/whisper)** (~110.8k) · *Implementation*
  Robust speech recognition trained on large-scale weakly supervised data. Used for transcription in call-center and meeting-analysis pipelines.

## 10. Learning & reference

- **[jakevdp/PythonDataScienceHandbook](https://github.com/jakevdp/PythonDataScienceHandbook)** (~50.2k) · *Examples*
  Full text in Jupyter notebooks: NumPy, pandas, Matplotlib, and scikit-learn.
- **[microsoft/ML-For-Beginners](https://github.com/microsoft/ML-For-Beginners)** (~91.6k) · *Course*
  12 weeks, 26 lessons, 52 quizzes on classic machine learning.
- **[d2l-ai/d2l-en](https://github.com/d2l-ai/d2l-en)** (~29.9k) · *Course*
  Interactive deep learning book with code in several frameworks.
- **[fastai/fastbook](https://github.com/fastai/fastbook)** (~25.4k) · *Course*
  The fastai book, published as Jupyter notebooks.
- **[eugeneyan/applied-ml](https://github.com/eugeneyan/applied-ml)** (~30.6k) · *Reference*
  Curated papers and tech blogs from companies applying data science and ML in production. A reading list, not code.

---

## Python packages (not the most famous)

Pip-installable libraries. The most famous ones (pandas, NumPy, scikit-learn, PyTorch, TensorFlow, Keras, Hugging Face Transformers, LangChain, spaCy, XGBoost, PyTorch Lightning) are left out.

| Package | Stars (~) | Use | Repo |
|---|---|---|---|
| Ray | 44.1k | Distributed compute for ML and batch workloads | [ray-project/ray](https://github.com/ray-project/ray) |
| Polars | 40.1k | Fast DataFrame engine (Rust core, Python API) for batch processing | [pola-rs/polars](https://github.com/pola-rs/polars) |
| DuckDB | 42.3k | In-process analytical SQL database for files and DataFrames | [duckdb/duckdb](https://github.com/duckdb/duckdb) |
| LlamaIndex | 52.6k | Document processing and RAG framework | [run-llama/llama_index](https://github.com/run-llama/llama_index) |
| Haystack | 26.8k | Framework for LLM pipelines, RAG, and agent workflows | [deepset-ai/haystack](https://github.com/deepset-ai/haystack) |
| crewAI | 59.9k | Framework for orchestrating role-based, multi-agent systems | [crewAIInc/crewAI](https://github.com/crewAIInc/crewAI) |
| mem0 | 67.4k | Memory layer for AI agents and apps | [mem0ai/mem0](https://github.com/mem0ai/mem0) |
| Prophet | 20.4k | Time series forecasting (see [section 6](#6-time-series-forecasting)) | [facebook/prophet](https://github.com/facebook/prophet) |
| Ultralytics | 62.6k | YOLO models for detection, segmentation, and tracking (see [section 3](#3-computer-vision)) | [ultralytics/ultralytics](https://github.com/ultralytics/ultralytics) |
| Supervision | 51.2k | Computer vision utilities for detections, tracking, and video (see [section 3](#3-computer-vision)) | [roboflow/supervision](https://github.com/roboflow/supervision) |
| EasyOCR | 30.1k | OCR in 80+ languages (see [section 4](#4-ocr--document-ai)) | [JaidedAI/EasyOCR](https://github.com/JaidedAI/EasyOCR) |

## Notes

- **Below the 20k threshold and left out:** LightGBM (~18.9k), Unstructured (~15.6k), `ageron/handson-ml3` (~14.3k), docTR (~6.4k), `Nixtla/statsforecast` (~4.9k).
- **Gaps:** recommendation and time series have few repositories above 20k. Those sections are short on purpose.
- **Verification:** star counts are rounded (for example "22.0k") and come from public GitHub pages. Check the live page before relying on an exact number.
