# Nicholas (Nico) Hernandez

**MS CS @ Georgia Tech (Fall 2026) · BS CS @ Boston College (2026) · GPA 3.89**  
Incoming MSCS student at Georgia Tech. Research background in NLP — low-resource machine translation and speech recognition for endangered Formosan indigenous languages. Building toward a career in perception/robotics ML.

📍 Boston, MA → Atlanta, GA  
📄 [Resume](#) · 🔗 [LinkedIn](#) · 📬 [Email](#)

---

## Research

**Senior Thesis — Machine Translation for Formosan Languages** · Boston College · 2025–2026  
Advisor: Dr. Emily Prud'hommeaux  
Extending prior ASR transfer learning work to machine translation using parallel corpora across the Formosan language group. Fine-tuning Meta's NLLB-200 with custom language ID tokens, supplementary-language augmentation, and FLORES cousin-language transfer experiments. Running large-scale multilingual fine-tuning on HPC cluster (Andromeda 2 / Slurm). Paper under review at ACL Rolling Review.  
`NLLB-200` `HuggingFace` `PyTorch` `Slurm` `HPC`

**REU — ASR for Endangered Formosan Languages** · Boston College / NSF Formosan Bank Project · Summer 2025  
Advisor: Dr. Emily Prud'hommeaux  
Trained baseline Wav2Vec2 XLSR-53 models on 10-hour datasets for Austronesian languages (Amis, Paiwan, and others). Selected source-target language pairs using similarity metrics: Acoustic Token Distribution Similarity (ATDS), token overlap, subword overlap, and Levenshtein distance. Extended experiments to typologically distant languages (English, Hungarian, Swahili) — unrelated languages with high ATDS scores improved WER by up to 68%. Found that within-family transfer benefited low-resource targets when source language had high n-gram perplexity. Results inform a strategic framework for source language selection in ASR tools for language revitalization.  
`Wav2Vec2` `XLSR-53` `HuggingFace` `PyTorch` `Austronesian NLP`

**REU — Multilingual Toxicity Detection** · University of Houston · Summer 2024  
Advisor: Dr. Rakesh Verma (NSF-funded)  
Fine-tuned XLM-RoBERTa for toxicity detection across six Romance languages (Spanish, French, Italian, Portuguese, Catalan, Romanian). Tested whether transfer learning was more effective between closely related languages using language subfamily structure. Confirmed transfer learning potential for cross-lingual toxicity detection while surfacing new questions about linguistic similarity and model behavior.  
`XLM-RoBERTa` `PyTorch` `HuggingFace` `Carya HPC`

---

## Projects

**MicroRTS Hybrid RL Agent** · Machine Learning Projects Course  
Built a hybrid agent for the MicroRTS environment combining tree-search planning with a PPO-based control model. Achieved a TrueSkill of 33.7, outperforming MicroRTS baselines including CoacAI (33.4). Early training of the integrated tree-search model showed faster convergence gains; preliminary results suggest promise for combining planning with RL in RTS games.  
`PPO` `Tree Search` `PyTorch` `MicroRTS`

**Music Popularity Predictor** · NLP Course  
Binary classification of Billboard Hot 100 hits from song lyrics. Compared BoW, Word2Vec, stylometric features, and fine-tuned BERT. Decade-stratified dataset of ~90K songs scraped via LyricsGenius + Spotify Tracks Dataset.  
`BERT` `Word2Vec` `scikit-learn` `Python`

**Robot Soccer** · Intro Robotics Course  
[Add a 1–2 sentence description here]  
`ROS` `Python`

**ArcGIS — Datacenter Effects on Utility Bills in Virginia**  
Spatial analysis project mapping the relationship between datacenter density and residential utility bill costs across Virginia. Built using ArcGIS with publicly available utility and infrastructure datasets.  
`ArcGIS` `GIS` `Spatial Analysis`

**Domino Pip Solver** · w/ Kai Gowers · Logic & Computation Course  
Automated solver for the NYT Pips puzzle using Z3. Encoded the puzzle as a constraint satisfaction problem: Boolean placement variables per domino/edge/orientation, integer cell value variables (0–6), and regional constraints (sum_lt, sum_eq, all_eq, all_diff). Guarantees every cell is filled by exactly one domino side while satisfying all regional pip conditions.  
`Z3` `Python` `CSP`

---

## Education

**Georgia Tech** — MS Computer Science *(starting Fall 2026)*  
Specialization: Robotics and Perception

**Boston College** — BS Computer Science, Minor in Mathematics *(May 2026)*  
GPA: 3.89 · Alpha Sigma Nu Honor Society · Phi Beta Kappa · Dean's List 
Relevant coursework: NLP, Machine Learning, Computer Vision, Robotics, Algorithms, Linear Algebra, Probability & Statistics

---

## Skills

**Languages:** Python, C++, JavaScript, Java  
**ML/NLP:** PyTorch, HuggingFace Transformers, scikit-learn, NLLB-200, XLM-RoBERTa, Wav2Vec2, BERT  
**Robotics:** ROS2 (Jazzy), Gazebo, Nav2, OpenCV  
**Tools:** Git, Slurm, Linux, HPC clusters, ArcGIS  
**Libraries:** NumPy, Pandas, Matplotlib, Tone.js, MediaPipe, Z3

---

## Currently

- Finishing senior thesis (MT for Formosan languages, ACL Rolling Review)

---

*Last updated April 2026*
