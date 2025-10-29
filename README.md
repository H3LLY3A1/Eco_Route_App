# 💻 Projektowanie Oprogramowania (Software Design)

**Politechnika Wrocławska (lub inna Uczelnia)**
**Wrocław, Semestr [Wpisz: Zimowy/Letni], 2025/2026**

Repozytorium to zawiera pełną **dokumentację projektową, modele UML oraz prototyp kodu źródłowego** systemu tworzonego w ramach przedmiotu **Projektowanie Oprogramowania**. Projekt jest realizacją systematycznego procesu wytwarzania oprogramowania, od analizy wymagań po testowanie.

| Aspekt | Szczegóły |
| :--- | :--- |
| **Typ Zajęć** | 30h Wykład (W) + 30h Projekt (P) |
| **Wymagania Wstępne** | Zaliczenie przedmiotu: **Podstawy inżynierii oprogramowania (ćwiczenia)** |
| **Zespół Projektowy** | [Wpisz Imię Nazwisko 1], [Wpisz Imię Nazwisko 2], [Wpisz Imię Nazwisko 3] |
| **Temat Wiodący** | [Wpisz temat wiodący projektu (np. System Zarządzania Wypożyczalnią Sprzętu)] |

***

## 🎯 Cele i Efekty Uczenia się

Głównym celem jest opanowanie cyklu życia oprogramowania wg **ISO/IEC 12207**, stosowanie **dobrych praktyk projektowych** (w tym **wzorców projektowych**) oraz umiejętność tworzenia **dokumentacji technicznej** w języku **UML**.

### Kluczowe Umiejętności (PEK\_U)
* Stosowanie **UML** do specyfikacji wymagań i modelowania domeny (**PEK\_U01**).
* Projektowanie **Graficznego Interfejsu Użytkownika (GUI)** (**PEK\_U02**).
* Adaptacja **wzorców architektonicznych/projektowych** (**PEK\_U03**).
* **Implementacja** funkcjonalności i specyfikacja **testów funkcjonalnych** (**PEK\_U04**).

***

## 🛠️ Stosowane Narzędzia i Technologie

### 📝 Modelowanie (UML)
* **UML Designer** / **Visual Paradigm** / **Diagrams.net**
* **Dokumentacja:** Edytor tekstowy, arkusz kalkulacyjny

### 💻 Implementacja
* **Język Programowania:** [Wpisz używany język, np. Java/Python/C#]
* **Środowisko:** [Wpisz używane IDE]
* **Testowanie:** [Wpisz używane narzędzia, np. JUnit, Selenium]
* **Analiza Jakości:** [Wpisz używane narzędzia, np. JDepend]

***

## 📂 Struktura Repozytorium i Harmonogram (Artefakty Projektu)

Repozytorium jest zorganizowane zgodnie z fazami projektu, które odzwierciedlają kolejne etapy wytwarzania oprogramowania.

### 1. 📃 Analiza i Koncepcja (Deadline: P4)
Katalog: `01_Koncepcja_Analiza/`

| P# | Artefakt | Opis |
| :--- | :--- | :--- |
| P2 | **Wizja i Słownik** | Definicja celów, użytkowników i terminologii projektu. |
| P3 | **Model Domenowy (UML)** | Diagram klas domenowych i związków. |
| P3 | **Reguły Biznesowe** | Minimum 10 reguł (RuleSpeak/język naturalny), spójne z modelem. |

### 2. 📝 Specyfikacja Wymagań (Deadline: P8)
Katalog: `02_Specyfikacja_Wymagan/`

| P# | Artefakt | Opis |
| :--- | :--- | :--- |
| P4 | **Specyfikacja Wymagań** | Diagram wymagań lub zbiór historyjek użytkownika (śladowalność do wizji). |
| P5 | **Diagram Przypadków Użycia (PU)** | Model PU z opisami streszczającymi. |
| P6 | **Specyfikacja PU** | Scenariusze dla 2 wybranych PU (wątki główne i alternatywne, indywidualnie). |
| P6 | **Model Informacyjny (UML)** | Uszczegółowiony model domenowy (atrybuty, ewentualnie **OCL** *opcjonalnie*). |
| P7 | **Prototyp Interfejsu** | Wizualny prototyp GUI dla głównych wątków PU. |

### 3. 🏗️ Projektowanie (Deadline: P11)
Katalog: `03_Projektowanie_Architektura/`

| P# | Artefakt | Opis |
| :--- | :--- | :--- |
| P8-9 | **Architektura Systemu** | Logiczna (Diagram Pakietów, Wzorzec Architektoniczny) i Fizyczna (Diagram Rozmieszczenia). |
| P8-9 | **Projekt Bazy Danych** | Model logiczny danych (diagram klas/encji lub definicja tabel) jako uszczegółowienie modelu informacyjnego. |
| P10 | **Realizacja PU (UML)** | Diagramy **Klas i Sekwencji** dla zaimplementowanych PU (projekt szczegółowy). |

### 4. 🚀 Implementacja i Testowanie (Deadline: P14)
Katalog: `04_Implementacja_Testy/`

| P# | Artefakt | Opis |
| :--- | :--- | :--- |
| P11 | **Implementacja Interfejsu** | Kod źródłowy GUI zgodny z prototypem. |
| P12 | **Implementacja Logiki** | Kod źródłowy logiki aplikacji (wątki główne i alternatywne, wykorzystanie **wzorców projektowych**). |
| P13 | **Testy Jednostkowe** | Kod testów dla logiki biznesowej (min. 2 metody/studenta). |
| P14 | **Testy Funkcjonalne** | Tekstowe przypadki testowe oraz skrypty do **automatyzacji testów**. |
| P14 | **Badanie Jakości** | Raport z wynikami **metryk jakości** kodu i wnioskami (*opcjonalnie*). |

***

## ⚠️ Zasady i Wymogi Zaliczenia Projektu

1.  **Obowiązkowa Implementacja:** Każdy student **MUSI zaimplementować przynajmniej 1 przypadek użycia** w ramach projektu.
2.  **Kary za Opóźnienia:** Za oddanie prac po terminie zespół otrzymuje **-5p.** za każdy tydzień spóźnienia.
3.  **Plagiat/Kopia:** Użycie nieswojego rozwiązania skutkuje **oceną niedostateczną (ndst)** i skierowaniem sprawy do Komisji Dyscyplinarnej.
4.  **Punkty Opcjonalne (\*):** Punkty oznaczone gwiazdką są dodatkowe i mogą pomóc w osiągnięciu wyższej oceny.

### Skala Ocen (dla 1 osoby, maks. 145p. + 30p.\*)
| Procent | Punkty | Ocena |
| :--- | :--- | :--- |
| `< 50%` | `< 72.5 p.` | **ndst (2.0)** |
| `[50%, 60%)` | `73 – 87 p.` | **dst (3.0)** |
| `[60%, 70%)` | `87.5 – 101.5 p.` | **dst+ (3.5)** |
| `[70%, 80%)` | `102 – 116 p.` | **db (4.0)** |
| `[80%, 90%)` | `116.5 – 130.5 p.` | **db+ (4.5)** |
| `[90%, 100%]` | `> 131 p.` | **bdb (5.0)** |
