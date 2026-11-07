# LinkTalk — procedura publikacji pliku APK

Ten dokument opisuje bezpieczną kolejność przygotowania wersji Android. Nie uruchamia automatycznie żadnego wdrożenia.

## 1. Ustal właściwe źródło

Kod aplikacji jest w [DominikSolorz/LinkTalk](https://github.com/DominikSolorz/LinkTalk). Sprawdź aktualną gałąź źródłową i commit, z których budowany jest APK. Nie zakładaj, że `main` jest aktualną aplikacją produkcyjną. HOME SECURITY jest osobnym projektem i nie należy go używać do tego wydania.

## 2. Zbuduj i sprawdź

Przygotuj wydanie z kontrolowanego commita. Wykonaj testy wymagane dla danego wariantu Android oraz sprawdź identyfikator pakietu, numer wersji, minSdk, docelową platformę, logowanie, uprawnienia i uruchamianie na urządzeniu testowym. Nie dodawaj sekretów, kluczy podpisujących ani prywatnych danych do repozytorium.

## 3. Zweryfikuj paczkę

Oblicz SHA-256 z gotowego APK i sprawdź jego podpis odpowiednimi narzędziami Android. Sama nazwa pliku ani metadane GitHub nie są dowodem poprawnego podpisu. Upewnij się, że nazwa pliku, numer wersji aplikacji i tag wskazują to samo wydanie.

## 4. Opublikuj

Opublikuj **nowy** tag i nowe wydanie w [GitHub Releases](https://github.com/DominikSolorz/LinkTalk-Releases/releases) z opisem zmian, statusem (testowe/stabilne), datą, wersją, wymaganiami i załącznikiem APK. Nie nadpisuj starego wydania ani nie kasuj archiwalnych paczek bez uzgodnionej procedury.

## 5. Potwierdź wynik

Sprawdź, czy opublikowany załącznik można pobrać, czy SHA-256 pobranych bajtów odpowiada oczekiwanej wartości, czy podpis jest zgodny oraz czy test instalacji i aktualizacji zakończył się powodzeniem. Dopiero wtedy uzupełnij [KATALOG-WYDAN.md](KATALOG-WYDAN.md). Odnotuj osobno kod źródłowy, commit, tag, plik, SHA-256 i rzeczywisty status wdrożenia.

**Nie wykonuj publikacji w imieniu użytkownika bez jego wyraźnej decyzji dotyczącej konkretnego wydania.**
