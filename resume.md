# Shivam Sharma

0435188859 | shivzzzzzz02@gmail.com | [LinkedIn](https://linkedin.com/in/shivam-sharma-6272b8245) | [GitHub](https://github.com/jxm020202) | Perth, Australia

---

## Technical Skills

- **Languages:** Python, Go, SQL, R, Java, TypeScript
- **ML / AI:** PyTorch, HuggingFace Transformers, PEFT (LoRA/QLoRA), scikit-learn, LightGBM, ONNX, TensorFlow/Keras, YOLOv5, OpenAI API, LangChain, LLM structured outputs, prompt engineering, RAG
- **MLOps & Experiment Tracking:** SageMaker (notebooks, model training, GPU instances), MLflow, Weights & Biases, ONNX Runtime, model versioning (S3), INT8 quantization, Label Studio
- **Cloud & Infrastructure:** AWS (Lambda, SQS, S3, Bedrock, EKS, ECR, RDS, SageMaker, CloudWatch, Secrets Manager, KMS), Terraform, Docker, Kubernetes, GitHub Actions CI/CD
- **Data & Tools:** PostgreSQL, pgvector, Redshift, FastAPI, pandas, NumPy, Git, REST APIs, microservices architecture, event-driven systems, Jira, Confluence

---

## Experience & Projects

### WeMoney — ML Engineer
**Perth, Australia | Nov 2025 – Present**

#### Merchant Enrichment Pipeline
- Designed and built an event-driven system from scratch that resolves raw transaction descriptions to structured merchant data (name, website, logo, category) using web search, LLM reasoning with structured outputs (AWS Bedrock), and automated logo scraping with headless Chromium.
- Implemented hexagonal (ports & adapters) architecture in Go with 6 interface ports, enabling full mock-based unit testing (29 tests) with zero infrastructure dependencies.
- Built a multi-stage entity deduplication pipeline combining exact matching, fuzzy similarity scoring, and LLM-based semantic matching to reduce duplicate records by 90%+.

#### ML Categorization Platform
- Own the transaction categorization service end-to-end — a custom transformer model (TXFormer) trained on SageMaker with multi-source labelling (human annotations, MCC codes, embeddings, LLM-generated labels, rule-based labels), exported to ONNX with INT8 quantization, and served on EKS processing thousands of daily transactions.
- Contributed to the model training data pipeline — human labelling on Label Studio and a self-hosted portal, with inter-annotator disagreement tracking and iterative label quality improvement across multiple training cycles.
- Operate the EKS-deployed categorization service — Helm deployments, pod scaling, health checks, and cross-service integration via SQS between Lambda and EKS workloads.

#### Predictive Modelling & Data Science
- Built prediction pipelines on SageMaker using logistic regression, WOE/IV feature ranking, and case-based reasoning, informing product decisions on user eligibility scoring.

#### Cloud Infrastructure & DevOps
- Authored all Terraform for Lambda, SQS FIFO queues (with DLQ), ECR, IAM roles, and CloudWatch monitoring. Built GitHub Actions CI/CD with automated build, lint, test, and multi-environment deployment (dev/prod). Managed secrets management (AWS Secrets Manager) and encryption at rest (KMS).

### Multilingual Chatbot Arena — WSDM Cup 2025
**Dec 2024 – Jan 2025**

- Built a human preference prediction model (reward model for RLHF) by fine-tuning Gemma-2 9B using QLoRA (4-bit NF4 quantization, rank-64 LoRA on layers 16–41) across dual GPUs.
- Rapid prototyping across 3 approaches: classical ML baseline (LightGBM + TF-IDF + feature engineering), DeBERTa multilingual encoder embeddings, then end-to-end LLM fine-tuning with progressive scaling (128→1000 token context, 240→2400 training samples).
- Engineered dual-GPU parallel inference with ThreadPoolExecutor, test-time augmentation (response swapping to cancel position bias), and smart token budget splitting across prompt and responses.
- Used HuggingFace ecosystem end-to-end: Transformers, PEFT, Accelerate, Datasets, bitsandbytes for 4-bit quantization, and Keras-NLP for DeBERTa embedding extraction.

### Norwood Systems (ASX: NOR) — Data Science Intern
**Perth, Australia | Jul 2024 – Dec 2024**

- Engineered PCA-based evaluation frameworks for chatbot systems, reducing high-dimensional conversation data to key performance drivers and enabling targeted system improvements.
- Created custom voice- and text-based chatbot metrics (user satisfaction, response accuracy, conversation flow coherence) adopted as the team's standard evaluation suite, replacing ad-hoc manual reviews.
- Built analysis pipelines in Python (pandas, NumPy, matplotlib) to process conversation logs and generate automated performance reports across multiple chatbot configurations.
- Containerized the evaluation service using Docker, enabling reproducible deployment and consistent results across development and staging environments.
- Led the chatbot evaluation workstream, coordinating tasks across a small team and ensuring consistent delivery of analytical outputs to stakeholders.

### Cerence Inc. — Software Engineer
**Pune, India | Jan 2023 – Jul 2023**

- Optimized backend systems and SQL queries for Cerence Studio, an in-car voice assistant platform used by major automotive OEMs, improving real-time analytics and reporting capabilities for enterprise clients.
- Implemented Test-Driven Development (TDD) practices, writing comprehensive unit and integration tests prior to feature development, resulting in substantially fewer production bugs and faster release cycles.
- Developed and tested RESTful API endpoints using Postman, improving interoperability between microservices in a distributed backend architecture.
- Leveraged Docker for containerization, streamlining development and deployment pipelines across multiple environments with consistent build reproducibility.
- Worked in an Agile environment using Jira for sprint planning and Confluence for technical documentation, contributing to Cerence Studio being recognized as a top-7 product company-wide.

### Object Detection for Visually Impaired — Symbiosis University
**Pune, India | Jan 2022 – Dec 2023** | *ML Researcher*

- Led a 3-person team to build a real-time object detection system for visually impaired navigation, fine-tuning YOLOv5 to 95–98% accuracy on high-priority object classes.
- Conducted comparative analysis of YOLO architectures (v3–v5), evaluating detection speed, accuracy, and model size tradeoffs including lightweight mobile-optimised variants for edge deployment. Published findings in IJACSA (Vol. 14, Issue 6).
- Built end-to-end ML pipeline: multi-dataset integration (COCO, Pascal VOC, ImageNet), extensive data augmentation and annotation on Roboflow, model training on Google Colab, and experiment tracking with Weights & Biases.

### Algorithmic Trading Bot — QFIN Trading Team / UWA
**Perth, Australia | 2025**

- Built a Bitcoin SMA-crossover trading bot in Python with a custom Differential Evolution optimizer (implemented from scratch) for automated strategy parameter tuning across historical data.
- Developed backtesting engine with transaction fee simulation, chronological train/test splitting, and convergence analysis to validate strategy robustness before deployment.

---

## Education

### University of Western Australia
**Master of Data Science | Global Excellence Scholarship | 2024 – 2025**
- NLP Project (top marks in cohort): Built BiLSTM attention models for aspect-based sentiment classification using TensorFlow/Keras with multi-input architectures (text + POS tags + aspect embeddings)
- Coursework: Machine Learning, NLP, Applied Predictive Modelling, Data Warehousing, AI Adaptive Systems, Relational Databases, Open Source Tools and Scripting
- Certificates: Financial Engineering & Risk Management (Columbia University, Coursera); Fundamentals of Quantitative Modelling (Wharton Online, Coursera)

### Symbiosis Institute of Technology
**B.Tech Computer Science, Honours in AI & ML | 2019 – 2023**
- Research Paper: "State-of-the-Art Analysis of Multiple Object Detection Techniques using Deep Learning" — published in IJACSA (Vol. 14, Issue 6, 2023)
- Coursework: Deep Learning, Neural Networks, Probability Theory, Linear Algebra, Big Data Analytics, Cloud Computing
- GRE Quant: 169/170 | CAT 2022: 99.63 percentile | MAH-CET: 99.81 percentile
- SOF IMO School Gold Medalist (11 & 12) | National Creative Aptitude Test: All India Rank 39 | Aston University x Symbiosis Hackathon Finalist

---

## Co-Curriculars

- **Cricket:** Play for UCC in PSCA (Perth); professional umpire in Perth
- **Chess:** College Team Captain, led inter-college tournaments
- **Volunteering:** Ranked 7th in volunteering hours across UWA
- **University Clubs:** QFIN Trading Team, Programming Society, Coders for Causes, AI Club
- **Sports Meet:** Represented UWA Maali in table tennis, badminton, cricket, and volleyball
