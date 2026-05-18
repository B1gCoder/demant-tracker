# Demant Tracker 🏭

Demant Tracker to w pełni responsywna, chmurowa aplikacja webowa stworzona z myślą o operatorach produkcji. Narzędzie cyfryzuje i automatyzuje proces obliczania codziennej wydajności operacyjnej (KPI), zastępując ręczne kalkulacje i arkusze kalkulacyjne. 

Projekt powstał z realnej potrzeby optymalizacji śledzenia realizacji norm czasowych i ilościowych na linii produkcyjnej.

## 🚀 Główne funkcjonalności

* **Automatyczne kalkulacje KPI:** System w czasie rzeczywistym przelicza zaraportowane sztuki oraz czas pracy na procentowy wskaźnik realizacji normy (z dynamicznym oznaczaniem kolorami wyników poniżej i powyżej oczekiwań).
* **Zarządzanie Słownikiem Zadań:** Wbudowany panel CRUD do definiowania własnych obróbek, z podziałem na kategorie (`Procesy` i `Przeróbki`).
* **System Miesięcznych Celów:** Możliwość nadpisywania domyślnych norm dedykowanymi celami narzuconymi przez Liderów na dany miesiąc. Aplikacja "zamraża" użytą normę w momencie zapisu, co chroni historyczne statystyki przed przekłamaniem po zmianie celów w kolejnym miesiącu.
* **Pełna synchronizacja (Cloud):** Dzięki architekturze Serverless, dane są natychmiast synchronizowane. Wyniki można wygodnie wprowadzać na telefonie (mobile-first) w trakcie przerwy, a analizować na komputerze w domu.
* **Zarządzanie Historią:** Automatyczne grupowanie wpisów według daty z możliwością bezpiecznego usuwania logów z zachowaniem integralności bazy danych.

## 💻 Wykorzystane technologie (Tech Stack)

Aplikacja została zbudowana w oparciu o czysty kod, bez ciężkich frameworków frontendowych, co gwarantuje jej błyskawiczne ładowanie i działanie.

* **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6+ / Fetch API)
* **Backend / Baza Danych:** Supabase (PostgreSQL, REST API)
* **Hosting:** GitHub Pages
* **Architektura:** Serverless / SPA (Single Page Application)

## 🎨 Interfejs Użytkownika (UI/UX)

Interfejs został zaprojektowany od podstaw w nowoczesnym stylu **Dark Glassmorphism** (efekt matowego szkła). Wykorzystanie głębokich, ciemnych barw (Dark Mode) połączonych z gradientami nie tylko nadaje aplikacji wygląd premium, ale przede wszystkim minimalizuje zmęczenie wzroku podczas korzystania z niej w warunkach przemysłowych lub po zakończonej zmianie.

## ⚙️ Struktura Bazy Danych

Projekt opiera się na relacyjnej bazie PostgreSQL zawierającej dwie główne tabele połączone kluczem obcym:
1. `processes` - Przechowuje słownik zadań (nazwa, typ, domyślna norma, cel miesięczny).
2. `daily_logs` - Przechowuje historię wpisów (data, przepracowane godziny, wykonane sztuki, "zamrożona" norma użyta do obliczeń).

---
*Projekt stworzony w celu optymalizacji codziennej pracy na hali produkcyjnej.*
