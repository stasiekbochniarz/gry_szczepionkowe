# Gry Szczepionkowe na Sieciach Społecznych (Vaccine Games on Social Networks)

Interdyscyplinarny projekt badawczy łączący **teorię gier, epidemiologię, rachunek prawdopodobieństwa oraz analizę numeryczną**. Projekt skupia się na modelowaniu decyzji o zaszczepieniu się z perspektywy racjonalnych jednostek powiązanych strukturą sieci społecznej.

Projekt realizowany w ramach działalności naukowej (rok akademicki 2026).

---

##  O projekcie

Model bada zachowania strategiczne agentów w sieci, którzy decydują się na przyjęcie szczepionki (koszt pewny) lub pozostanie podatnym na zakażenie (ryzyko zachorowania i koszty choroby). Głównym celem jest analiza dynamiki rozprzestrzeniania się chorób zakaźnych (model SIR) na różnych topologiach grafowych oraz weryfikacja stanów **równowagi Nasha**.

### Kluczowe elementy projektu:
* **Generowanie struktur sieciowych:** Tworzenie grafów losowych Erdősa-Rényiego (ER) oraz sieci bezskalowych Barabásiego-Alberta (BA) przy użyciu biblioteki `networkx`.
* **Stochastyczna dynamika epidemii:** Symulacja rozprzestrzeniania się patogenu na sieci w oparciu o dyskretny model SIR.
* **Racjonalne decyzje agentów:** Estymacja wektora prawdopodobieństw zakażenia $\boldsymbol{\pi}$ metodą Monte Carlo.
* **Analiza równowagi Nasha:** Weryfikacja stabilności profili strategii z uwzględnieniem tolerancji numerycznej (`tol`) dla stanów granicznych.

---

##  Struktura repozytorium

* `notebooks/` – Główny notatnik Jupyter zawierający pełny kod symulacji, opisy analityczne oraz wizualizacje.
* `src/` *(opcjonalnie)* – Moduły z funkcjami pomocniczymi (jeśli kod został wydzielony do plików `.py`).
* `README.md` – Dokumentacja projektu.

---

##  Wymagania i instalacja

Do uruchomienia symulacji potrzebne jest środowisko Python oraz następujące pakiety:

```bash
pip install numpy scipy matplotlib networkx
