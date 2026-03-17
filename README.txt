Titel: Can Perplexity Detect AI-Generated Text?

Autor: Mike Kosthorst und Alexandra Schaef 
Datum: 08. Februar 2026
Kurs/Modul: Angewandte Künstliche Intelligenz / Hochschule Ansbach
Abgabedatum: 08. Februar 2026

Beschreibung
------------
Diese Abgabe enthält die Untersuchung, ob Perplexity ein geeignetes Maß ist, um KI-generierten Text von menschlichem Text zu unterscheiden.

Enthaltene Dateien:
- Paper.pdf                               → das eigentliche Research Paper (3-4 Seiten)
- Notebook.ipynb                          → Jupyter Notebook mit allen Experimenten, Code, Berechnungen und Visualisierungen
- requirements.txt                        → Liste der benötigten Python-Pakete
- README.txt                              → diese Datei
- assignment_results/                     → Ordner mit allen exportierten Ergebnissen
  ├── 01_results_summary_all_models.csv
  ├── 02_results_summary_table.png
  ├── 03_descriptive_stats_per_model.csv   (falls vorhanden)
  └── figures/
      ├── 04_mean_ppl_comparison_bar.png
      ├── 05_overall_ppl_boxplot.png
      ├── 06_multi_roc_comparison.png
      └── 07_burstiness_bar.png
      (ggf. weitere modell-spezifische Plots)

Ausführungshinweise
-------------------
1. Requirements installieren:
   pip install -r requirements.txt

2. Notebook starten:
   jupyter notebook Notebook.ipynb
   oder
   jupyter lab

3. Wichtige verwendete Modelle (Hugging Face):
   - gpt2
   - bigscience/bloom-560m
   - EleutherAI/gpt-neo-125m
   - distilgpt2
   - Qwen/Qwen2.5-1.5B-Instruct   (oder ähnliche Qwen-Varianten)

4. Hardware-Hinweis:
   - Die meisten Modelle laufen gut auf CPU (getestet).
   - Größere Modelle (z. B. Qwen2.5) profitieren stark von GPU (CUDA), falls verfügbar.

5. Reproduzierbarkeit:
   - Alle Seeds sind auf 42 gesetzt (np.random.seed(42))
   - NLTK-Downloads erfolgen automatisch (punkt, punkt_tab)
