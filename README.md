# SPO++ — Self-Supervised Prompt Optimization

Reproduction of [Xiang et al. (2025)](https://arxiv.org/abs/2502.06855) + three extensions: Ensemble Evaluator, Curriculum Sampling, and Meta-Prompt Memory.

## Setup


pip install openai


Add your OpenAI key:


export OPENAI_API_KEY=sk-...


## Run


jupyter notebook SPO_vs_SPOpp_BBH_Navigate.ipynb


Set flags at the top of the notebook:


N_ITERATIONS = 10          # or 20
TEST_SUBSET_SIZE = 60
BASELINE_CONFIG = SPOConfig(ensemble_size=1, curriculum=False, memory=False)
SPOPP_CONFIG    = SPOConfig(ensemble_size=3, curriculum=True,  memory=True)

