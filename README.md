📚 Project Title

Evaluation of Psychological Counselling Using Locally Deployed LLMs
🧠 Project Overview

This project aims to investigate the feasibility and effectiveness of using locally deployed open-source Large Language Models (LLMs), such as Llama 3, to automate the evaluation of psychological counselling sessions.
The evaluation is based on the Consultation Interactions Coding Scheme (CICS), with the goal of reducing the time and cost required for therapist feedback while preserving patient data privacy.

Key Features:

    Local model deployment: No patient data is sent to external cloud services.

    CICS-based analysis: Predict therapy outcomes based on coded patient-therapist interactions.

    Ethical compliance: Data anonymization and responsible AI practices applied.

📂 Project Structure

P216_Qing_EvalCounsellingLLM/
├── code/              # Core scripts for data processing and model interaction

├── data/              # Anonymized raw and processed counselling session datasets

├── notebooks/         # Jupyter Notebooks for exploration and prototyping

├── models/            # Pretrained LLMs and fine-tuned versions

├── results/           # Evaluation outputs and visualizations

├── reports/           # Project proposal, final report, and presentations

├── ethics/            # IRB documents, consent forms, anonymization scripts

├── references/        # Academic references and reading materials

└── README.md          # Project overview and usage instructions

🛠️ How to Run
1. Environment Setup

Install the necessary dependencies:

pip install -r requirements.txt

Recommended environment:

    Python 3.10+

    PyTorch

    Huggingface Transformers

    BitsAndBytes (for Llama quantized models)

    JupyterLab (optional for notebooks)

2. Prepare Data

    Place anonymized counselling transcripts under data/raw/.

    Preprocess the data:

python code/data_preprocess.py

3. Run LLM Evaluation

Run CICS-based prediction:

python code/run_cics_llm.py

This will load the locally installed Llama 3 model, process the sessions, and generate CICS code predictions.
4. View Results

Evaluation outputs will be saved to:

results/eval_outputs.csv
results/visualisations/

You can visualize session interaction metrics using provided Jupyter notebooks.
🔐 Ethics and Data Protection

    All counselling data is fully anonymized prior to processing.

    No personally identifiable information (PII) is stored or shared.

    This project follows institutional guidelines and has IRB/ethics committee approval documentation in the ethics/ folder.

📑 References

    Consultation Interactions Coding Scheme (CICS)

    Developing an Automated Assessment of In-session Patient Activation for Psychological Therapy

    ExTRAPPOLATE Project: Responsible AI Research in Psychological Therapy

    Meta AI (2023): Llama 2/3 Technical Report

📈 Future Work

    Fine-tuning Llama 3 on domain-specific therapy dialogues.

    Expanding classification beyond CICS, e.g., Lacanian discourse markers.

    Developing a real-time therapist feedback tool with UI integration.

🧑‍💻 Contact

Project Author: Qing
Supervisor: Dr. Kai Xu
Summer MSc Final Project 2025
