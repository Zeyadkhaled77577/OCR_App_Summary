# Document Analyzer with Summarization & Question Generation

This project is designed to process a variety of file types (PDF, image, PowerPoint, audio) to extract text, summarize it, and generate questions based on the content. Using advanced models like **Llama 3.2**, this tool leverages the power of natural language processing (NLP) to create accurate and human-like summaries and questions, catering to both English and Arabic texts.

## Key Features

- **Multi-format Support**: Upload files in formats like PDF, Word, Excel, PowerPoint, images, and audio files (MP3, WAV) to extract text.
- **Optical Character Recognition (OCR)**: Extract text from images using Tesseract with language support for Arabic and English.
- **Speech Recognition**: Convert speech from audio files into text using Google Web Speech API.
- **Summarization**: Generate concise summaries in both English and Arabic, using Llama 3.2.
- **Question Generation**: Automatically generate comprehension questions from the text in either English or Arabic.
- **Interactive Interface**: Easy-to-use interface built with Gradio.

## Technologies Used

- **Llama 3.2**: A powerful language model by Meta AI, fine-tuned for text generation tasks. Llama 3.2 is a state-of-the-art model that excels in handling complex text generation tasks such as summarization and question generation.
- **Hugging Face Transformers**: For loading and using Llama 3.2 in text-generation tasks.
- **Tesseract OCR**: For extracting text from images, supporting multiple languages.
- **PyMuPDF (Fitz)**: For text and image extraction from PDF files.
- **SpeechRecognition**: For converting audio files into text.
- **Gradio**: A web-based interface for users to interact with the model.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/EngAhmed19/OCR_App_Summary
   cd OCR_App_Summary
   ```
2. Install the required dependencies:
   ```bash
   !sudo pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   python ocr_summaryapp.py
   ```
4. Access the interface through the provided URL in the terminal. Upload your file, select the task (Summarization/Question Generation), and choose the language options to get started.


## Llama 3.2 Overview
Llama 3.2 is a highly sophisticated transformer-based language model built on the foundations of the original LLaMA architecture by Meta AI. The key features of Llama 3.2 include:
-**Architecture**:Like other transformer models, Llama 3.2 uses attention mechanisms to process and generate text. Its multi-head attention layers allow it to weigh the importance of different words in a sentence, creating highly contextualized and relevant text outputs.
-**Model Size**: Llama 3.2 is available in various sizes (e.g., 1B, 7B, 13B parameters) depending on the task requirements. This project uses the 1B parameter version, balancing performance and efficiency.


## Model Architecture
image ref: [Llama3.2 source](https://x.com/rasbt/status/1842548690256384278/photo/1)

![Llama3.2](./images/llama3.2.jfif)

The architecture of Llama 3.2 consists of stacked transformer layers, where each layer contains a self-attention mechanism followed by feed-forward networks. These components allow the model to capture long-range dependencies between words and generate coherent, human-like text.

### Llama 3.2 1B:
- **Vocabulary Size**: 128,256  
- **Hidden Layer Dimension**: 8,192  
- **Attention Heads**: 32  
- **Activation Function**: SiLU  
- **Normalization**: Final RMSNorm  
- **Embedding Dimension**: 2,048  
- **Context Length**: 8,192 tokens  
- **Features**: Masked grouped-query attention, RoPE rescaling

