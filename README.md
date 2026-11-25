# Garaż – koszty pojazdów

Jednoplikowa aplikacja webowa (`index.html`) do prowadzenia kosztów aut, z synchronizacją przez prywatny GitHub Gist i eksportem do Excela.

## Publikacja na GitHub Pages

1. Utwórz nowe repozytorium na GitHubie (może być prywatne, jeśli masz plan, który pozwala na Pages z prywatnych repo; inaczej publiczne – dane i tak są w giście, nie w repo).
2. Wrzuć do niego wszystkie pliki: `index.html`, `icon.svg`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `manifest.webmanifest` (i ten README).
3. Settings → Pages → Source: „Deploy from a branch”, Branch: `main`, folder `/ (root)` → Save.
4. Po minucie aplikacja będzie pod adresem `https://<twoj-login>.github.io/<nazwa-repo>/`.

## Synchronizacja

1. Utwórz token: https://github.com/settings/tokens/new?scopes=gist (classic, tylko uprawnienie **gist**).
2. W aplikacji kliknij „Tylko lokalnie” → wklej token → „Połącz”. Aplikacja sama znajdzie lub utworzy prywatny gist z plikiem `garaz-koszty-pojazdow.json`.
3. Na telefonie i innych komputerach wklej ten sam token.

Zmiany są scalane wpis po wpisie, więc dodanie czegoś na dwóch urządzeniach naraz nie nadpisze danych.

## Przeniesienie starego arkusza

„Excel / dane” → „Wczytaj arkusz Excela” i wskaż dotychczasowy plik. Zakładki w formacie `Auto - Kategoria` zamienią się na auta i kategorie.

## Ikona na ekranie telefonu

- iPhone (Safari): Udostępnij → „Do ekranu początkowego”.
- Android (Chrome): menu ⋮ → „Dodaj do ekranu głównego” / „Zainstaluj aplikację”.
