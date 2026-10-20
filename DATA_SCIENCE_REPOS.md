# Top Data Science Repositories

A reference list of popular data-science repositories on GitHub, organized by field and by business application. The focus is on **systems, implementations, examples, and ready-to-run projects** rather than bare libraries.

## How this list is built

- **Popularity is a guide, not a cutoff.** Star counts are shown so you can gauge how established a project is. Entries are not dropped for falling below a fixed number.
- **Classics are included** even when they are a single reference point in a niche.
- **Small fields stay useful.** Where a niche has few widely starred projects (time series, optimization, causal inference), the sections include the strongest available options, even when they have only a few thousand stars.
- **Star counts** are approximate, rounded values read from public GitHub pages in October 2026. They change over time.
- **Python packages** are indexed in their own section at the end. Each one links back to the field where it is discussed.
- Each entry is tagged with its type: **System**, **Implementation**, **Examples**, **Course**, **Library**, **Model**, or **Reference**.

## Field map

| Field | Business applications | Section |
|---|---|---|
| Recommendation systems | Product recommendations, personalization, e-commerce | [1](#1-recommendation-systems) |
| RAG & LLM applications | Internal knowledge bases, document Q&A, support copilots, AI agents | [2](#2-rag--llm-applications) |
| Computer vision | Quality inspection, object detection, segmentation, video analytics | [3](#3-computer-vision) |
| OCR & document AI | Invoice and form extraction, digitizing archives, feeding documents to LLMs | [4](#4-ocr--document-ai) |
| Big data & batch processing | ETL at scale, PySpark batch jobs, pipeline orchestration | [5](#5-big-data--batch-processing) |
| Time series forecasting | Demand, sales, and capacity forecasting | [6](#6-time-series-forecasting) |
| Optimization & mathematical programming | Scheduling, routing, planning, resource allocation, pricing | [7](#7-optimization--mathematical-programming) |
| Anomaly detection & causal inference | Fraud and quality monitoring, uplift modeling, measuring impact | [8](#8-anomaly-detection--causal-inference) |
| BI & data apps | Dashboards, internal tools, ML demos | [9](#9-bi--data-apps) |
| MLOps | Experiment tracking, model registry, deployment | [10](#10-mlops) |
| Speech | Call-center transcription, voice interfaces | [11](#11-speech) |
| Tabular machine learning | Churn, credit scoring, demand features, pricing models | [12](#12-tabular-machine-learning) |
| Learning & reference | Learning ML in practice, deep learning, ML in production | [13](#13-learning--reference) |
| Python packages | Index of pip-installable libraries from every section | [Python packages](#python-packages-index) |

---

## 1. Recommendation systems

- **[microsoft/recommenders](https://github.com/microsoft/recommenders)** (~22.0k) · *Examples*
  Best-practice notebooks and utilities covering collaborative filtering, content-based, and deep learning recommenders, plus evaluation. Under the Linux Foundation for AI & Data.
- **[RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole)** (~4.6k) · *Library*
  Unified, comprehensive library for reproducing and developing recommendation algorithms in PyTorch. Useful for comparing many models on the same data.
- **[tensorflow/recommenders](https://github.com/tensorflow/recommenders)** (~2.0k) · *Library*
  Library for building recommender models with TensorFlow, including two-tower retrieval models.
- **[NVIDIA-Merlin/Merlin](https://github.com/NVIDIA-Merlin/Merlin)** (~0.9k) · *System*
  End-to-end, GPU-accelerated recommender pipeline: feature engineering, preprocessing, model training, and production inference.

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

- **[ultralytics/ultralytics](https://github.com/ultralytics/ultralytics)** (~62.6k) · *Library* · see [Python packages](#python-packages-index)
  YOLO models for detection, segmentation, classification, pose estimation, and tracking. Production-oriented and easy to adopt.
- **[facebookresearch/segment-anything](https://github.com/facebookresearch/segment-anything)** (~55.0k) · *Implementation*
  Inference code, checkpoints, and example notebooks for the Segment Anything Model (SAM). Useful for labeling and object-segmentation workflows.
- **[facebookresearch/detectron2](https://github.com/facebookresearch/detectron2)** (~34.9k) · *System*
  Platform for object detection, segmentation, and other visual recognition tasks.
- **[opencv/opencv](https://github.com/opencv/opencv)** (~91.2k) · *Library*
  The foundational open-source computer vision library. Used as a building block in most CV pipelines.
- **[roboflow/supervision](https://github.com/roboflow/supervision)** (~51.2k) · *Library* · see [Python packages](#python-packages-index)
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
- **[JaidedAI/EasyOCR](https://github.com/JaidedAI/EasyOCR)** (~30.1k) · *Library* · see [Python packages](#python-packages-index)
  Ready-to-use OCR with 80+ languages and many writing systems.
- **[mindee/doctr](https://github.com/mindee/doctr)** (~6.4k) · *Library*
  Deep learning OCR toolkit (document text detection and recognition). A smaller, focused option for building custom OCR pipelines.
- **[Unstructured-IO/unstructured](https://github.com/Unstructured-IO/unstructured)** (~15.6k) · *Library*
  Converts complex documents (PDFs, HTML, office files) into structured elements for LLM and search pipelines.

## 5. Big data & batch processing

- **[apache/spark](https://github.com/apache/spark)** (~44.2k) · *System*
  Unified analytics engine for large-scale data processing. **PySpark** (the `python/` directory) is the standard way to run batch jobs from Python.
- **[apache/airflow](https://github.com/apache/airflow)** (~47.2k) · *System*
  Platform to author, schedule, and monitor data pipelines. The usual orchestrator for nightly batch jobs.
- **Ray, Polars, DuckDB** are indexed in [Python packages](#python-packages-index) as alternatives for distributed or single-machine batch processing.

## 6. Time series forecasting

- **[google-research/timesfm](https://github.com/google-research/timesfm)** (~34.6k) · *Model*
  Pretrained time-series foundation model from Google Research for zero-shot forecasting of univariate and multivariate series, with covariates and quantile outputs. Runs on PyTorch (or MLX on Apple silicon).
- **[facebook/prophet](https://github.com/facebook/prophet)** (~20.4k) · *Library*
  Forecasting tool for series with multiple seasonality and linear or non-linear growth. A long-standing business default.
- **[sktime/sktime](https://github.com/sktime/sktime)** (~10.1k) · *Library*
  Unified framework for machine learning with time series: forecasting, classification, and more, behind one interface.
- **[unit8co/darts](https://github.com/unit8co/darts)** (~9.6k) · *Library*
  User-friendly forecasting and anomaly detection on time series, with many classical and deep learning models behind one API.
- **[amazon-science/chronos-forecasting](https://github.com/amazon-science/chronos-forecasting)** (~6.2k) · *Model*
  Pretrained forecasting models (Chronos-2, Chronos-Bolt, and the original Chronos) for zero-shot forecasting.
- **[Nixtla/statsforecast](https://github.com/Nixtla/statsforecast)** (~4.9k) · *Library*
  Fast statistical and econometric forecasting models, including classical methods such as ARIMA and ETS, for large numbers of series.
- **[Nixtla/neuralforecast](https://github.com/Nixtla/neuralforecast)** (~4.3k) · *Library*
  Neural forecasting algorithms with a common, scalable interface.
- **[ourownstory/neural_prophet](https://github.com/ourownstory/neural_prophet)** (~4.3k) · *Library*
  Interpretable, PyTorch-based forecasting that combines neural networks with classical time-series components.

## 7. Optimization & mathematical programming

Optimization splits into a **modeling layer** (you write the problem) and a **solver layer** (it finds the answer). Several entries below are modeling languages that call one or more solvers.

- **[google/or-tools](https://github.com/google/or-tools)** (~14.2k) · *System*
  Google's suite of combinatorial optimization tools: routing, scheduling, assignment, and CP-SAT for constraint programming. Written in C++ with Python bindings. Strong choice for vehicle routing and shift scheduling.
- **[Pyomo/pyomo](https://github.com/Pyomo/pyomo)** (~2.5k) · *Library*
  Object-oriented algebraic modeling language in Python for linear, mixed-integer, and nonlinear programs. It sends models to external solvers, so it pairs well with HiGHS, CBC, or SCIP.
- **[coin-or/pulp](https://github.com/coin-or/pulp)** (~2.5k) · *Library*
  Linear and mixed-integer programming modeler in Python. Bundles the CBC solver, so it runs with no extra setup.
- **[cvxpy/cvxpy](https://github.com/cvxpy/cvxpy)** (~6.4k) · *Library*
  Python-embedded modeling language for convex optimization problems such as portfolio allocation and resource planning.
- **[coin-or/python-mip](https://github.com/coin-or/python-mip)** (~0.6k) · *Library*
  Python tools for modeling and solving mixed-integer linear programs, with CBC as the default solver.
- **[anyoptimization/pymoo](https://github.com/anyoptimization/pymoo)** (~3.0k) · *Library*
  Framework for multi-objective and single-objective optimization: NSGA-II/III, MOEA/D, differential evolution, CMA-ES, and PSO. Use it when no single objective is clear, such as cost vs. service level.
- **[ERGO-Code/HiGHS](https://github.com/ERGO-Code/HiGHS)** (~1.9k) · *System*
  Open-source solver for linear, quadratic, and mixed-integer programming. Callable from Python, and a solid open-source default for LP/MIP.
- **[coin-or/Cbc](https://github.com/coin-or/Cbc)** (~1.0k) · *System*
  COIN-OR branch-and-cut solver for mixed-integer linear programs. The solver behind PuLP's default setup.
- **[scipopt/scip](https://github.com/scipopt/scip)** (~0.7k) · *System*
  Solver for mixed-integer programming and nonlinear extensions, plus a framework for constraint integer programming and branch-cut-and-price. Strong on hard MIP instances.
- **[jump-dev/JuMP.jl](https://github.com/jump-dev/JuMP.jl)** (~2.5k) · *Library*
  Modeling language for mathematical optimization in **Julia** (linear, mixed-integer, conic, and nonlinear). Included as the main non-Python counterpart to Pyomo.

## 8. Anomaly detection & causal inference

- **[yzhao062/pyod](https://github.com/yzhao062/pyod)** (~10.1k) · *Library*
  Anomaly detection with 60+ detectors across tabular, time series, graph, text, image, and audio data. Useful for fraud, quality, and monitoring alerts.
- **[py-why/dowhy](https://github.com/py-why/dowhy)** (~8.4k) · *Library*
  Causal inference that makes assumptions explicit and tests them. Good fit for "what would have happened without the change" questions.
- **[uber/causalml](https://github.com/uber/causalml)** (~6.0k) · *Library*
  Uplift modeling and conditional average treatment effect (CATE) estimation. Used for targeting marketing or retention actions where the goal is incremental impact.

## 9. BI & data apps

- **[apache/superset](https://github.com/apache/superset)** (~75.2k) · *System*
  Data visualization and exploration platform for dashboards over SQL databases. A self-hosted BI tool.
- **[metabase/metabase](https://github.com/metabase/metabase)** (~49.7k) · *System*
  Business intelligence and embedded analytics tool that lets non-technical users query data.
- **[streamlit/streamlit](https://github.com/streamlit/streamlit)** (~46.0k) · *Library*
  Build and share data apps in Python. Common for internal tools and model demos.
- **[gradio-app/gradio](https://github.com/gradio-app/gradio)** (~43.8k) · *Library*
  Build and share ML apps and demos in Python.

## 10. MLOps

- **[mlflow/mlflow](https://github.com/mlflow/mlflow)** (~28.4k) · *System*
  Open-source AI engineering platform for experiment tracking, model registry, and evaluation of agents, LLMs, and ML models.

## 11. Speech

- **[openai/whisper](https://github.com/openai/whisper)** (~110.8k) · *Implementation*
  Robust speech recognition trained on large-scale weakly supervised data. Used for transcription in call-center and meeting-analysis pipelines.

## 12. Tabular machine learning

- **[dmlc/xgboost](https://github.com/dmlc/xgboost)** (~28.9k) · *Library*
  Scalable gradient boosting for classification, regression, and ranking. Runs on a single machine or distributed systems such as Spark, Dask, and Flink.
- **[microsoft/LightGBM](https://github.com/microsoft/LightGBM)** (~18.9k) · *Library*
  Fast, distributed gradient boosting framework built on decision trees. A common choice for large tabular datasets.

## 13. Learning & reference

- **[jakevdp/PythonDataScienceHandbook](https://github.com/jakevdp/PythonDataScienceHandbook)** (~50.2k) · *Examples*
  Full text in Jupyter notebooks: NumPy, pandas, Matplotlib, and scikit-learn.
- **[microsoft/ML-For-Beginners](https://github.com/microsoft/ML-For-Beginners)** (~91.6k) · *Course*
  12 weeks, 26 lessons, 52 quizzes on classic machine learning.
- **[d2l-ai/d2l-en](https://github.com/d2l-ai/d2l-en)** (~29.9k) · *Course*
  Interactive deep learning book with code in several frameworks.
- **[fastai/fastbook](https://github.com/fastai/fastbook)** (~25.4k) · *Course*
  The fastai book, published as Jupyter notebooks.
- **[ageron/handson-ml3](https://github.com/ageron/handson-ml3)** (~14.3k) · *Course*
  Hands-on machine learning and deep learning in Jupyter notebooks, using scikit-learn, Keras, and TensorFlow.
- **[eugeneyan/applied-ml](https://github.com/eugeneyan/applied-ml)** (~30.6k) · *Reference*
  Curated papers and tech blogs from companies applying data science and ML in production. A reading list, not code.

---

## Python packages index

Pip-installable libraries from the sections above, plus a few others. Only the ubiquitous base tools are left out (pandas, NumPy, scikit-learn, PyTorch, TensorFlow, Keras, Hugging Face Transformers, LangChain, spaCy, PyTorch Lightning). Gradient-boosting classics are kept because they are standard in business modeling.

| Package | Stars (~) | Use | Where it's discussed |
|---|---|---|---|
| [XGBoost](https://github.com/dmlc/xgboost) | 28.9k | Gradient boosting for tabular data | [Tabular ML](#12-tabular-machine-learning) |
| [LightGBM](https://github.com/microsoft/LightGBM) | 18.9k | Fast gradient boosting for tabular data | [Tabular ML](#12-tabular-machine-learning) |
| [docTR](https://github.com/mindee/doctr) | 6.4k | Deep learning OCR toolkit | [OCR](#4-ocr--document-ai) |
| [Unstructured](https://github.com/Unstructured-IO/unstructured) | 15.6k | Converts documents into structured data for LLM pipelines | [OCR](#4-ocr--document-ai) |
| [Ray](https://github.com/ray-project/ray) | 44.1k | Distributed compute for ML and batch workloads | [Big data](#5-big-data--batch-processing) |
| [Polars](https://github.com/pola-rs/polars) | 40.1k | Fast DataFrame engine (Rust core, Python API) | [Big data](#5-big-data--batch-processing) |
| [DuckDB](https://github.com/duckdb/duckdb) | 42.3k | In-process analytical SQL database for files and DataFrames | [Big data](#5-big-data--batch-processing) |
| [LlamaIndex](https://github.com/run-llama/llama_index) | 52.6k | Document processing and RAG framework | [RAG](#2-rag--llm-applications) |
| [Haystack](https://github.com/deepset-ai/haystack) | 26.8k | Framework for LLM pipelines, RAG, and agent workflows | [RAG](#2-rag--llm-applications) |
| [crewAI](https://github.com/crewAIInc/crewAI) | 59.9k | Role-based, multi-agent orchestration | [RAG](#2-rag--llm-applications) |
| [mem0](https://github.com/mem0ai/mem0) | 67.4k | Memory layer for AI agents and apps | [RAG](#2-rag--llm-applications) |
| [Ultralytics](https://github.com/ultralytics/ultralytics) | 62.6k | YOLO detection, segmentation, and tracking | [Computer vision](#3-computer-vision) |
| [Supervision](https://github.com/roboflow/supervision) | 51.2k | Detections, tracking, and video utilities | [Computer vision](#3-computer-vision) |
| [EasyOCR](https://github.com/JaidedAI/EasyOCR) | 30.1k | OCR in 80+ languages | [OCR](#4-ocr--document-ai) |
| [Prophet](https://github.com/facebook/prophet) | 20.4k | Time series forecasting | [Time series](#6-time-series-forecasting) |
| [TimesFM](https://github.com/google-research/timesfm) | 34.6k | Pretrained time-series foundation model | [Time series](#6-time-series-forecasting) |
| [sktime](https://github.com/sktime/sktime) | 10.1k | Unified ML framework for time series | [Time series](#6-time-series-forecasting) |
| [Darts](https://github.com/unit8co/darts) | 9.6k | Forecasting and anomaly detection | [Time series](#6-time-series-forecasting) |
| [Chronos](https://github.com/amazon-science/chronos-forecasting) | 6.2k | Pretrained forecasting models | [Time series](#6-time-series-forecasting) |
| [statsforecast](https://github.com/Nixtla/statsforecast) | 4.9k | Classical statistical forecasting at scale | [Time series](#6-time-series-forecasting) |
| [NeuralForecast](https://github.com/Nixtla/neuralforecast) | 4.3k | Neural forecasting models | [Time series](#6-time-series-forecasting) |
| [NeuralProphet](https://github.com/ourownstory/neural_prophet) | 4.3k | Interpretable neural forecasting | [Time series](#6-time-series-forecasting) |
| [OR-Tools](https://github.com/google/or-tools) | 14.2k | Routing, scheduling, and CP-SAT | [Optimization](#7-optimization--mathematical-programming) |
| [Pyomo](https://github.com/Pyomo/pyomo) | 2.5k | Algebraic modeling for LP, MIP, and NLP | [Optimization](#7-optimization--mathematical-programming) |
| [PuLP](https://github.com/coin-or/pulp) | 2.5k | LP and MIP modeling, bundles CBC | [Optimization](#7-optimization--mathematical-programming) |
| [CVXPY](https://github.com/cvxpy/cvxpy) | 6.4k | Convex optimization modeling | [Optimization](#7-optimization--mathematical-programming) |
| [python-mip](https://github.com/coin-or/python-mip) | 0.6k | MIP modeling and solving | [Optimization](#7-optimization--mathematical-programming) |
| [pymoo](https://github.com/anyoptimization/pymoo) | 3.0k | Multi-objective optimization | [Optimization](#7-optimization--mathematical-programming) |
| [PyOD](https://github.com/yzhao062/pyod) | 10.1k | Anomaly detection | [Anomaly & causal](#8-anomaly-detection--causal-inference) |
| [DoWhy](https://github.com/py-why/dowhy) | 8.4k | Causal inference | [Anomaly & causal](#8-anomaly-detection--causal-inference) |
| [CausalML](https://github.com/uber/causalml) | 6.0k | Uplift modeling and CATE | [Anomaly & causal](#8-anomaly-detection--causal-inference) |
| [RecBole](https://github.com/RUCAIBox/RecBole) | 4.6k | Recommendation algorithms | [Recommendation](#1-recommendation-systems) |
| [TF Recommenders](https://github.com/tensorflow/recommenders) | 2.0k | Recommender models in TensorFlow | [Recommendation](#1-recommendation-systems) |
| [Merlin](https://github.com/NVIDIA-Merlin/Merlin) | 0.9k | GPU-accelerated recommender pipeline | [Recommendation](#1-recommendation-systems) |

## Notes

- **Optimization tip:** pair a modeling language (Pyomo, PuLP, python-mip, CVXPY) with a solver (HiGHS, CBC, SCIP, or OR-Tools' CP-SAT) based on problem type. Start with OR-Tools for routing and scheduling, and with HiGHS or CBC for LP and MIP.
- **Star counts are approximate.** They are rounded (for example "22.0k") and read from public GitHub pages. Check the live page before relying on an exact number.
- **Classic kept for reference:** `ageron/handson-ml3` (~14.3k) is a widely used hands-on ML book in notebooks; it is a strong option for beginners.
