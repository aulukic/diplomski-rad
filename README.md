# Empirijska analiza algoritama stabala odlučivanja i ansambl metoda

Ovaj repozitorij sadrži cjelokupni izvorni kod i rezultate diplomskog rada fokusiranog na usporedbu performansi, robusnosti i računske složenosti algoritama stabala odlučivanja.

## 🚀 Sažetak Projekta
Istraživanje obuhvaća evoluciju od izvornih algoritama (**ID3**, **C4.5**) do modernih ansambala (**Random Forest**, **XGBoost**). Testiranje je provedeno na 5 raznolikih UCI skupova podataka (Iris, Bank Marketing, Adult, Breast Cancer, Wine Quality) kroz 8 različitih klasifikacijskih i regresijskih zadataka.

## 💻 Hardverska Arhitektura (Hibridno Okruženje)
Projekt je razvijan koristeći hibridni pristup:
1. **Google Colab (Prototipiranje):** Inicijalna obrada podataka i razvoj modela.
2. **Lokalna Radna Stanica (Finalni Benchmark):**
   - **CPU:** AMD Ryzen 7 7840HS (8C/16T, up to 5.1 GHz)
   - **GPU:** NVIDIA GeForce RTX 4070 (Laptop, 8GB VRAM, CUDA 12.x)
   - **RAM:** 32 GB DDR5 5600 MHz

## 📊 Ključni Rezultati
- **Superiornost ansambala:** Random Forest i XGBoost statistički značajno nadmašuju pojedinačna stabla na kompleksnim podacima (p < 0.05).
- **GPU Skalabilnost:** Dokazano je da XGBoost na GPU-u zadržava linearno vrijeme izvođenja pri rastu podataka, dok CPU modeli pokazuju eksponencijalni rast.
- **Interpretabilnost:** Korištenjem **SHAP** metodologije (teorija igara), dekonstruirani su "black-box" modeli te su izvučene poslovne smjernice za Bank Marketing kampanje.

## 📂 Organizacija Repozitorija
- `notebooks/`: Sadrži Jupyter bilježnice s kodom za treniranje i evaluaciju.
- `results/plots/`: Vizualizacije distribucija, performansi i SHAP analiza.
- `results/tables/`: Detaljni .csv izvještaji o unakrsnoj validaciji (10-fold CV).

## 🛠️ Kako pokrenuti
1. Klonirajte repozitorij:
   ```bash
   git clone [https://github.com/aulukic/diplomski-rad](https://github.com/aulukic/diplomski-rad.git)

2. Instalirajte ovisnosti:
```bash
   pip install -r zahtjevi.txt

Pokrenite bilježnice unutar notebooks/ mape.

⚖️ Licenca
Ovaj projekt je razvijen u akademske svrhe (Diplomski rad - FOI).
