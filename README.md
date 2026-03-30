🚀  AI TEXT DETECTOR USING DISTILBERT

<p align="center">
  <b>Detect whether a piece of text is Human-written or AI-generated</b><br>
  Built with Transformers · Deployed on Hugging Face 🚀
</p>

📌 OVERVIEW:-

This project presents a high-performance NLP model that classifies text as Human-written or AI-generated using a fine-tuned DistilBERT architecture.

It is designed to handle diverse writing styles and provides real-time predictions through a deployed web application.


✨ FEATURES:-

•	🧠 Transformer-based text classification (DistilBERT)
	
•	⚡ Fast and lightweight inference
	
•	🌐 Live deployed web app (Hugging Face Spaces)
	
•	📊 High accuracy on real-world datasets
	
•	🔍 Handles both formal and informal text styles

🧠 HOW THE MODEL WORKS:-

🔹 1. Input Processing

•	The input text is tokenized using a pretrained tokenizer.

•	Text is converted into numerical representations (input IDs + attention masks).

•	Sequence length is limited (e.g., 128 tokens) for efficient processing.


🔹 2. Contextual Understanding (DistilBERT)

•	The tokenized input is passed through DistilBERT, a transformer-based model.

•	It uses self-attention mechanisms to understand relationships between words.

•	Instead of reading text sequentially, it captures global context across the sentence.


🔹 3. Feature Extraction

•	The model generates contextual embeddings for the entire sentence.

•	These embeddings capture:
	Writing style
	Sentence structure
	Linguistic patterns


🔹 4. Classification Layer

•	A fully connected layer (classification head) is applied on top of DistilBERT.

•	It outputs logits for two classes:

•	0 → Human

•	1 → AI


🔹 5. Probability & Prediction

•	Logits are converted into probabilities using Softmax.

•	The class with highest probability is selected:

	pred = argmax(softmax(logits))

🔹 6. Learning Patterns

During training, the model learns to distinguish:

✔ Human text:

•	More variability

•	Imperfections / inconsistencies

•	Less uniform structure

✔ AI-generated text:

•	More structured and consistent

•	Repetitive phrasing patterns

•	Higher grammatical uniformity


🔹 7. Decision Making

Final prediction is based on learned patterns such as:

•	Sentence fluency

•	Structural consistency

•	Repetition patterns

•	Context coherence


📊 MODEL PERFORMANCE:

            	  precision    recall  f1-score   support

        		0       1.00      0.96      0.98      1751
         	 	1       0.95      1.00      0.97      1164

  		  accuracy                           0.98      2915
  		macro avg       0.97      0.98       0.97      2915
		weighted avg    0.98      0.98       0.98      2915

⚠️ Note: Performance may vary on adversarial or highly edited AI text.



🔗 Try the app here:

	 https://huggingface.co/spaces/sahil077/spacenew

🤖 MODEL REPOSITORY:

 	https://huggingface.co/sahil077/ai-text-detector

⚙️ INSTALLATION

	pip install -r requirements.txt

📁 PROJECT STRUCTURE:

	ai-text-detector/
	│
	├── app.py              # Inference script
	├── train.p             # Training pipeline
	├── requirements.txt
	├── License
	├── notebookai2txt.ipynb
	├── README.md
	└── .gitignore

Installation:

	pip install -r requirements.txt


🧠 TECH STACK:-

•	Python 🐍

•	PyTorch 🔥

•	Hugging Face Transformers 🤗

•	Gradio (for UI)



📈 FUTURE IMPROVEMENTS:-

•	Improve robustness on adversarial AI text

•	Add ensemble models (BERT, RoBERTa)

•	Expand dataset diversity

•	Fine-tune on longer context inputs


🔐 License:

This project is intended for academic and research purposes.


👨‍💻 Author

Sahil Kumar

B.E. Robotics and Artificial Intelligence

Sir M. Visvesvaraya Institute of Technology, Bengaluru






