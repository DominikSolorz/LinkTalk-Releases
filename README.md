# 03 / LinkTalk Releases — publiczne pliki do pobrania

**Adres repozytorium:** https://github.com/DominikSolorz/LinkTalk-Releases  
**Pobieranie wersji:** https://github.com/DominikSolorz/LinkTalk-Releases/releases  
**Kod aplikacji:** [DominikSolorz/LinkTalk](https://github.com/DominikSolorz/LinkTalk) (repozytorium prywatne, dostęp wymaga uprawnień)

To jest repozytorium wydań, **a nie miejsce edycji aplikacji**. Pliki binarne znajdują się przede wszystkim w zakładce **Releases**, dlatego sam katalog plików `main` może być niemal pusty.

## Szybka nawigacja po wydaniach

Po otwarciu katalogu [docs/](docs/) znajdziesz [katalog zweryfikowanych wydań](docs/KATALOG-WYDAN.md) z konkretnym plikiem APK, datą i sumą SHA-256 podaną przez GitHub, a także [procedurę przygotowania nowej wersji](docs/PROCEDURA-WYDANIA.md).

## Aktualnie potwierdzone wydanie

`v1.0.0-preview.1` — **LinkTalk Android Preview 1**. Plik: `LinkTalk-1.0.0-preview.1.apk`. To wersja testowa z 17.07.2026; nie jest gwarancją aktualnej wersji produkcyjnej i nie jest aplikacją HOME SECURITY.

## Prosty podział

| Zadanie | Miejsce |
| --- | --- |
| Poprawa wyglądu, ofert, kont, połączeń API LinkTalk | `DominikSolorz/LinkTalk` |
| Zmiana numeru kodu aplikacji | `DominikSolorz/LinkTalk` / `package.json` na właściwej gałęzi źródłowej |
| Testy i budowanie pakietu APK | źródła oraz właściwy workflow projektu LinkTalk |
| Publiczny plik APK i notatki wydania | **`DominikSolorz/LinkTalk-Releases` / zakładka Releases** |
| Windows HOME SECURITY, kamera, PWA | `DominikSolorz/dominiksolorz.github.io`, nigdy tutaj |

## Zasady publikacji

Każde wydanie ma otrzymać jednoznaczny tag (np. `vX.Y.Z` lub `vX.Y.Z-preview.N`), nazwę pliku z tym samym numerem, datę, informację o zmianach i sumę kontrolną SHA-256 wyliczoną z gotowego pliku. Nie deklaruj podpisu cyfrowego, jeśli nie został niezależnie sprawdzony. Nie nadpisuj starego tagu innym APK; opublikuj nowe wydanie. Nie dodawaj tutaj kluczy, tokenów, bazy użytkowników ani kodu produkcyjnej aplikacji.

Skróty do zlecania agentom: [AGENT-SHORTCUTS.md](AGENT-SHORTCUTS.md).

Instrukcje dla agentów: [AGENTS.md](AGENTS.md). Pliki i wersje można zobaczyć w [Releases](https://github.com/DominikSolorz/LinkTalk-Releases/releases).
