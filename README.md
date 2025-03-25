This paper investigated whether CoT-decoding as described by Wang, X., & Zhou, D. (2024) can
successfully be combined with smaller language models, for which the experiments described
in Section 3.1 of the original paper have been repeated with Qwen2.5 (0.5B) in both pre-trained
and instruction tuned versions, as well as with TinyLLama (1.1B).
The results suggest that in most cases CoT-decoding as of now cannot be usefully com-
8bined with smaller language models, and that those models lack some of the intrinsic reasoning
capabilities that larger models have shown. Their ability seems to depend much more on the
training process than with larger models. The Qwen2.5 models with 0.5 billion parameters have
demonstrated the general knowledge on how to reason, but still had shortcomings that might
not be solvable without external support (e.g., fine-tuning, regular tools).
CoT-decoding comes with high computational costs, making it impractical for applications
requiring fast inference. While it might improve accuracy in certain cases, the trade-off between time and performance must be carefully considered. This is especially important as this
decoding method mitigates two of the main advantages of smaller language models, i.e. speed
and less computational cost, without the guarantee of improved performance.

This is the main references for current research:
Wang, X., & Zhou, D. (2024). Chain-of-thought reasoning without prompting. arXiv preprint arXiv:2402.10200.
