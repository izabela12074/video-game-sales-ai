# 🤖 Automatyzacja Raportowania Biznesowego z AI (LLM)

> Automatyczne generowanie insightów biznesowych i rekomendacji strategicznych z użyciem modeli językowych | na podstawie danych sprzedażowych gier wideo

## 📌 O projekcie

Projekt demonstruje jak modele językowe (LLM) mogą wspierać analityka danych w automatycznym generowaniu insightów biznesowych i rekomendacji strategicznych na podstawie zagregowanych danych sprzedażowych.

Analiza przeprowadzona na publicznym datasecie zawierającym globalne dane sprzedaży gier wideo (źródło: Kaggle). Projekt skupia się na **praktycznej integracji AI w workflow raportowania** – nie na budowie modeli predykcyjnych.

## 🎯 Problem biznesowy

Firmy działające globalnie (np. wydawcy gier, firmy produktów cyfrowych) muszą regularnie analizować:
- trendy sprzedażowe
- wydajność platform i produktów
- różnice regionalne

Manualne przygotowanie raportów analitycznych i wniosków strategicznych jest **czasochłonne i trudne do skalowania**. Projekt pokazuje jak AI może przyspieszyć ten proces.

## 🧠 Cele projektu

- Przygotowanie strukturalnych danych sprzedażowych do analizy biznesowej
- Automatyczne generowanie insightów biznesowych z użyciem AI (LLM)
- Demonstracja jak AI może przyspieszyć raportowanie i procesy decyzyjne

## 🛠️ Zakres prac

### 1️⃣ Przygotowanie i analiza danych (Python)
- Wczytanie i czyszczenie danych (obsługa brakujących wartości w kolumnie `Year`)
- Agregacja sprzedaży:
  - Globalne trendy czasowe
  - Wydajność platform
  - Wydajność gatunków
  - Wydajność wydawców
  - Sprzedaż regionalna (NA, EU, JP, Other)

### 2️⃣ Agregacja danych dla AI
Zamiast przekazywać surowe dane do LLM, przygotowano strukturalne podsumowania biznesowe zawierające:
- Łączną globalną sprzedaż
- Top platformy, gatunki i wydawców
- Porównanie sprzedaży regionalnej
- Ostatnie trendy sprzedażowe

Wynik zapisany jako `ai_input_summary.json` – AI otrzymuje czysty, skontekstualizowany input gotowy do analizy biznesowej.

### 3️⃣ Analiza biznesowa z AI (LLM)
Zagregowane dane przekazane do modelu językowego wraz z kontekstem biznesowym. AI wygenerowało:
- Kluczowe insighty biznesowe
- Potencjalne ryzyka
- Rekomendacje strategiczne dla przyszłych premier produktów

## 🤖 Rola AI w projekcie

W tym projekcie AI pełni rolę **wirtualnego analityka biznesowego** który:
- Interpretuje dane liczbowe
- Identyfikuje wzorce i trendy
- Wspiera podejmowanie decyzji strategicznych

Projekt demonstruje praktyczne zastosowanie **prompt engineeringu** w workflow analizy danych.

## 📈 Wyniki

- Symulowane skrócenie czasu przygotowania raportów
- Czytelne, strukturalne insighty biznesowe w formacie tekstowym
- Insighty wygenerowane przez AI zwalidowane względem dashboardów Power BI
- Projekt ilustruje jak AI może **uzupełniać** tradycyjne narzędzia BI, a nie je zastępować

## 🧰 Stack technologiczny

| Technologia | Zastosowanie |
|---|---|
| Python (pandas, numpy) | Przygotowanie i agregacja danych |
| matplotlib, seaborn | Wizualizacja trendów sprzedażowych |
| Jupyter Notebook | Środowisko analizy |
| AI / LLM | Analiza tekstowa, prompt engineering |
| JSON | Struktura danych wejściowych dla AI |

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

## 🚀 Możliwe rozszerzenia

- Integracja z dashboardami Power BI
- Automatyczne cykliczne raportowanie (np. aktualizacje miesięczne)
- Wdrożenie jako wewnętrzny asystent raportowania

## 👩‍💻 Autor

**Izabela Popiołek** – Specjalista ds. Digitalizacji | Power BI Developer | AI Analyst  
[LinkedIn](https://linkedin.com/in/izabela-popiolek) | [GitHub](https://github.com/izabela12074)
