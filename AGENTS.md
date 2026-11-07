# Instrukcje dla agentów — 03 / LinkTalk-Releases

Krótkie aliasy zadań `LTR-WYDANIA`, `LTR-APK` itd.: [AGENT-SHORTCUTS.md](AGENT-SHORTCUTS.md).

Repozytorium `DominikSolorz/LinkTalk-Releases` ma jeden cel: udostępniać użytkownikom oficjalne paczki instalacyjne LinkTalk i opis zmian. Nie jest repozytorium źródeł. Sam katalog `main` może być pusty, ponieważ właściwe APK są w GitHub Releases.

Jeżeli zadanie wymaga zmian kodu, UI, konta, katalogu albo API: przenieś je do `DominikSolorz/LinkTalk`, na właściwą bazę kodu, ustaloną po sprawdzeniu wdrożeń. Nie edytuj pliku `app.js` tutaj, bo go nie ma. Nie dotykaj `DominikSolorz/dominiksolorz.github.io` — to HOME SECURITY, osobny produkt.

Dla każdego nowego pliku: sprawdź pochodzenie i uprawnienia do dystrybucji, testy, dokładny tag i nazwę APK, sumę SHA-256, datę i treść release notes. Nie publikuj tokenów ani materiałów prywatnych. Nie uznawaj pliku za podpisany bez walidacji. Nie zmieniaj już opublikowanych tagów i assetów bez jasnego polecenia i planu migracji. Nie twórz publicznego APK na podstawie niezweryfikowanego brancha.

Ostatnie potwierdzone wydanie w chwili tworzenia mapy: `v1.0.0-preview.1` z plikiem `LinkTalk-1.0.0-preview.1.apk`. Aktualność zawsze sprawdź w GitHub Releases.

Na końcu podaj: repo źródłowe, commit, tag, asset, SHA-256, wyniki testów i rzeczywisty URL wydania.

## Obowiązek prowadzenia katalogu wydań

Przed zadaniem publikacji przeczytaj [procedurę wydania](docs/PROCEDURA-WYDANIA.md) i [katalog istniejących wydań](docs/KATALOG-WYDAN.md). Każda nowa paczka ma mieć czytelną nazwę z wersją, odpowiedni tag, właściwy stan `prerelease` lub stabilny, źródłowy commit, zweryfikowaną sumę SHA-256 i potwierdzony podpis.

Po publikacji zweryfikuj plik z GitHub Releases i uaktualnij dokumentację, ale **nigdy nie deklaruj instalacji ani działania na urządzeniu bez rzeczywistego testu**. Stare wydania i ich assety zachowuj do audytu i bezpiecznej aktualizacji. W tym repo nie tworzy się nowych kopii kodu React ani plików HTML aplikacji.
