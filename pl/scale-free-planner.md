# Planer Scale-Free — narzędzie UP

Narzędzie do długofalowego planowania, w którym poziom szczegółowości wynika z odległości w czasie — nie z decyzji planującego.

## Do czego służy

Większość narzędzi do planowania działa na jednym poziomie szczegółowości — tygodniowy planer, tablica projektowa, kwartalny roadmap. Przełączanie między nimi oznacza utrzymywanie kilku równoległych systemów i ręczne synchronizowanie ich ze sobą.

Scale-Free Planner obejmuje wszystkie horyzonty jednocześnie. Bliskie przedziały są wąskie i konkretne; odległe — szerokie i przybliżone. Struktura odzwierciedla to, jak planowanie naprawdę działa: wiadomo, co się robi w tym tygodniu, ma się ogólne pojęcie o następnym kwartale, a dalej operuje się raczej intencjami niż zobowiązaniami.

## Jak to działa

Zadania i plany przydzielane są do przedziałów czasowych. Przedziały są skwantowane — stanowią stały zestaw interwałów — ale ich szerokość rośnie wraz z odległością od teraźniejszości. Domyślny zestaw przedziałów, od najdłuższego do najkrótszego:

- **4 lata** — wyrównane do stałej siatki (2001–2004, 2005–2008, …), dzielącej wiek na 25 równych przedziałów; końcowy rok każdego okresu zawsze dzieli się przez 4
- **2 lata**
- **1 rok**
- **Pół roku**
- **Kwartał**
- **Miesiąc**
- **Połowa miesiąca** — sposób podziału miesiąca na dwie połowy jest umowny; zalecane jest trzymanie się granic tygodni zgodnie z poziomem poniżej
- **Tydzień** — miesiące nie dzielą się na równe tygodnie; wygodniej na tym poziomie operować na całych tygodniach według stałego cyklu (np. poniedziałek–niedziela), przypisując każdy tydzień do miesiąca, w którym leży jego większa część

Domyślne przedziały można dostosować do własnych potrzeb.

→ [Przykładowy plan](example-plans.md#planer-scale-free)

## Kluczowa zasada: przedziały się dzielą, nie przesuwają

W miarę upływu czasu przedziały nigdy nie są przemianowywane ani przestawiane. Zamiast tego — dzielą się. Gdy odległy przedział wystarczająco się przybliży, rozpada się na węższe przedziały, które teraz mieszczą się w jego obrębie. Zadanie przydzielone do „następnego kwartału" pozostaje tam, gdy kwartał się zbliża — a gdy nadchodzi moment szczegółowego planowania tego kwartału, przedział jest dzielony i zadanie umieszczane precyzyjniej.

Oznacza to, że system nigdy nie wymaga przebudowy od zera. Plany trwale budują się i uszczegóławiają z czasem, zamiast wygasać i być zastępowane.

## Dojrzewanie

Przedział uznawany jest za dojrzały do podziału, gdy do jego początku pozostało mniej niż połowa jego długości. Dla trzymiesięcznego kwartału oznacza to dojrzewanie mniej więcej sześć tygodni przed jego rozpoczęciem. Dojrzewanie to sygnał — nie zobowiązanie. Skłania do przyjrzenia się temu, co znajduje się w danym przedziale, i podjęcia decyzji, jak rozdzielić te plany między węższe interwały, na które się podzieli.

Decyzja o tym, kiedy i jak dokonać podziału, zawsze należy do użytkownika. Narzędzie wskazuje moment; użytkownik podejmuje decyzję.

## Wspólne planowanie

Struktura scale-free sprawdza się naturalnie przy planowaniu między dwiema lub więcej osobami. Wspólna tablica daje wszystkim wgląd w ten sam horyzont — od konkretnego krótkiego terminu po przybliżony długi. Ponieważ przedziały dzielą się stopniowo, zamiast resetować się okresowo, nie ma jednego wyznaczonego momentu, w którym wszyscy muszą siadać i planować od nowa — system sprzyja asynchronicznemu uzupełnianiu i uszczegóławianiu planów.

## Implementacja

To narzędzie nie zakłada żadnej konkretnej technologii. Można użyć tego, co najlepiej pasuje do własnego stylu pracy:

- Tablicy Trello z jedną listą na przedział
- Arkusza kalkulacyjnego z kolumnami lub sekcjami dla każdego interwału
- Fizycznej tablicy z opisanymi kolumnami
- Zwykłego dokumentu przeglądanego i aktualizowanego od czasu do czasu

Struktura jest metodą. Nośnik należy do użytkownika.

## Zgodność z UP

To narzędzie stosuje zasadę UP — odzwierciedla istniejącą presję, nie dodając własnej:

- Brak narzuconego rytmu — nie ma wymaganego harmonogramu planowania; użytkownik angażuje się, gdy przedział dojrzewa lub gdy sam uzna to za właściwe
- Brak kary za nieobecność — struktura pozostaje niezmieniona; powrót po przerwie nie wymaga przebudowy systemu
- Brak sztucznej pilności — dojrzewanie to delikatny sygnał oparty na upływie czasu, nie termin narzucony przez narzędzie
- Szczegółowość wynika z rzeczywistości — poziom ziarnistości wyznacza bliskość w czasie, nie schemat narzucony przez narzędzie
