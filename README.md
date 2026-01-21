# 🤖 Automatyzacja raportowania biznesowego z wykorzystaniem AI (LLM)

## 📌 Opis projektu

Projekt pokazuje, w jaki sposób **LLM** mogą wspierać analityka danych w automatycznym generowaniu **insightów biznesowych i rekomendacji strategicznych** na podstawie zagregowanych danych sprzedażowych.

Analiza została przeprowadzona na publicznym zbiorze danych dotyczącym **globalnej sprzedaży gier wideo** (źródło: kaggle.com).

---

## 🎯 Problem biznesowy

Firmy działające globalnie (np. wydawcy gier, produktów cyfrowych) muszą regularnie analizować:

* trendy sprzedażowe,
* wydajność platform i produktów,
* różnice regionalne,

Jednocześnie **ręczne przygotowanie raportów i wniosków** jest czasochłonne i trudne do skalowania.

---

## 🧠 Cel projektu

* przygotowanie danych sprzedażowych do analizy biznesowej,
* automatyczne wygenerowanie insightów przy użyciu AI (LLM),
* pokazanie, jak AI może **przyspieszyć proces raportowania i podejmowania decyzji**.

---

## 🛠 Zakres prac

### 1️⃣ Przygotowanie i analiza danych (Python)

* wczytanie i czyszczenie danych (usunięcie braków w kolumnie `Year`),
* agregacja sprzedaży:

  * globalnie (trend czasowy),
  * według platform,
  * według gatunków,
  * według wydawców,
  * według regionów (NA, EU, JP, Other).

### 2️⃣ Agregacja danych dla AI

Zamiast przekazywać do AI surowe dane, przygotowano **zagregowane podsumowania biznesowe**, obejmujące:

* całkowitą sprzedaż globalną,
* top platformy,
* top gatunki,
* top wydawców,
* sprzedaż regionalną,
* ostatnie trendy sprzedażowe.

Dane zostały zapisane w pliku `ai_input_summary.json`.

### 3️⃣ Analiza biznesowa z wykorzystaniem AI (LLM)

Dane zagregowane zostały przekazane do **modelu językowego (LLM)** wraz z kontekstem biznesowym.

AI wygenerowało:

* kluczowe insighty,
* potencjalne ryzyka,
* rekomendacje strategiczne dla przyszłych wydań produktów.

---

## 🤖 Rola AI w projekcie

AI pełni rolę **wirtualnego analityka biznesowego**, który:

* interpretuje dane liczbowe,
* identyfikuje trendy i zależności,
* wspiera proces decyzyjny.

Projekt demonstruje **praktyczne zastosowanie prompt engineeringu** w analizie danych.

---

## 📈 Rezultaty

* skrócenie czasu analizy i raportowania (symulacja procesu),
* czytelne insighty biznesowe w formie tekstowej,
* Rezultaty analizy AI zostały zweryfikowane w odniesieniu do dashboardów Power BI.

---

## 🧰 Stack technologiczny

* Python (pandas, numpy, matplotlib, seaborn)
* Jupyter Notebook
* AI / LLM (analiza tekstowa, prompt engineering)
* JSON / Markdown

---

## 📁 Struktura repozytorium

```
video-game-sales-ai/
│
├── data/
│   └── vgsales.csv
│
├── notebooks/
│   └── 01_data_analysis.ipynb
│
├── output/
│   ├── ai_input_summary.json
│   └── ai_business_report.md
│ 
├── prompts/
│   └── ai_prompt.md
│
└── README.md
```

---

## 🚀 Możliwe rozszerzenia

* integracja z Power BI (walidacja insightów AI),
* cykliczne raportowanie (np. miesięczne).

---

## 👩‍💻 Autor

Projekt wykonany jako element **portfolio Data Analyst / Specjalisty ds. AI**.
