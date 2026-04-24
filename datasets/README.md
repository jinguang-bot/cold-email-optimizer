# Datasets for Cold Email Optimizer

This directory contains datasets downloaded for the Cold Email Optimizer project. The datasets focus on negotiation, persuasion, and dialogue systems research.

## Dataset Overview

| Dataset | Status | Size | Type | Source |
|---------|--------|------|------|--------|
| CaSiNo | ✅ Success | 9.4M | Negotiation Dialogues | GitHub |
| PersuasionForGood | ✅ Success | 34M | Persuasion Dialogues | GitHub |
| NegotiationToM | ⚠️ Partial | 6.4M | Negotiation with Theory of Mind | GitHub |
| Awesome-LLMs-as-Judges | ✅ Success | 18M | Survey/Paper List | GitHub |

---

## 1. CaSiNo Dataset

**Status:** ✅ Successfully cloned

**Repository:** https://github.com/kushalchawla/CaSiNo

**Local Path:** `/home/ubuntu/.openclaw/workspace/projects/cold-email-optimizer/datasets/CaSiNo`

**Paper:** "CaSiNo: A Corpus of Campsite Negotiation Dialogues for Automatic Negotiation Systems" (NAACL 2021)

### Content Summary

The CaSiNo dataset contains **1,030 negotiation dialogues** between two participants taking the role of campsite neighbors. They negotiate for **Food**, **Water**, and **Firewood** packages based on their individual preferences.

**Dataset Structure:**
- `data/casino.json` - Complete dataset (1,030 dialogues)
- `data/split/` - Train/valid/test splits
- `strategy_prediction/` - PyTorch code for strategy prediction

**Key Features per Dialogue:**
- **Participant Info:** Demographics (age, gender, ethnicity, education), personality attributes (SVO and Big-5), preference order, arguments
- **Negotiation Dialogue:** Alternating conversation (11.6 utterances on average), includes four emoticons (Joy, Sadness, Anger, Surprise)
- **Negotiation Outcomes:** Points scored, satisfaction (1-5 scale), opponent likeness (1-5 scale)
- **Strategy Annotations:** Utterance-level annotations for 396 dialogues (4,615 utterances)

### Project Relevance

- **Negotiation Patterns:** Understanding how people negotiate and persuade in resource allocation scenarios
- **Dialogue Strategies:** Learning effective negotiation tactics that can inform cold email persuasion
- **Personalization:** Participant demographics and personality attributes provide insights into personalized communication

---

## 2. PersuasionForGood Dataset

**Status:** ✅ Successfully cloned

**Repository:** https://github.com/ohyj1002/persuasionforgood

**Local Path:** `/home/ubuntu/.openclaw/workspace/projects/cold-email-optimizer/datasets/persuasionforgood`

**Paper:** "Persuasion for Good: Towards a Personalized Persuasive Dialogue System for Social Good" (ACL 2019)

### Content Summary

The PersuasionForGood dataset contains **1,017 persuasion dialogues** (300 annotated, 717 additional) focused on persuading participants to donate to charity.

**Dataset Structure:**
- `data/AnnotatedData/` - 300 annotated dialogues with participant information
- `data/FullData/` - All 1,017 dialogues with participant information
- `classifier/` - Codebase for classification models
- `data/persuader_scheme.docx` - Annotation scheme for persuaders
- `data/persuadee_scheme.docx` - Annotation scheme for persuadees

**Key Features:**
- **Dialogue Structure:** Multi-turn persuasion conversations
- **Annotations:** Salient persuasion strategies for both persuader and persuadee
- **Outcomes:** Intended vs. actual donation amounts
- **Participant Info:** User demographics and roles
- **Sentiment:** neg, neu, pos values for each utterance

### Project Relevance

- **Persuasion Strategies:** Direct relevance to cold email persuasion tactics
- **Personalized Persuasion:** Understanding how to tailor messages based on participant characteristics
- **Dialogue Effectiveness:** Measuring persuasion success through actual donations
- **Multi-turn Conversation:** Learning how persuasion unfolds over multiple exchanges

---

## 3. NegotiationToM Dataset

**Status:** ⚠️ Partial Success (Password Protected)

**Repository:** https://github.com/HKUST-KnowComp/NegotiationToM

**Local Path:** `/home/ubuntu/.openclaw/workspace/projects/cold-email-optimizer/datasets/NegotiationToM`

**Paper:** "NegotiationToM: A Benchmark for Stress-testing Machine Theory of Mind on Negotiation Surrounding" (EMNLP 2024)

### Content Summary

This dataset provides a benchmark for testing machine Theory of Mind (ToM) capabilities in negotiation contexts.

**Current State:**
- `NegotiationToM.zip` - Password-protected dataset file
- `README.md` - Documentation available
- `Example_Figure.jpg` - Visual example of the task

**Access Issue:**
The dataset file is password-protected with password: **"NegotiationToM"** (as stated in the README). The zip file needs to be manually extracted using this password.

