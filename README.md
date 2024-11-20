
# KaggleX Fellowship Chatbot Project

<div align="center">
  <p><img src="icons/KaggleX_Chatbot_Logo.png" alt="Project Logo" width="500"></p>
</div>

## Proposal

### 1. Problem Area
This project focuses on developing a conversational chatbot tailored to provide accurate and context-sensitive information within the medical domain. The goal is to address key challenges in disseminating reliable medical knowledge to two primary audiences: 
- Patients seeking clear, trustworthy answers about medical conditions and treatments.
- Healthcare professionals (education and training): To assist in learning and decision-making.

### 2. Users and Benefits
The key intended users are:
- **Patients**: To help them understand medical conditions without overwhelming them with technical jargon.
- **Healthcare Practitioners**: To assist in clinical training by providing fast, reliable references for decision-making.

By tailoring the chatbot’s behavior to these groups, the project aims to:
- Empower patients with accessible, accurate medical knowledge.
- Enhance the efficiency of healthcare professionals' training and empowerment, saving valuable time.

### 3. Core Impact
The chatbot has the potential to:
- **Improve Patient Outcomes**: By bridging the knowledge gap between patients and healthcare providers.
- **Enhance Medical Education Efficiency**: By quickly providing healthcare professionals with accurate information.
- **Build Trust in AI**: By emphasizing transparency and reliability in responses.

---

## Project Details

### Dataset
- **Source**: [Hugging Face Medical-Llama3 Fine-tune Dataset](https://huggingface.co/datasets/Pistachio-LLM/Medical-llama3-finetune-train)
- **Description**: A curated collection of medical conversation data, designed for fine-tuning language models in the healthcare domain.
- **Justification**: This dataset was chosen for its depth, diversity, and medical focus, making it ideal for training a chatbot that needs both domain-specific expertise and conversational adaptability.

### Model and Fine-Tuning
- **Base Model**: Gemma 2B model, chosen for its balance of size, performance, and suitability for running smaller, localized instances while leveraging cloud-based solutions like GCP for scaling.
- **Fine-Tuning Strategy**:
  - Leveraged the dataset to adapt the base model for medical context.
  - Focused on aligning responses with user needs—differentiating between patient-friendly explanations and clinical terminology.

### Experimental Setup
- **Local vs. Cloud**: The chatbot can operate both as a lightweight local instance for private use and a robust cloud-deployed service for broader access.
- **Tracking Progress**: Experimentation was tracked using comprehensive metrics, ensuring reproducibility and gradual improvement.

---

## Project Results

### Validation and Metrics
To ensure the chatbot meets its intended purpose:
- **Accuracy**: Measured using prompt-response pair evaluations and comparison to expert benchmarks.
- **Complex Prompt Testing**: Included edge cases like ambiguous medical queries and multi-layered questions to evaluate the chatbot’s reasoning capabilities.
- **Limitations**: Known challenges include occasional overconfidence in uncertain responses and difficulty with highly specialized medical terminology.

---

## Technologies Used
- **Hugging Face**: For dataset access and fine-tuning tools.
- **Keras**: For model customization and training.
- **Gemma**: Selected as the base LLM model for its robust capabilities and suitability for medical chatbot applications.
- **LoRA**: Used to fine-tune the large language model efficiently, minimizing computational requirements while preserving model performance.
- **Google Cloud Platform (GCP)**: For scalable deployment and experimentation.


---

## Reproducibility
- All dependencies are captured in an `environment.yml` file for quick setup.
- Code is modularized for ease of experimentation and scalability.
- Instructions for running the chatbot locally or on GCP are included.

### How to Run
1. Clone this repository.
2. Set up the environment using:
   ```bash
   conda env create -f environment.yml
   ```
3. Follow the instructions in the notebook `Rebuilt_LoRA_Notebook.ipynb` to load the dataset and run the model.

---

## Deliverables
1. **Presentation Slide Deck**: Overview of project goals, methodology, and results.
2. **YouTube Video**: Demonstration of chatbot capabilities with various user types.

---

## Next Steps
1. **Expand Dataset Coverage**: Incorporate additional medical datasets to enhance chatbot diversity and expertise.
2. **Advanced Testing**: Develop specific metrics for conversational fluency and error handling.
3. **User Feedback Loop**: Deploy pilot versions for patients and practitioners to gather real-world feedback.

---
