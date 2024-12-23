AI/ML

Recall
F1 score

Models:
	Xgboost


Overfit
Underfit


Do not store secrets in notebook
Untrusted models
Untrusted dependencies
Model management (tag the model with data sensitivity treat it as an asset) 

Scoping -> ML Problem -> Data aquisition and prep ->Model training -> Model evaluation -> Model acceptance-> model release to prod -> Privision inference -> Monitor (Model drift, performance eval, feedback)

AI bill of materials
sign model


Generative AI
Direct prompt injection
Indirect prompt injection - "read the website and summarize"

Prompt injection
system prompt and user prompt


Attack:
Prompt injection (all these are prompt injections)
Context Overflow (context length attacks)
Inferencing Attack
Steal model
model evasion
Jailbreak(realted to prompt injection)
DAN framework
gandalf.lakera.ai
gpt prompt attacker




Defense:
Prompt management
taint analysis
layered 
few shot prompts
Temperature to 0 to make it more deterministic
finetuning



make the llm app more focused on task instead of general 