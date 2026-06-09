Deepfake Video Detector: Neural Forensic Platform
A high-performance forensic workstation designed to authenticate video media using advanced deep learning architectures. This platform performs automated biometric analysis to identify synthetic media manipulation with high-dimensional statistical verification.

Core Forensic Capabilities
Neural Engine: Utilizes a custom EfficientNetV2 core architecture to perform latent space mapping and biometric face isolation.

Explainable AI (XAI): Moves beyond "black box" detection by providing Forensic Interpretability Weights. It breaks down the classification logic based on:

Facial Edge Blending: Identifies boundary discontinuities indicative of mask-based manipulation.

Spatial Noise Artifacts: Detects GAN-generated pixel inconsistencies.

Temporal Flickering: Measures inter-frame structural jitter.

Statistical Rigor: Computes deep analytical metrics, including ROC-AUC variance, Log-Loss convergence indices, SSIM vector deviation, and Benford’s Law Delta analysis to verify media integrity.

Automated Reporting: Generates comprehensive, multi-page forensic PDF reports for every input, featuring detailed frame-by-frame ledger tables, anomaly trace graphs, and biometric thumbnail captures.

Architecture Highlights
Inference Pipeline: Executes a sequential 20-frame biometric matrix extraction.

Verdict Logic: Features a robust 3-way classification system—REAL, DEEPFAKE, or INCONCLUSIVE (for mid-threshold statistical ambiguity).

Temporal Mapping: Visualizes probability drifts across the video timeline to pinpoint exact moments of suspected manipulation.

Technical Stack
Backend: Flask (Python) with TensorFlow/Keras integration.

Forensics: OpenCV for biometric region isolation and temporal structure analysis.

Frontend: TailwindCSS, Chart.js for real-time telemetry, and HTML2PDF for automated forensic document generation.

Installation
Clone the repository: git clone [https://github.com/AbdulRehmanShariff/Deepfake-Video-Detector.git](https://github.com/AbdulRehmanShariff/Deepfake-Video-Detector.git)

Install requirements: pip install -r requirements.txt

Run the backend: python app.py

Open index.html in your web browser.

Forensic Results
All generated PDF reports and analytical data are stored in the results/ directory.

Built as an enterprise-grade forensic tool for media authenticity verification.
