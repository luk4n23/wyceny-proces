# Karta procesu — Laser (ULAMEX)

Edytowalna, drukowalna karta procesu dla toru lasera (zlecenie zbiorcze).
Pojedynczy statyczny plik `index.html` — bez builda, bez zależności. Logo firmowe zaszyte w pliku.

## Funkcje
- Nagłówek zlecenia: nr zlecenia, klient, data przyjęcia, termin.
- Tabela detali (1 wiersz = 1 detal): nazwa, materiał, grubość, ilość, plik DXF, podpis.
- Kolumny etapów **R / C / P** (rozkrój / cięcie / pakowanie) — checkbox zaznaczany po wykonaniu.
- Przyciski: **+ Dodaj detal**, **Wyczyść**, **Drukuj / zapisz PDF**.
- Kontrola jakości (checklista) + pole uwag.
- Autozapis treści w przeglądarce (localStorage) — dane nie znikają po odświeżeniu.

## Uruchomienie lokalne
Otwórz `index.html` w przeglądarce (dwuklik) — to wszystko.

## Wdrożenie na Render (Static Site)
1. Wypchnij ten katalog do repozytorium na GitHub.
2. Render → **New** → **Static Site** → wskaż repozytorium.
3. Ustawienia:
   - **Build Command:** *(puste)*
   - **Publish Directory:** `.`
4. Deploy. Strona serwuje `index.html`.

## Druk
Przycisk **Drukuj / zapisz PDF** otwiera systemowy dialog druku (format A4).
Przy dłuższej liście detali wydruk automatycznie przechodzi na kolejne strony.
