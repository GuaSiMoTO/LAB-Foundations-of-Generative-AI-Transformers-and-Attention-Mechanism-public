![](https://user-images.githubusercontent.com/970858/63474771-d6734700-c469-11e9-83bb-9429da563909.png)
# LAB-Foundations-of-Generative-AI-Transformers-and-Attention-Mechanism

## Introduction
In this lab, students will compare Transformer models on two key tasks:
1. **Text Summarization**: Using **BART** to evaluate the quality of generated summaries.
2. **Sentiment Analysis**: Comparing a pretrained model (e.g., **DistilBERT** or **RoBERTa**) for sentiment classification.
3. **Text Translation**: Utilizing the **Helsinki-NLP** model to translate text from English to Spanish and analyze the impact of different parameters on translation quality.

The objective is to observe how different Transformer models process and produce results for the same tasks, evaluating differences in precision, consistency, and quality, and exploring their applicability to real-world scenarios.

## Initial Setup

### Requirements
Start by forking the provided GitHub repository to your account and then clone it locally. This will be your workspace for completing the lab exercises.

- [Learn how to fork this repo](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project)
- Clone this repo into your code/labs folder.

```bash
git clone https://github.com/codeskills-ai/LAB-Foundations-of-Generative-AI-Transormers-and-Attention-Mechanism.git
cd LAB-Foundations-of-Generative-AI-Transormers-and-Attention-Mechanism
```

### Setup Instructions

Create a virtual environment and install the required packages:

```bash
pip install -r requirements.txt
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Once your environment is ready, you're all set to dive into the exercises.

## Iteration 1: Loading the Models
1. **BART**:
   - Import the model and tokenizer from Hugging Face.
   - Load the pretrained model `facebook/bart-large-cnn`.
2. **Sentiment Analysis Model**:
   - Use a pretrained model like **DistilBERT** or **RoBERTa** from Hugging Face.
   - Load the model and tokenizer.
3. **Translation Model**:
   - Import and initialize the pre-trained **Helsinki-NLP/opus-mt-en-es** model.

---

## Iteration 2: Text Summarization with BART
1. Choose a text file (`article.txt`) containing substantial content for summarization.
2. Use **BART** to generate a summary:
   - Define a function that takes the input text and returns a summary using **BART**.
   - Save the summary to `summary_bart.txt`.

---

## Iteration 3: Translating Text with Helsinki-NLP
1. **Generate a Translation**:
   - Use the tokenized input to translate the text from English to Spanish using the Helsinki-NLP model.
   - Experiment with parameters like `max_length` and `num_beams` to explore how they affect the translation output.

2. **Save Translations**:
   - Save the translations to a file `translations_helsinki.txt`.

---

## Iteration 4: Sentiment Analysis with DistilBERT or RoBERTa
1. Prepare a set of short texts with sentiment labels (positive, negative, neutral).
2. Use the pretrained model (e.g., **DistilBERT**) for sentiment classification:
   - Define a function to process each text and return a sentiment label.
   - Save the predictions to `sentiments_model.txt`.

---

## Iteration 5: Final Evaluation
1. Reflect on the tasks performed and answer key questions:
   - How effective was **BART** for text summarization? What were the strengths and limitations?
   - How effective was the sentiment analysis model? What differences did you observe?
   - How well did the Helsinki-NLP model perform for text translation? Were there any noticeable patterns or limitations?

## Bonus: Fine-Tuning for Custom Summarization and Translation

In this bonus exercise, you will explore **BART** and **Helsinki-NLP**’s abilities to generate customized outputs based on specific contexts.

### Instructions:

#### 1. Customizing Summarization and Translation:
- Experiment with different aspects of the input file for summarization and translation.
- For example:
  - *"Summarize the text and then translate it to Spanish focusing on key points related to AI."*

#### 2. Evaluating Coherence and Accuracy:
- Generate summaries and translations for different inputs.
- Evaluate the coherence, consistency, and accuracy of the results.

#### 3. Exploring Translation Parameters:
- Modify translation parameters such as `max_length`, `num_beams`, and `temperature` to observe their impact.
- Document the parameter settings and corresponding results for analysis.

## Bonus: Fine-Tuning Ollama for Custom Summarization

In this bonus exercise, you will explore the **Ollama** model’s ability to generate customized summaries based on specific contexts. Your task is to modify prompts and experiment with different approaches to create audience-specific summaries and varying lengths of summaries using the article provided.

## Instructions:

### 1. Customizing the Prompt:
- Modify the prompt to focus on different aspects of the ```article.txt```.
- Examples of custom prompts include:
  - *"Summarize the text focusing on AI's impact in medical imaging"*
  - *"Summarize the text emphasizing AI's role in streamlining administrative tasks in healthcare"*

- Compare the results and reflect on how the variations in prompts affect the output of the summary.

### 2. Evaluating Coherence:
- Generate multiple summaries of the same article using slight changes in the prompt (e.g., focusing on different sections or aspects).
- Evaluate the coherence and consistency of each summary. Which prompts led to the most accurate and clear results? Why?

### 3. Audience-Specific Summaries:
- Create summaries for different audiences. For example:
  - *"Generate a summary for healthcare professionals"*
  - *"Summarize the article for patients interested in AI applications in healthcare"*

- Analyze how the content changes based on the audience. Does the model successfully adapt the information to match the audience's needs?

### 4. Summary Length:
- Experiment with summary length by varying the prompts:
  - *"Provide a brief summary of the article"*
  - *"Provide a detailed summary of the article"*

- Compare the results and evaluate how the level of detail and accuracy shifts with different lengths.



## Submission

Once you have completed the lab, push your Jupyter notebook to your forked GitHub repository and create a pull request.

```bash
$ git add .
$ git commit -m "completed lab"
$ git push origin main
```

![happy_coding](https://user-images.githubusercontent.com/970858/63899010-c23fc480-c9ea-11e9-84a2-542907e42362.png)
