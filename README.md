# TOP 5 PIOSENEK NA SPOTIFY W POLSCE
Repo przedstawia **5 najczęściej słuchanych** utworów na spotify w Polsce z dnia 24.11.2026 w dwóch formatach: **JSON** *(JavaScript Object Notation)* oraz **CSV** *(Comma Separated Values)*.

## Zawartość repo:
*`spotify.json` - dane zapisane w strukturze obiektowo tablicowej.
*`spotify.csv` - dane zapisane w formie tabeli.

---

## Charakterystyka formatów:

### 1. JSON 
Składnia jest powiązana z obiektami w języku **JavaScript**, ale format jest kompatybilny z wszystkimi językami.

* **Zastosowania:** stosowany w przypadkach gdy musimy przesłać uporzadkowane dane, przechować je lub odebrać z predefinowanych źródeł
* **Budowa:** plik składa się z **obiektów** `{..}` i **tablic** `[..]`
* **Typ danych:** rozpoznaje typy danych, pozwala na przechowywanie string, number, object, array, boolean, null.
* **Wady i zalety:** prosta i przejrzysta skłabnia, mniej czytelny przy większych zagnieżdżeniach, wymaga pilnowania poprawnego formatowania i walidacji.

### 2. CSV
Przechowuje dane w postaci **tabeli**, kolumny odpowiadają cechom, a wiersze przechowują wartości.

* **Zastosowania:** najlepiej sprawdza się w przechowywaniu danych numerycznych.
* **Budowa:** Plik składa sie z **wierszy** i **kolumn**. Komórki rozdziela się przecinkiem.
* **Typ danych:** nie rozpoznaje typów danych i nie można narzucić formatu.
* **Wady i zalety:** bardzo prosty, plik możemy szybko otworzyc (np w *Excelu*), problemem są białe znaki i różnice w kodowaniu znaków.

---

## Różnice w przedstawieniu danych
Oba pliki przechowują dokładnie te same dane, ale przedstawiają je w inny sposób.

* **Układ danych:** W pliku **CSV** mamy strukturę wierszy i kolumn. W **JSON** dane są zagnieżdżone, główny obiekt zawiera listę, w której wszystko jest osobnym obiektem.
* **Opis wartości:** W **CSV** nagłówki kolumn pojawiają się tylko raz. W **JSON** nazwa klucza stoi przy każdej wartości.
* **Rozróżnienie danych:** W **JSON** tekst jest zawsze w cudzysłowie, a liczby bez niego. W **CSV** używanie cudzysłowia nie jest konieczne i możemy zapisywać dane jako zwykły tekst.

---

## Porównanie JSON i CSV

| Cecha | JSON | CSV |
| ----- | ---- | --- |
| **Struktura** | hierarchiczna, obiekty `{}` i tablice `[]` | prosta tabela |
| **Rozróżnianie danych** | tak | domyślnie nie |
| **Integracja z innymi źródłami** | łatwa dzięki swojej strukturze | problematyczna przez różnice w kodowaniu |
| **Główne zastosowania** | wymiana danych w sieci, komunikacja z API | zestawienia w  tabeli, dane numeryczne |

---

## Czytanie i otwieranie plików:
W zależności od tego w jaki sposób chcemy wykorzystać te dane (rzucic na nie okiem, użyć w jakimś programie) mamy kilka opcji:

* **Plik CSV:** po kliknięciu na niego w github strona od razu przedstawia go w formie tabeli. Możemy te tabele otworzyć też w excelu lub przejrzeć plik w notatniku.
* **Plik JSON:** otworzy się jako zwykły plik tekstowy w dowolnym edytorze lub przeglądarce. 
