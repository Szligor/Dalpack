# 📦 Magazyn Dalpack

Interaktywny magazyn materiałów działający w przeglądarce telefonu — odwzorowanie bazy Notion „Magazyn materiałów" (kategorie: Mocowanie, Pakowanie, Folia, Pasy, Czujniki; lokalizacje: 🚚 Na aucie i 🏭 Magazyn Opole).

## Funkcje

- **Trzy widoki**: Wszystko / 🚚 Auto / 🏭 Opole (jak widoki w Notion)
- **Liczniki +/−** przy każdej pozycji — przytrzymaj przycisk, żeby liczyć szybciej; stuknij liczbę, żeby wpisać dokładną wartość
- **Przenoszenie** materiału między autem a magazynem Opole jednym stuknięciem
- **Wyszukiwarka** materiałów
- **Dodawanie / edycja / usuwanie** pozycji i kategorii, z cofaniem (Cofnij)
- **Kopia zapasowa**: eksport i import danych do pliku JSON (menu ⋮)
- **Działa offline** (PWA) — po pierwszym otwarciu nie potrzebuje internetu
- Tryb jasny i ciemny (zgodnie z ustawieniem telefonu)

Dane zapisują się w pamięci przeglądarki telefonu (localStorage). Żeby przenieść stan na inne urządzenie, użyj eksportu/importu w menu ⋮.

## Jak otworzyć na telefonie

Aplikacja jest opublikowana na GitHub Pages: **https://szligor.github.io/Dalpack/**

Dodaj ją do ekranu głównego:
- **Android (Chrome)**: menu ⋮ → „Dodaj do ekranu głównego"
- **iPhone (Safari)**: przycisk Udostępnij → „Do ekranu początkowego"

Od tej pory aplikacja otwiera się jak zwykła apka, na pełnym ekranie i offline.

## Publikowanie zmian

Strona jest serwowana z gałęzi `gh-pages`. Po zmianach w kodzie zaktualizuj ją tak:

```bash
git push origin <twoja-gałąź>:gh-pages
```

## Struktura

- `index.html` — cała aplikacja (HTML + CSS + JS, bez zależności)
- `manifest.webmanifest`, `sw.js`, `icons/` — instalacja na telefonie i tryb offline
