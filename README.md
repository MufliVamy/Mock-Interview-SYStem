The AI Mock Interview System is a project that aims to help individuals prepare for job interviews by providing a simulated interview experience. The system utilizes two natural language processing (NLP) models: a T5 model for generating interview questions and a BERT model for evaluating the user's responses.

<img width="2026" alt="tldraw (1) (1)" src="https://github.com/MufliVamy/Mock-Interview-SYStem/assets/93393847/b00fb1e2-afc6-4b3c-9686-c839a83e08f2">




**Project Overview**

The system works as follows:

1. Question Generation: The user provides a context or a job description, which is fed into the T5 model. The T5 model generates a list of relevant interview questions based on the given context.
2. User Response: From the generated list of questions, one question is presented to the user. The user then provides their response to the question.
3. Response Evaluation: The user's response is compared with the answer generated by the BERT model. The comparison is performed using two techniques:

a.Word-level Comparison: The cosine similarity between the user's response and the model's answer is calculated, providing a word-level similarity score.
b.Sentence-level Comparison: To account for semantic similarities beyond individual words, a sentence transformer function is employed to compare the user's response with the model's answer at the sentence level.


4. Rating: Based on the cosine similarity scores from both the word-level and sentence-level comparisons, the user's response is rated, providing feedback on their performance.








**Installation**

Clone the repository: git clone https://github.com/MufliVamy/Mock-Interview-SYStem.git
Install the required dependencies: pip install -r requirements.txt
Run the application: python main.py








**License**

This project is licensed under the Apache-2.0 License.







**Acknowledgments**

The T5 model used for question generation is based on the work of Google AI.
The BERT model used for response evaluation is based on the work of Google AI.
The sentence transformer function is based on the Sentence-Transformers library
