# Planer tempa — narzędzie UP

Narzędzie do śledzenia czynności bez terminów — tylko z zadanym tempem.

## Do czego służy

Niektóre czynności są ważne, ale nigdy nie stają się pilne. Nauka języka, sport, granie w gry, czytanie dla przyjemności — wszystkie konkurują o ten sam ograniczony zasób: czas wolny. I im tego czasu jest mniej, tym bardziej warto go świadomie zagospodarować.

Jednocześnie każdy system, który zamienia przyjemność w obowiązek, działa przeciwko sobie. Planer tempa jest zaprojektowany tak, żeby utrzymywać świadomość tego, jak czas rozkłada się między różne czynności — bez zamieniania tej świadomości w presję.

## Jak to działa

Każdej czynności przypisywana jest planowana średnia — docelowa ilość czasu dziennie. Znacznik śledzi realizację względem planu, przesuwając się do przodu i do tyłu w kalendarzu.

Dzienne średnie wybierane są ze skwantowanego zestawu wartości, a nie wpisywane dowolnie. Domyślny zestaw to: 5, 7, 10, 15, 20, 30 minut. Podobnie jak przedziały częstości w Czynności powtarzalnych, chodzi o wyeliminowanie pozornej decyzji — to, czy danej czynności należy się 13 czy 14 minut dziennie, nie ma istotnego znaczenia, więc deliberowanie nad tym byłoby nic nie wnoszącym obciążeniem. Domyślne wartości można dostosować do własnych potrzeb.

Jeśli znacznik wskazuje dzisiejszy dzień, realizacja jest dokładnie zgodna z planem. Czas poświęcony na daną czynność przesuwa znacznik proporcjonalnie do przodu. Trzydzieści minut przy planowanych piętnastu minutach dziennie przesuwa znacznik o dwa dni do przodu. Jeśli znacznik wyprzedza dzisiaj, dana czynność ostatnio pochłaniała więcej niż swój udział czasu — naturalny sygnał, żeby dać teraz szansę innym. Jeśli znacznik opóźnia się w stosunku do dzisiaj, czynność była zaniedbywana.

W dniach, gdy nic się nie dzieje, nie trzeba niczego wpisywać. Znacznik po prostu zostaje tam, gdzie jest.

→ [Przykładowy plan](example-plans.md#planer-tempa)

## Czym znacznik nie jest

Znacznik nie jest terminem. Nie generuje poczucia winy. Spędzenie godziny na czymś planowanym po piętnaście minut dziennie jest w porządku — znacznik po prostu wysuwa się bardziej do przodu, a dana czynność naturalnie schodzi na dalszy plan na jakiś czas. System odzwierciedla decyzje; nie ocenia ich.

## Sprzęgło (leeway)

Z czasem różnica między planem a realizacją może urosnąć na tyle, że przestaje być użyteczna. Znacznik opóźniony o kilka tygodni wywołuje poczucie beznadziei — plan jest tak odległy, że podejmowanie prób wyrównania nie ma sensu. Znacznik wybiegający kilka tygodni do przodu albo prowadzi do paraliżu — trudno w ogóle zająć się daną czynnością — albo powoduje utratę orientacji, jak bardzo realizacja odbiega od planu.

Mechanizm sprzęgła stopniowo zmniejsza te różnice w regularnych odstępach czasu. Raz w tygodniu wszystkie odległości od teraźniejszości są proporcjonalnie redukowane — w referencyjnej implementacji o 1 dzień dla każdych 5 dni różnicy. Znacznik trzy tygodnie do przodu cofa się o cztery dni. Znacznik dwa tygodnie do tyłu przesuwa się do przodu o trzy dni.

Sprzęgło nie jest resetem. Nie wymazuje historii ani nie udaje, że różnica nie istniała. Stopniowo godzi plan z rzeczywistością, utrzymując znaczniki wystarczająco blisko teraźniejszości, żeby pozostały motywujące.

Tygodniowa korekta jest stosowana w odniesieniu do stałego dnia — w referencyjnej implementacji poniedziałku — ale można ją przeprowadzić dowolnego dnia.

## Implementacja

To narzędzie nie zakłada żadnej konkretnej technologii. Można użyć tego, co najlepiej pasuje do własnego stylu pracy:

- Tablicy Trello z jedną kartą na czynność, używając dat jako znaczników
- Arkusza kalkulacyjnego śledzącego daty i dzienne cele
- Fizycznego kalendarza z przesuwalnymi znacznikami
- Zwykłego dokumentu aktualizowanego ręcznie

Struktura jest metodą. Nośnik należy do użytkownika.
