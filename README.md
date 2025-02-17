# 📝 Handwriting Recognition & Document-Based Chatbot

A robust handwriting recognition and document-based chatbot system that integrates classical and deep learning techniques for high-accuracy handwriting recognition and efficient document retrieval. The chatbot enables users to query documents using a conversational interface powered by **FAISS vector store** and **LLaMA2 (CTransformers)**.

## 🚀 Features
- **Handwriting Recognition**: Uses CNNs and BiLSTM for feature extraction and sequence modeling.
- **Vector-Based Document Retrieval**: Converts text into embeddings and stores them in **FAISS** for efficient searching.
- **Conversational Chatbot**: Utilizes `ConversationalRetrievalChain` with **LLaMA2 (CTransformers)** to answer queries.
- **Preprocessing Pipeline**: Grayscale conversion, thresholding, and bounding box detection for better OCR accuracy.
- **Real-Time Response**: The chatbot provides responses based on document content quickly and efficiently.

## 🏗️ System Architecture
The system workflow is depicted in the block diagram below:

![System Architecture](assets/block_diagram.png)

## 🔧 Technologies Used
- **Python** 🐍
- **TensorFlow / PyTorch** 🔥
- **FAISS (Facebook AI Similarity Search)** 📌
- **LLaMA2 (CTransformers)** 🦙
- **ConversationalRetrievalChain** 🔄
- **OpenCV for Image Processing** 🖼️
- **Streamlit / Flask (for Deployment)** 🌍

## 📂 Project Structure
📦 Handwriting-Recognition-Chatbot ├── 📂 assets # Images, block diagram, and other visuals ├── 📂 data # Sample dataset for handwriting recognition ├── 📂 models # Pretrained models for OCR and chatbot ├── 📂 scripts # Code for training and inference │ ├── preprocess.py # Preprocessing pipeline (grayscale, filtering, etc.) │ ├── feature_extraction.py # Feature extraction using CNN & BiLSTM │ ├── vector_store.py # FAISS-based embedding storage │ ├── chatbot.py # Chatbot logic using LLaMA2 │ ├── app.py # Web app using Streamlit/Flask ├── README.md # Project documentation

## 📦 Installation
Clone this repository and install the required dependencies:

```sh
git clone https://github.com/your-username/Handwriting-Recognition-Chatbot.git
cd Handwriting-Recognition-Chatbot
pip install -r requirements.txt

🛠️ Usage
1️⃣ Run the Handwriting Recognition Model
python scripts/feature_extraction.py --input data/sample.png
2️⃣ Start the Chatbot
python scripts/chatbot.py
3️⃣ Launch the Web Interface
streamlit run scripts/app.py
or

sh
Copy
Edit
flask run
