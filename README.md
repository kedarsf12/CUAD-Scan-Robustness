# Document-AI Robustness to Scanned-Document Degradation

Code and evaluation harness for the preprint *"How Robust Is Document AI to Scanned-Document Degradation? An Empirical Study of Extraction Robustness on Contract Clause Recognition"* (Ferozabadkar & Deshpande, 2026). It degrades CUAD contracts to graded scan quality, runs OCR + LLM clause extraction, and scores accuracy and failure modes.

Download CUAD separately (CC BY 4.0) into the repo root, then run `python compare_providers.py --source cuad --split test --ollama-models llama3.1,mistral,qwen2.5 --max-pages 8` followed by `python plot_results.py`. See `requirements.txt` for dependencies (Python, Tesseract, Ollama).
