# BI_NGO
1. O projekcie
Tytuł projektu: Sytuacja opuszczonych noworodków i dzieci w pieczy zastępczej w Polsce
Cel projektu:
Celem projektu jest analiza i wizualizacja danych dotyczących liczby opuszczonych noworodków w polskich szpitalach oraz dzieci przebywających w pieczy zastępczej, zarówno rodzinnej, jak i instytucjonalnej. Projekt ma na celu edukację społeczeństwa, podniesienie świadomości na temat skali problemu oraz wskazanie kluczowych obszarów wymagających reform i wsparcia.
Kontekst sytuacji: Każdego roku w Polsce kilkaset noworodków jest pozostawianych przez swoich biologicznych rodziców w szpitalach. Decyzje te wynikają z różnych przyczyn, w tym problemów ekonomicznych, trudnej sytuacji życiowej lub zdrowotnej rodziców. Ważnym elementem projektu jest unikanie stygmatyzacji, dlatego zamiast określeń "porzucenie" używa się bardziej neutralnego terminu "opuszczenie noworodka".
Opuszczone noworodki często trafiają do adopcji lub systemu pieczy zastępczej, który w Polsce dzieli się na dwa główne rodzaje:
•	Piecza rodzinna – dzieci trafiają do rodzin zastępczych, zarówno spokrewnionych, jak i niespokrewnionych. Jest to bardziej pożądana forma opieki, gdyż zapewnia stabilniejsze i bardziej domowe warunki wychowania.
•	Piecza instytucjonalna – dzieci są umieszczane w domach dziecka lub placówkach opiekuńczo-wychowawczych. Choć przepisy ograniczają przebywanie dzieci poniżej 10. roku życia w takich placówkach, brak rodzin zastępczych sprawia, że wiele najmłodszych dzieci nadal tam przebywa.
Piecza zastępcza odgrywa kluczową rolę w ochronie dzieci przed zaniedbaniem i zapewnieniu im możliwości rozwoju w bezpiecznym środowisku. Mimo to system boryka się z wieloma problemami, takimi jak:
•	brak wystarczającej liczby rodzin zastępczych, szczególnie zawodowych,
•	niski poziom wynagrodzeń dla rodzin zastępczych,
•	brak odpowiedniego wsparcia psychologicznego i systemowego dla dzieci i opiekunów,
•	wzrost liczby dzieci przebywających w pieczy instytucjonalnej mimo dążeń do jej ograniczenia.
Projekt skupi się na analizie trendów oraz przedstawieniu danych w formie wizualizacji w Power BI, co pozwoli na czytelne i przystępne przedstawienie skali problemu. W ramach projektu powstało sześć zakładek, każda poświęcona innemu aspektowi problematyki:
1.	Kluczowe wskaźniki
2.	Opuszczone noworodki
3.	Piecza zastępcza
4.	Piecza instytucjonalna
5.	Piecza rodzinna
6.	Adopcje
Znaczenie projektu:
Projekt jest pierwszym tego typu przedsięwzięciem realizowanym publicznie i w ramach wolontariatu dla Fundacji Gajusz zajmującej się problematyką dzieci opuszczonych i w pieczy zastępczej. Jego celem jest dostarczenie rzetelnych danych i analiz, które mogą posłużyć jako narzędzie do działań na rzecz poprawy sytuacji dzieci w Polsce. Praca ta ma nie tylko na celu przedstawienie aktualnej sytuacji, ale także wpłynięcie na rozwój przyszłych inicjatyw społecznych i systemowych.
Osobisty aspekt projektu:
Projekt ten jest dla mnie szczególnie ważny, ponieważ stanowi pierwsze publiczne przedsięwzięcie, które może mieć realny wpływ na poprawę sytuacji społecznej. Wykorzystując swoje umiejętności analizy danych i wizualizacji, mam nadzieję na wniesienie wartości do działań Fundacji oraz na podniesienie świadomości społecznej w tym ważnym obszarze.