**Manual Download Instructions:**
```bash
cd /home/ubuntu/.openclaw/workspace/projects/cold-email-optimizer/datasets/NegotiationToM
unzip NegotiationToM.zip
# Enter password: NegotiationToM
```

### Project Relevance

- **Theory of Mind:** Understanding how to model and predict the beliefs, intentions, and emotions of negotiation partners
- **Strategic Reasoning:** Learning to anticipate and respond to the mental states of counterparts
- **Contextual Understanding:** Leveraging surrounding information (context) in negotiation scenarios

---

## 4. Awesome-LLMs-as-Judges

**Status:** ✅ Successfully cloned

**Repository:** https://github.com/CSHaitao/Awesome-LLMs-as-Judges

**Local Path:** `/home/ubuntu/.openclaw/workspace/projects/cold-email-optimizer/datasets/Awesome-LLMs-as-Judges`

**Paper:** "LLMs-as-Judges: A Comprehensive Survey on LLM-based Evaluation Methods" (arXiv 2024)

### Content Summary

This is a curated list of research papers and resources on using Large Language Models (LLMs) as evaluators (judges). It's not a dataset in the traditional sense, but rather a comprehensive survey and bibliography.

**Repository Structure:**
- `README.md` - Main documentation with categorized paper list
- `NeurIPS.md` - Papers from NeurIPS 2024
- `img/` - Visualizations and overview diagrams

**Key Categories:**
1. **Functionality**
   - Performance Evaluation
   - Model Enhancement
   - Data Collection

2. **Methodology**
   - Single-LLM Systems
   - Multi-LLM Systems
   - Human-AI Collaboration Systems

3. **Applications**
   - General, Multimodal, Medical, Legal, Financial, Education, Information Retrieval, etc.

4. **Meta-Evaluation**
   - Benchmarks
   - Metrics

5. **Limitations**
   - Biases
   - Adversarial Attacks
   - Inherent Weaknesses

### Project Relevance

- **Evaluation Metrics:** Understanding how to evaluate the effectiveness of cold emails
- **LLM-as-Judge:** Using LLMs to automatically assess email quality and persuasion
- **Bias Awareness:** Recognizing potential biases in automated evaluation
- **Benchmarking:** Establishing evaluation frameworks for cold email optimization

---

## Summary

All four repositories have been successfully cloned. The datasets provide complementary perspectives on:

1. **Negotiation** (CaSiNo) - Resource allocation, dialogue strategies
2. **Persuasion** (PersuasionForGood) - Direct persuasion tactics, personalization
3. **Theory of Mind** (NegotiationToM) - Understanding mental states in negotiation
4. **Evaluation** (Awesome-LLMs-as-Judges) - Automated assessment methodologies

These datasets collectively cover key aspects relevant to optimizing cold emails:
- Understanding persuasion strategies
- Personalizing communication
- Modeling recipient psychology
- Evaluating email effectiveness

---

## Next Steps

1. **Extract NegotiationToM dataset** using password "NegotiationToM"
2. **Explore data formats** for each dataset
3. **Identify relevant features** for cold email optimization
4. **Design evaluation metrics** based on LLM-as-Judge insights
5. **Develop training pipelines** using the dialogue and negotiation datasets

---

## Citation Information

### CaSiNo
```bibtex
@inproceedings{chawla2021casino,
  title={CaSiNo: A Corpus of Campsite Negotiation Dialogues for Automatic Negotiation Systems},
  author={Chawla, Kushal and Ramirez, Jaysa and Clever, Rene and Lucas, Gale and May, Jonathan and Gratch, Jonathan},
  booktitle={Proceedings of the 2021 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies},
  pages={3167--3185},
  year={2021}
}
```

### PersuasionForGood
```bibtex
@article{wang2019persuasion,
  title={Persuasion for Good: Towards a Personalized Persuasive Dialogue System for Social Good},
  author={Wang, Xuewei and Shi, Weiyan and Kim, Richard and Oh, Yoojung and Yang, Sijia and Zhang, Jingwen and Yu, Zhou},
  journal={arXiv preprint arXiv:1906.06725},
  year={2019}
}
```

### NegotiationToM
```bibtex
@article{DBLP:journals/corr/abs-2404-13627,
  author       = {Chunkit Chan and others},
  title        = {NegotiationToM: {A} Benchmark for Stress-testing Machine Theory of Mind on Negotiation Surrounding},
  journal      = {CoRR},
  volume       = {abs/2404.13627},
  year         = {2024}
}
```

### Awesome-LLMs-as-Judges
```bibtex
@misc{li2024llmsasjudgescomprehensivesurveyllmbased,
  title={LLMs-as-Judges: A Comprehensive Survey on LLM-based Evaluation Methods},
  author={Haitao Li and Qian Dong and Junjie Chen and Huixue Su and Yujia Zhou and Qingyao Ai and Ziyi Ye and Yiqun Liu},
  year={2024},
  eprint={2412.05579},
  archivePrefix={arXiv},
  primaryClass={cs.CL},
}
```

---

*Last Updated: 2026-04-23*
