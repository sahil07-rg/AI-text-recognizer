# AITextRecognizer-487K-BART
AI Text Recognizer – A transformer-based NLP model trained on 487K+ samples to classify human-written and AI-generated text. Currently under active development and training optimization.
It is a transformer-based natural language processing (NLP) project designed to classify text as:

	•	Human-written
	•	AI-generated

The model is being trained on a large-scale dataset containing 487,235 text samples sourced from Kaggle.

# 🎯 Project Goal
To build a robust AI detection system capable of distinguishing between:
	•	Authentic human-written content
	•	Machine-generated content (LLMs such as GPT-like systems)

The aim is to develop a scalable and production-ready AI content detection pipeline.

# 🧠 Model Architecture (Current)
	•	Transformer-based architecture (BART / DistilBERT experiments)
	•	Sequence classification setup
	•	Token length: 128–256
	•	Binary classification (0 = Human, 1 = AI)

Model experimentation is ongoing to determine the best architecture-performance tradeoff.

# 📊 Dataset
	•	Total Samples: ~487,000
	•	Labels:
	•	0 → Human-written
	•	1 → AI-generated
	•	Large-scale training for better generalization.

# ⚙️ Current Status

# 🚧 The model is currently under training and optimization.

Ongoing challenges include:

	•	GPU memory optimization
	•	Checkpoint storage management
	•	Training time reduction
	•	Hyperparameter tuning
	•	Evaluation pipeline stabilization

Several configurations are being tested to improve accuracy and training stability.

# 📈 Planned Improvements
	•	Optimize training using lighter transformer models
	•	Hyperparameter tuning
	•	Class imbalance handling
	•	Precision/Recall improvement for human text detection
	•	Model compression for deployment
	•	Web API integration for live text detection

# 🚀 Future Vision
The final goal is to deploy this as:

	•	A web-based AI detection tool
	•	REST API service
	•	Lightweight inference model for real-time detection

# 🛠️ Tech Stack
	•	Python
	•	PyTorch
	•	HuggingFace Transformers
	•	Scikit-learn
	•	Kaggle GPU Environment
