# Czynności powtarzalne — narzędzie UP

Prosty system do śledzenia czynności, które trzeba wykonywać regularnie, ale bez ściśle określonego harmonogramu.

## Do czego służy

Niektóre zadania nie mają terminów. Po prostu trzeba je wykonywać *mniej więcej* co jakiś czas — wyczyścić filtr w pralce, wymienić szczoteczkę do zębów, sprawdzić gaśnicę. Łatwo o nich zapomnieć, trudno je precyzyjnie zaplanować, a wpisywanie ich do kalendarza to zbędny narzut.

To narzędzie zbiera je w jednym miejscu i śledzi, kiedy każda z nich była ostatnio wykonana.

## Jak to działa

Prowadzona jest tabela z trzema informacjami dla każdej czynności:

- **Co** — krótki opis zadania
- **Jak często** — przybliżona częstość, wybrana z zestawu predefiniowanych przedziałów
- **Ostatnio wykonano** — data ostatniego wykonania

Gdy od ostatniego wykonania minął dolny próg wybranego przedziału, pozycja zostaje delikatnie oznaczona — nie jako zaległa ani niewykonana, ale jako przypomnienie: *chciałeś zajmować się tym mniej więcej tak często, a właśnie nadszedł ten czas.*

## Przedziały częstości

Zamiast wybierać dokładną częstość (co 3 tygodnie? co 28 dni?), czynnościom przypisuje się jeden z kilku przedziałów. Domyślny zestaw to:

- **1–2 miesiące**
- **3–4 miesiące**
- **6–8 miesięcy**

Sens przedziałów — zamiast dokładnych wartości — polega na eliminacji pozornej decyzji. To, czy coś dzieje się co 3 czy co 4 miesiące, rzadko ma znaczenie. Przedział oddaje intencję bez wymagania fałszywej precyzji.

Domyślne przedziały można dostosować do własnych potrzeb.

## Kiedy pojawia się sygnał

Czynność jest oznaczana w momencie, gdy od ostatniego wykonania minął dolny próg jej przedziału. Dla czynności ustawionej na *1–2 miesiące* sygnał pojawia się po miesiącu. Nic nie jest oznaczane wcześniej. Sygnał wynika z ustawień użytkownika i rzeczywistego upływu czasu — nie z założeń samego narzędzia.

## Implementacja

To narzędzie nie zakłada żadnej konkretnej technologii. Można użyć tego, co najlepiej pasuje do własnego stylu pracy:

- Tablicy Trello z kartami i etykietami
- Arkusza kalkulacyjnego (Excel, Google Sheets, Numbers)
- Pliku tekstowego lub tabeli w Markdown
- Kartki i ołówka

Struktura jest metodą. Nośnik należy do użytkownika.

## Zgodność z UP

To narzędzie stosuje zasadę UP — odzwierciedla istniejącą presję, nie dodając własnej:

- Brak narzuconego rytmu — narzędzie nie oczekuje regularnych przeglądów
- Brak kary za nieobecność — powrót po tygodniu zastaje dane dokładnie w takim stanie, w jakim zostały zostawione
- Brak sztucznej pilności — oznaczanie rozpoczyna się dopiero po przekroczeniu progu ustawionego przez użytkownika
- Konfiguracja należy do użytkownika — częstości są wybierane i swobodnie modyfikowane przez użytkownika
