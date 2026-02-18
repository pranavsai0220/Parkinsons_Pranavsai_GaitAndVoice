# Parkinsons_Pranavsai_GaitAndVoice


Parkinson’s Disease AI Research Suite: Multimodal Screening
A Hybrid LLM-ML Framework for Bio-Acoustic and Kinematic Biomarker Extraction
Author: Pranavsai Dodla, TMSA Class of 2029

Status: Research & Validation Phase

Research Targets: Sensitivity Baseline 93%–96% | Accuracy 90%+

🧬 Project Philosophy
Traditional Parkinson’s Disease (PD) screening requires expensive gait labs or specialized clinical acoustics. This suite investigates a Hybrid AI Architecture: using Google Gemini 3 (Multimodal LLM) as a zero-shot feature extractor and grounding those outputs in Classical Machine Learning (KNN) trained on gold-standard clinical datasets.

🛠 Project Components
🎙 1. VoiceBiomarkerAI
Technical Stack: React 19, TypeScript, Gemini-3-Pro-Preview, KNN Classifier.

Mechanism: Uses a two-stage analysis pipeline to identify vocal fold instability.

Stage 1: Gemini acts as a bio-acoustic analyst, extracting Jitter (%), Shimmer (%), and Pitch Variability via strict JSON schema enforcement.

Stage 2: A client-side KNN model compares these features against the UCI Parkinson’s Dataset to provide a data-driven risk classification.

Result: ~94% Sensitivity; optimized to ensure at-risk individuals are encouraged to seek professional neurological consultation.

Live App: VoiceBiomarkerAI

🚶 2. GaitBiomarkerAI
Technical Stack: React 19, Gemini-3-Flash-Preview, Recharts, Google GenAI SDK.

Mechanism: Re-engineers the Gemini API into a specialized biomechanical tool for video-based analysis.

Innovation: Instruction-tuned analysis identifies sub-threshold biomarkers: Hypokinesia, Bradykinesia, and Postural Instability.

Prompt Engineering: Achieved a 60% cumulative improvement in clinical relevance by tethering AI logic to the PhysioNet Gait Database benchmarks.

Performance: Achieves a diagnostic baseline of 93%–96% sensitivity through temporal reasoning of gait cycles.

Live App: GaitBiomarkerAI

🧪 Scientific Validation (Google Colab)
The research transition in 10th grade focuses on rigorous statistical verification using Python (Pandas, Scikit-Learn):

LOOCV Validation: Utilizing Leave-One-Out Cross-Validation to ensure model generalizability.

Metric Analysis: Analysis of Confusion Matrices to balance the trade-off between False Positives (21%) and high Sensitivity (94%).

Clinical Grounding: All AI observations are cross-verified against established clinical literature (Goldberger et al., 2000).

⚠️ Disclaimer
GaitBiomarkerAI and VoiceBiomarkerAI are functional MVPs for educational and screening purposes only. They are not intended to provide medical diagnoses. Users must consult with a board-certified neurologist for clinical evaluation.

📜 Citations & Acknowledgments
UCI Dataset: Little, M. (2007). Parkinsons [Dataset]. UCI Machine Learning Repository.

PhysioNet: Goldberger, A., et al. (2000). Circulation. RRID:SCR_007345.

Implementation: All technical conceptualization and code implementation are the sole work of Pranavsai Dodla.
