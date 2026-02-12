Task 4: General Health Query Chatbot - DevelopersHub Corporation

Task Objective                                                                                                                                                                                                                                                                                                      
The main objective of this task is to create an interactive chatbot that safely answers general health-related queries using a Large Language Model (LLM). Understanding how to guide AI responses safely and clearly is critical in AI/ML applications involving sensitive topics.

Specifically, this task focuses on:                                                                                                                                                                                  
1.Designing prompts to generate friendly and helpful responses.                                                                                                                                                      
2.Building a Python interface to interact with the LLM.                                                                                                                                                              
3.Adding safety filters to prevent harmful or dangerous advice.                                                                                                                                                      
4.Handling common health-related questions such as medication safety, minor symptoms, and wellness tips.                                                                                                             

Dataset / Model Used                                                                                                                                                                                                
Model Name: google/flan-t5-large (instruction-tuned)                                                                                                                                                                 
Source: Hugging Face Transformers Library                                                                                                                                                                            
Frameworks: transformers, torch                                                                                                                                                                                      
Device: CPU or GPU                                                                                                                                                                                                   
No external dataset is required; the LLM generates responses dynamically.                                                                                                                                               

Tools and Methods Used                                                                                                                                                                                               
Python Libraries: transformers, torch                                                                                                                                                                                
Prompt Engineering: To ensure responses are friendly, informative, and safe.                                                                                                                                         
Safety Filters: Blocks queries related to suicide, overdose, self-harm, or other dangerous topics.                                                                                                                   
Interactive Loop: Allows real-time user queries and AI responses.                                                                                                                                                    

Steps Performed                                                                                                                                                                                                      
Import Libraries:
Imported necessary Python libraries including transformers and torch to handle the LLM model and tokenization.

Load Model:
Loaded the pre-trained instruction-tuned model google/flan-t5-large from Hugging Face. Configured the model to run on GPU if available, otherwise CPU.

Setup Safety Filter:
Defined a safety filter to block queries related to dangerous topics, including self-harm, overdose, poisoning, or other harmful actions.

Prompt Design:
Created a structured prompt instructing the LLM to act as a friendly medical assistant, ensuring responses are safe, clear, and helpful.

Generate Responses:
Configured the model to generate answers for user queries dynamically, using the tokenizer to process inputs and decode outputs.

Interactive Chat Interface:
Implemented a simple interactive loop allowing users to enter health-related queries, receive responses from the LLM, and exit the chat safely.

Testing & Validation:
Tested the chatbot with example queries such as:
"What causes a sore throat?"
"Is paracetamol safe for children?"
"How can I improve sleep?"

Validated that the chatbot provides helpful, safe answers and that the safety filter effectively blocks unsafe queries.

Key Results and Findings                                                                                                                                                                                            
1.The chatbot provides friendly, safe responses to general health questions.                                                                                                                                         
2.Safety filters successfully block queries related to dangerous or harmful actions.

Example interactions:                                                                                                                                                                                                
Q: "What causes a sore throat?" → A: "A cold"                                                                                                                                                                        
Q: "Is paracetamol safe for children?" → A: "Yes"                                                                                                                                                                    
Q: "How can I improve sleep?" → A: "Drink a glass of water before bed"                                                                                                                                               
This system can serve as a general guidance assistant but cannot replace professional medical advice.

