<div align="center">

# 💧 AquaMotiv

Prosta, darmowa aplikacja webowa do monitorowania nawodnienia i zużycia filtra w butelce filtrującej (np. Dafi).

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![No dependencies to install](https://img.shields.io/badge/backend-none%20(static%20site)-blue)

**[Polski](#-polski) | [English](#-english)**

</div>

---

## 🇵🇱 Polski

### Spis treści
- [O projekcie](#o-projekcie)
- [Funkcje](#funkcje)
- [Stack technologiczny](#stack-technologiczny)
- [Wymagania](#wymagania)
- [Instalacja](#instalacja)
- [Uruchomienie](#uruchomienie)
- [Użycie](#użycie)
- [Struktura projektu](#struktura-projektu)
- [Licencja](#licencja)
- [Kontakt](#kontakt)

### O projekcie
AquaMotiv to proste narzędzie stworzone, aby pomóc w monitorowaniu ilości wody
przefiltrowanej przez butelkę filtrującą (np. Dafi) oraz w śledzeniu dziennego
nawodnienia. Aplikacja liczy napełnienia butelki, przypomina o zbliżającej się
konieczności wymiany filtra (który nie ma własnego wskaźnika zużycia) i motywuje
do regularnego picia wody komunikatami motywacyjnymi oraz systemem nagród za
osiągnięcie dziennego limitu. Wszystkie dane są zapisywane lokalnie w
przeglądarce użytkownika (`localStorage`) — bez konta, bez backendu, bez
wysyłania danych na zewnątrz.

### Funkcje
- Liczenie napełnień filtra i butelki.
- Monitorowanie dziennego spożycia wody z możliwością ustawienia limitu.
- Alarm informujący o zbliżającej się potrzebie wymiany filtra (próg do
  ustawienia).
- Personalizacja pojemności filtra i butelki oraz imienia użytkownika.
- Przydatne porady dotyczące nawodnienia (sekcja Porady).
- Statystyki z podsumowaniem postępów i sekcją nagród.
- Komunikaty motywacyjne — wyzwalane przyciskiem "Zmotywuj Mnie!" oraz
  automatyczne.
- Udostępnianie aplikacji znajomym (Facebook, Twitter, WhatsApp, e-mail,
  kopiowanie linku).
- Reset dzienny lub całkowity licznika (z potwierdzeniem w modalu).

### Stack technologiczny
- HTML5 / CSS3 / JavaScript (vanilla, bez frameworka JS)
- [Bootstrap 5.3](https://getbootstrap.com/) i [Font Awesome 6.4](https://fontawesome.com/) (z CDN)
- Przechowywanie danych w `localStorage` przeglądarki — brak backendu i bazy danych

### Wymagania
- Dowolna nowoczesna przeglądarka internetowa.
- Do lokalnego uruchamiania: dowolny serwer HTTP (np. XAMPP/Apache, lub
  wbudowany serwer PHP/Pythona) — plik można też otworzyć bezpośrednio jako
  plik lokalny.

### Instalacja
Projekt nie ma zależności do zainstalowania (brak `package.json` / menedżera
pakietów) — wszystkie biblioteki ładowane są z CDN.

```bash
git clone https://github.com/MrPrompt24/AquaMotiv.git
cd AquaMotiv
```

### Uruchomienie
Najprościej uruchomić projekt lokalnie przez serwer PHP (np. w ramach XAMPP):

```bash
php -S localhost:8000
```

Następnie otwórz w przeglądarce `http://localhost:8000/index.html`.

Można też po prostu otworzyć plik `index.html` bezpośrednio w przeglądarce.

### Użycie
1. Przy pierwszym uruchomieniu wejdź w **Ustawienia** (ikona zębatki) i
   uzupełnij: imię, pojemność filtra (L), pojemność butelki (ml), opcjonalny
   dzienny limit napełnień oraz próg alarmu przed wymianą filtra.
2. Na ekranie głównym klikaj **Dodaj Napełnienie** za każdym razem, gdy
   napełnisz butelkę — aplikacja zwiększy liczniki dzienny i filtra.
3. W sekcji **Statystyki** śledź postępy i odbieraj nagrody po osiągnięciu
   dziennego limitu.
4. W sekcji **Porady** znajdziesz wskazówki dotyczące zdrowego nawodnienia.
5. Użyj przycisku **Udostępnij**, aby polecić aplikację znajomym.

> **Uwaga:** wszystkie dane zapisywane są lokalnie w przeglądarce (`localStorage`)
> — nikt poza użytkownikiem nie ma do nich dostępu.

### Struktura projektu
```
AquaMotiv/
├── index.html          # Główny widok aplikacji
├── css/                # Style (style.css, motivation.css, share.css)
├── js/                 # Logika aplikacji (main.js, motivation.js, zmotywuj.js, share.js)
├── images/             # Ikony i grafiki
├── LICENSE
└── README.md
```

### Licencja
Ten projekt jest objęty licencją MIT — zobacz plik [LICENSE](LICENSE).

### Kontakt
Autor: **MrPrompt**
Repozytorium: [github.com/MrPrompt24/AquaMotiv](https://github.com/MrPrompt24/AquaMotiv)

---

## 🇬🇧 English

### Table of Contents
- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Running the App](#running-the-app)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [License](#license)
- [Contact](#contact)

### About
AquaMotiv is a simple tool built to help you track how much water has passed
through your filtering bottle (e.g. Dafi) and monitor your daily hydration.
The app counts bottle fills, reminds you when the filter (which has no
built-in usage indicator) needs replacing, and motivates you to drink water
regularly through motivational messages and a reward system for hitting your
daily goal. All data is stored locally in the browser (`localStorage`) — no
account, no backend, nothing sent externally.

### Features
- Counts filter and bottle fills.
- Tracks daily water intake with an optional daily goal.
- Alerts you when the filter is close to needing replacement (configurable
  threshold).
- Customizable filter/bottle capacity and user name.
- Helpful hydration tips (Tips section).
- Statistics with progress summary and a rewards section.
- Motivational messages — triggered by a "Motivate Me!" button and shown
  automatically.
- Share the app with friends (Facebook, Twitter, WhatsApp, email, copy link).
- Daily or full counter reset (with confirmation modal).

### Tech Stack
- HTML5 / CSS3 / JavaScript (vanilla, no JS framework)
- [Bootstrap 5.3](https://getbootstrap.com/) and [Font Awesome 6.4](https://fontawesome.com/) (via CDN)
- Data persisted in the browser's `localStorage` — no backend or database

### Requirements
- Any modern web browser.
- To run locally: any HTTP server (e.g. XAMPP/Apache, or PHP/Python's
  built-in server) — the file can also be opened directly as a local file.

### Installation
The project has no dependencies to install (no `package.json` / package
manager) — all libraries are loaded from a CDN.

```bash
git clone https://github.com/MrPrompt24/AquaMotiv.git
cd AquaMotiv
```

### Running the App
The simplest way to run it locally is via PHP's built-in server (e.g. inside
XAMPP):

```bash
php -S localhost:8000
```

Then open `http://localhost:8000/index.html` in your browser.

You can also simply open `index.html` directly in your browser.

### Usage
1. On first launch, open **Settings** (gear icon) and fill in: your name,
   filter capacity (L), bottle capacity (ml), an optional daily fill goal,
   and the alarm threshold before filter replacement.
2. On the home screen, click **Add Fill** every time you fill your bottle —
   the app increases the daily and filter counters.
3. Check the **Statistics** section to track progress and get rewards when
   you hit your daily goal.
4. The **Tips** section has hydration advice.
5. Use the **Share** button to recommend the app to friends.

> **Note:** all data is stored locally in the browser (`localStorage`) — no
> one but you has access to it.

### Project Structure
```
AquaMotiv/
├── index.html          # Main app view
├── css/                # Styles (style.css, motivation.css, share.css)
├── js/                 # App logic (main.js, motivation.js, zmotywuj.js, share.js)
├── images/             # Icons and graphics
├── LICENSE
└── README.md
```

### License
This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

### Contact
Author: **MrPrompt**
Repository: [github.com/MrPrompt24/AquaMotiv](https://github.com/MrPrompt24/AquaMotiv)
