# Wprowadzenie do Git i wersjonowania

## Spis treści

1. [Czym jest Git?](#1-czym-jest-git)
2. [Instalacja Git](#2-instalacja-git)
3. [Podstawowe polecenia Git](#3-podstawowe-polecenia-git)
4. [Tworzenie repozytorium](#4-tworzenie-repozytorium)
5. [Dodawanie i zatwierdzanie zmian](#5-dodawanie-i-zatwierdzanie-zmian)
6. [Pushing i pulling](#6-pushing-i-pulling)
7. [Zarządzanie gałęziami](#7-zarządzanie-gałęziami)
8. [Praca zdalna z repozytorium na GitHubie](#8-praca-zdalna-z-repozytorium-na-githubie)

---

## 1. Czym jest Git?

**Git** to system kontroli wersji, który umożliwia śledzenie zmian w plikach i współpracę nad projektami. Pozwala na:

- Zapisywanie historii zmian w projekcie.
- Współpracę wielu osób nad tym samym projektem.
- Tworzenie gałęzi, aby eksperymentować z nowymi funkcjami.

---

## 2. Instalacja Git

### Krok 1: Pobranie Git

1. Wejdź na stronę [git-scm.com](https://git-scm.com/downloads).
2. Pobierz najnowszą wersję Git dla swojego systemu operacyjnego (Windows, macOS, Linux).

### Krok 2: Instalacja Git

- **Windows**:

  1. Uruchom pobrany plik `.exe`.
  2. Postępuj zgodnie z instrukcjami instalatora, zaznaczając opcje, które chcesz włączyć (np. dodanie Git do zmiennych środowiskowych).

- **macOS**:

  1. Otwórz terminal.
  2. Możesz zainstalować Git przez Homebrew, wpisując:

  ```bash
  brew install git
  ```

- **Linux**:

  1. Otwórz terminal.
  2. Wpisz polecenie:

  ```bash
  sudo apt update
  sudo apt install git
  ```

---

## 3. Podstawowe polecenia Git

Oto kilka podstawowych poleceń Git, które warto znać:

- `git init` - Inicjalizuje nowe repozytorium Git.
- `git clone <repo-url>` - Klonuje zdalne repozytorium.
- `git status` - Sprawdza status repozytorium (zmiany, gałęzie itp.).
- `git add <plik>` - Dodaje pliki do staging area (przygotowuje do zatwierdzenia).
- `git commit -m "komentarz"` - Zatwierdza zmiany z komentarzem.
- `git push` - Wysyła lokalne zmiany do zdalnego repozytorium.
- `git pull` - Pobiera zmiany z zdalnego repozytorium.
- `git branch` - Wyświetla listę gałęzi.
- `git checkout <nazwa-gałęzi>` - Przechodzi do innej gałęzi.

---

## 4. Tworzenie repozytorium

Aby stworzyć nowe repozytorium Git:

1. Otwórz terminal i przejdź do katalogu, w którym chcesz utworzyć repozytorium:

   ```bash
   cd /ścieżka/do/katalogu
   ```

2. Wpisz polecenie:

   ```bash
   git init
   ```

To polecenie zainicjalizuje nowe repozytorium Git w tym katalogu.

---

## 5. Dodawanie i zatwierdzanie zmian

### Krok 1: Dodanie plików

1. Stwórz nowy plik lub zmień istniejący.
2. Dodaj pliki do staging area:

   ```bash
   git add <nazwa_pliku>
   ```

   Aby dodać wszystkie zmiany:

   ```bash
   git add .
   ```

### Krok 2: Zatwierdzenie zmian

1. Zatwierdź zmiany z komentarzem:

   ```bash
   git commit -m "Opis zmian"
   ```

---

## 6. Pushing i pulling

### Krok 1: Wysyłanie zmian do zdalnego repozytorium

1. Aby wysłać lokalne zmiany do zdalnego repozytorium, użyj:

   ```bash
   git push origin main
   ```

   (Zastąp `main` nazwą swojej gałęzi, jeśli używasz innej.)

### Krok 2: Pobieranie zmian z zdalnego repozytorium

1. Aby pobrać zmiany, które zostały wprowadzone w zdalnym repozytorium:

   ```bash
   git pull origin main
   ```

---

## 7. Zarządzanie gałęziami

### Krok 1: Tworzenie nowej gałęzi

1. Aby utworzyć nową gałąź, użyj:

   ```bash
   git branch <nazwa_nowej_gałęzi>
   ```

### Krok 2: Przechodzenie między gałęziami

1. Aby przejść na inną gałąź:

   ```bash
   git checkout <nazwa_gałęzi>
   ```

### Krok 3: Usuwanie gałęzi

1. Aby usunąć gałąź:

   ```bash
   git branch -d <nazwa_gałęzi>
   ```

---

## 8. Praca zdalna z repozytorium na GitHubie

Aby pracować z repozytorium na GitHubie:

1. Stwórz nowe repozytorium na GitHubie.
2. Skopiuj adres URL repozytorium (SSH lub HTTPS).
3. Klonuj repozytorium:

   ```bash
   git clone <repo-url>
   ```

4. Po dokonaniu zmian w lokalnym repozytorium, dodaj, zatwierdź i wyślij zmiany jak opisano wcześniej.

---

## Podsumowanie

Git to potężne narzędzie do zarządzania wersjami, które ułatwia pracę nad projektami i współpracę z innymi. Praktykuj używanie podstawowych poleceń Git, aby lepiej zrozumieć jego możliwości i efektywnie zarządzać swoim kodem.
