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


## Generative AI
**Prompt injection**
- Direct prompt injection
- Indirect prompt injection - "read the website and summarize"


system prompt and user prompt


### Attack:
```python
Prompt injection (all thebelow are prompt injections)
Context Overflow (context length attacks)
Inferencing Attack
Steal model
model evasion
Jailbreak(realted to prompt injection)
DAN framework
gandalf.lakera.ai
gpt prompt attacker
weak model provenance
```



### Defense:
```python
Prompt management
taint analysis
layered 
few shot prompts
Temperature to 0 to make it more deterministic
finetuning
Differential privacy
federated learning
homomorphic encryption
```



make the llm app more focused on task instead of general 

## OWASP Top10 ffor LLM

- LLM01:2025 Prompt Injection
- LLM02:2025 Sensitive Information Disclosure
- LLM03:2025 Supply Chain
- LLM04: Data and Model Poisoning
- LLM05:2025 Improper Output Handling
- LLM06:2025 Excessive Agency
- LLM07:2025 System Prompt Leakage
- LLM08:2025 Vector and Embedding Weaknesses
- LLM09:2025 Misinformation
- LLM10:2025 Unbounded Consumption

Bedrock Security
```
Prompt management

Bedrock Guardrails
VPC endpoints
Encryption
observability, Moinitoring and alerting

```