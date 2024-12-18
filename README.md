Abstract: Large language models (LLMs) have been
shown to carry the political biases of their training data. We investigate how political bias influences an LLM’s performance on the text classification task, focusing on political ideology
detection (PID). Using a transformed version of
the Ideological Books Corpus (IBC), we evaluate models in two phases: zero-shot evaluation and fine-tuned evaluation. In the zero-shot
phase, we employ HuggingFace pipelines and
the OpenAI API to test various zero-shot models on PID with both three-label [Liberal, Conservative, Neutral] and two-label [Liberal, Conservative] setups. We observe a tendency for
the models to overpredict “Neutral” foremostly,
with the label aligning with their inferred political bias (bias label) second. In the two-label
setup, the bias label is overpredicted. In the second phase, we fine-tune BERT-base for the PID
task. The fine-tuned model avoids the Neutral
overprediction observed in zero-shot evaluation. Our findings suggest that political biases
in LLMs influence performance on the PID task
with respect to the bias label both in zero-shot
and brief fine-tuning scenarios, with the possibility of being mitigated through additional
thorough fine-tuning and larger models. 

This repository holds the write up. Code is in my co-researchers repository: https://github.com/luhaza/pid-of-nlp-models
