# DuplexGen: Adaptive Synthesis of Human-AI Turn-Taking Dialogues

[Takyoung Kim](https://youngerous.github.io/)<sup>1\*</sup>,
[Kang-wook Kim](https://kwkim.me/)<sup>2,4\*</sup>,
[Sang Hoon Woo](https://tonywoo.me/)<sup>2,5</sup>,
[Julia Hirschberg](https://www.cs.columbia.edu/~julia/)<sup>3</sup>,
[Gunhee Kim](https://vision.snu.ac.kr/gunhee/)<sup>2</sup>,
[Dilek Hakkani-Tür](https://siebelschool.illinois.edu/about/people/faculty/dilek)<sup>1</sup>

<sup>1</sup>University of Illinois Urbana-Champaign &nbsp;
<sup>2</sup>Seoul National University &nbsp;
<sup>3</sup>Columbia University &nbsp;
<sup>4</sup>University of California, Berkeley &nbsp;
<sup>5</sup>Georgia Institute of Technology

<sup>\*</sup>Equal contribution

[![arXiv](https://img.shields.io/badge/arXiv-2607.26178-b31b1b.svg)](https://arxiv.org/abs/2607.26178)

📄 [**Paper**](https://arxiv.org/abs/2607.26178) &nbsp;·&nbsp;
🌐 [**Samples & Demo**](https://duplexgen.github.io/) &nbsp;·&nbsp;
💻 [**Code**](https://github.com/duplexgen/duplexgen-code) &nbsp;·&nbsp;
🤗 [**Corpus**](https://huggingface.co/datasets/DuplexGen/duplexgen-corpus) &nbsp;·&nbsp;
🤗 [**Spoken**](https://huggingface.co/datasets/DuplexGen/duplexgen-spoken)

---

> **Code release coming soon. The full code will be released by the end of the first week of August.**

This repository will host the recipe for fine-tuning a full-duplex model (PersonaPlex)
on DuplexGen-generated data.

---

## Abstract

Turn-taking is a central component of full-duplex interaction. Which turn-taking
behaviors are appropriate varies with the scenario, yet current models apply a single
norm regardless of context. This limitation originates in their training data:
human-human speech corpora capture natural timing phenomena but provide little
role grounding or scenario-specific norms, while heuristic or prompted synthesis
methods inject turn-taking behaviors without basing them on human preferences.
We introduce **DuplexGen**, a framework for generating dialogues with
scenario-adaptive turn-taking by calibrating LLM predictions against a small set of
slot-level human preference annotations.
In six cooperative and competitive tasks, human turn-taking preferences differ
systematically, and DuplexGen aligns substantially more closely with those
preferences than uncalibrated prompting or training solely on generic
human-human data; a full-duplex model trained on DuplexGen-generated data
exhibits distinctive, human-preferred turn-taking behaviors. These results show that
human calibration, not corpus scale or prompt design alone, is what allows
turn-taking synthesis to be scenario-specific.

## Citation

```bibtex
@misc{kim2026duplexgenadaptivesynthesishumanai,
      title={DuplexGen: Adaptive Synthesis of Human-AI Turn-Taking Dialogues},
      author={Takyoung Kim and Kang-wook Kim and Sang Hoon Woo and Julia Hirschberg and Gunhee Kim and Dilek Hakkani-Tür},
      year={2026},
      eprint={2607.26178},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2607.26178},
}
```