2: Jakie dane zostały wykorzystane
Do realizacji projektu wykorzystano dane z oficjalnych źródeł, w tym:
•	Główny Urząd Statystyczny (GUS) – raporty i zestawienia roczne dotyczące liczby urodzeń, adopcji oraz dzieci pozostających w pieczy zastępczej.
•	Ministerstwo Zdrowia – dane dotyczące liczby noworodków pozostawionych w szpitalach. Liczba opuszczeń dzieci tuż po narodzinach zmienia się każdego roku. Ministerstwo Zdrowia gromadzi te dane, lecz nie są one ogólnie dostępne. Fundacja występuje o nie corocznie w ramach dostępu do informacji publicznej.
Struktura danych:
•	Zakładka "Kluczowe wskaźniki" – zestawienie najważniejszych informacji o liczbie dzieci w pieczy zastępczej, liczbie adopcji i noworodków pozostawionych w szpitalach.
•	"Opuszczone noworodki" – dane o liczbie noworodków pozostawionych w szpitalach w podziale na lata i województwa.
•	"Piecza zastępcza" – informacje o liczbie dzieci w pieczy zastępczej, z podziałem na pieczę rodzinną i instytucjonalną.
•	"Piecza instytucjonalna" – liczba dzieci przebywających w placówkach opiekuńczo-wychowawczych.
•	"Piecza rodzinna" – dane na temat rodzin zastępczych, liczby dzieci w ich opiece oraz struktura tych rodzin.
•	"Adopcje" – statystyki dotyczące liczby adopcji, w tym adopcji krajowych i zagranicznych.
Dane są przedstawione w formie tabel, wykresów oraz map, co pozwala na dogłębną analizę i interpretację wyników. Projekt pozwala na monitorowanie zmian w czasie oraz porównywanie sytuacji w poszczególnych regionach kraju.

Przykładowe metryki stworzone w języku DAX (Data Analysis Expressions):
•	Liczba_opuszczonych_noworodków = SUM('Noworodki'[Opuszczenia]) – suma liczby opuszczonych noworodków w danym okresie.
•	Średnia_roczna_adopcji = AVERAGE('Adopcje'[Liczba_adopcji]) – średnia roczna liczba adopcji.
•	%_opuszczonych_wg_województwa = DIVIDE(SUM('Noworodki'[Opuszczenia]), SUM('Noworodki'[Urodzenia]), 0) – procent opuszczonych noworodków w stosunku do liczby urodzeń w danym województwie.
Te metryki pozwalają na dynamiczne śledzenie i analizowanie danych, wspomagając identyfikację trendów i problemów systemowych.

3: W jaki sposób problem biznesowy został rozwiązany
Problem społeczny, jakim jest opuszczanie noworodków oraz potrzeba monitorowania sytuacji dzieci w pieczy zastępczej, został rozwiązany poprzez stworzenie kompleksowej analizy i wizualizacji danych. Dzięki połączeniu danych z GUS i Ministerstwa Zdrowia powstał interaktywny raport, który pozwala na:
1.	Identyfikację trendów – analiza danych na przestrzeni lat umożliwia wychwycenie wzrostów lub spadków liczby noworodków pozostawianych w szpitalach oraz dzieci przebywających w pieczy zastępczej.
2.	Regionalne porównania – dane zostały podzielone na województwa, co pozwala na zidentyfikowanie regionów o największych wyzwaniach oraz tych, które skutecznie radzą sobie z problemem.
3.	Wizualizację i transparentność – dane są przedstawione w formie wykresów, map i tabel, co ułatwia ich interpretację przez osoby niezwiązane na co dzień z analizą danych.
4.	Wsparcie dla działań społecznych i politycznych – raport dostarcza Fundacji oraz decydentom solidnych podstaw do prowadzenia kampanii edukacyjnych, tworzenia programów wsparcia oraz postulowania zmian w polityce społecznej.
Projekt nie tylko dostarcza aktualnych danych, ale również podkreśla kluczowe problemy systemowe, takie jak niewystarczająca liczba rodzin zastępczych, brak dostępnych ośrodków adopcyjnych i zróżnicowanie regionalne. Analiza umożliwia również monitorowanie skuteczności wprowadzanych zmian w kolejnych latach.

