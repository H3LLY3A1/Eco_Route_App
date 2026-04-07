# EcoRouteApp

Repozytorium projektu zespołowego realizowanego w ramach przedmiotu Projektowanie Oprogramowania.

EcoRouteApp to aplikacja mobilna i backend do monitorowania tras użytkownika oraz ekspozycji na zanieczyszczenia powietrza (m.in. PM2.5, PM10, AQI) na podstawie danych ze stacji pomiarowych.

## Co zawiera repozytorium

- Dokumentację projektową.
- Backend API (FastAPI + PostgreSQL + testy).
- Frontend mobilny Android (Kotlin, Gradle).

## Struktura katalogów

```text
.
|- Documentation/
|  |- E1.docx.pdf
|  |- E2.dotm.pdf
|  |- E3 (1).zip
|  |- E4.pdf
|- EcoRouteApp/
|  |- EcoRouteApp/
|  |  |- Backend + Tests/
|  |  |  |- Backend + Tests/
|  |  |  |  |- EcoRouteApp/          # FastAPI backend + testy
|  |  |- Frontend/
|  |  |  |- EcoRouteAppv2/           # Aplikacja Android
|- README.md
```

## Technologie

- Backend: Python, FastAPI, Uvicorn, PostgreSQL, pytest
- Frontend: Kotlin, Android SDK, Gradle
- Konteneryzacja: Docker, Docker Compose

## Szybki start

### 1) Backend

Katalog roboczy backendu:

```text
EcoRouteApp/EcoRouteApp/Backend + Tests/Backend + Tests/EcoRouteApp
```

Uruchomienie lokalne:

```bash
python -m venv .venv
# Windows PowerShell
.venv\Scripts\Activate.ps1
pip install -r backend/requirements.txt
uvicorn backend.main:app --reload
```

API będzie dostępne pod adresem:

```text
http://127.0.0.1:8000
```

Dokumentacja OpenAPI:

```text
http://127.0.0.1:8000/docs
```

Uruchomienie testów backendu:

```bash
pip install -r tests/requirements-test.txt
pytest -q
```

Uruchomienie przez Docker:

```bash
docker-compose up --build
```

### 2) Frontend (Android)

Katalog aplikacji Android:

```text
EcoRouteApp/EcoRouteApp/Frontend/EcoRouteAppv2
```

Uruchomienie:

```bash
./gradlew assembleDebug
```

Na Windows:

```powershell
.\gradlew.bat assembleDebug
```

## Dokumentacja

Artefakty projektowe (analiza, projekt, dokumentacja) znajdują się w katalogu `Documentation/`.

## Uwagi organizacyjne

- Repozytorium zawiera podkatalogi z własnymi konfiguracjami narzędziowymi (backend i frontend).
- Główny `.gitignore` obejmuje typowe artefakty dla Python/Android/IDE i porządkuje pracę całego repo.
