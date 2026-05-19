##########
>white|orangered|left|14|30|hr Sekcja 3.2
### 3.2. Praktyki zarządzania ryzykiem
>white|orangered|left|24|30|hb Praktyki zarządzania ryzykiem

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Kluczowe informacje
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Ogólne zarządzanie ryzykiem dla sztucznej inteligencji ogólnego przeznaczenia obejmuje zestaw praktyk stosowanych do identyfikowania, oceny i ograniczania ryzyk wynikających ze sztucznej inteligencji ogólnego przeznaczenia. Obejmuje to testowanie i ewaluację na poziomie modelu (takie jak „red-teaming”), procesy organizacyjne ukierunkowujące decyzje dotyczące rozwoju i udostępnienia, warunkowe zabezpieczenia (takie jak zobowiązania „jeśli-wtedy”) oraz raportowanie incydentów.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kilku twórców AI opracowało Ramy Bezpieczeństwa Frontier AI. Ramy te zawierają informacje o ocenie ryzyka i określają środki warunkowe, takie jak ograniczenia dostępu, które firmy planują wdrożyć dla bardziej zdolnych modeli. Różnią się pod względem ryzyk, które obejmują, sposobu definiowania progów zdolności oraz tego, jakie działania są uruchamiane po osiągnięciu progów.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dowody na rzeczywistą skuteczność praktyk zarządzania ryzykiem w obszarze AI pozostają ograniczone. Brak raportowania incydentów i monitorowania utrudnia ocenę, jak dobrze obecne praktyki redukują ryzyko lub jak konsekwentnie są wdrażane.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Od czasu publikacji ostatniego Raportu (styczeń 2025) zarządzanie ryzykiem stało się bardziej uporządkowane dzięki nowym inicjatywom branżowym i w obszarze ładu korporacyjnego. Nowe instrumenty, takie jak Kodeks praktyk UE dla AI o zastosowaniu ogólnym, Ramy zarządzania bezpieczeństwem AI Chin 2.0 oraz G7. Proces raportowania z Hiroszimy, wraz z inicjatywami kierowanymi przez firmy, pokazują trend w kierunku bardziej ujednoliconych podejść do przejrzystości, oceny i raportowania incydentów.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dynamika rynku i tempo rozwoju AI stwarzają dodatkowe wyzwania. Ze względu na presję konkurencyjną firmy AI mogą stanąć przed dylematami między szybszym wprowadzaniem produktów na rynek a inwestowaniem w działania na rzecz ograniczania ryzyka. Wiele szkodliwych skutków związanych z AI jest również przenoszonych na otoczenie, a odpowiedzialność prawna za nie pozostaje niejasna, a procesy zarządzania mogą wolno dostosowywać się do zmian w krajobrazie AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Kluczowe wyzwania dla decydentów obejmują nadawanie priorytetu spośród różnorodnych ryzyk stwarzanych przez AI ogólnego przeznaczenia oraz wyjaśnienie, którzy aktorzy w całym łańcuchu wartości AI są najlepiej przygotowani do ograniczania tych ryzyk. Wyzwania te są potęgowane przez ograniczoną widoczność tego, jak ryzyka są w praktyce identyfikowane, oceniane i zarządzane, a także przez rozdrobnione udostępnianie informacji między deweloperami, wdrażającymi oraz dostawcami infrastruktury.
>oldlace|black||11|15|br      


Zarządzanie ryzykiem w obszarze AI obejmuje szereg praktyk, których celem jest identyfikacja, ocena oraz ograniczanie prawdopodobieństwa i dotkliwości ryzyk związanych z systemami AI. Praktyki te mogą być wdrażane przez twórców AI, wdrażających, ewaluatorów oraz regulatorów. Przykłady obejmują modelowanie zagrożeń, kategoryzację ryzyka, red-teaming, audytowanie oraz raportowanie incydentów. Ta sekcja opisuje aktualne praktyki zarządzania ryzykiem, nowe rozwinięcia oraz pozostałe ograniczenia.

Od początku 2025 roku opracowano kilka nowych międzynarodowych inicjatyw dotyczących zarządzania ryzykiem dla ogólnego sztucznego inteligencji, w tym ramy organizacyjnej przejrzystości i sprawozdawczości ryzyka, a także ramy regulacyjne i zarządzania.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Postać 3.4: Cztery komponenty zarządzania ryzykiem
>white|black||9|11|br Cztery kategorie metod zarządzania ryzykiem dla ogólnego sztucznego (AI) ryzyka: identyfikacja ryzyka; analiza i ocena ryzyka; łagodzenie ryzyka; oraz zarządzanie ryzykiem. Tworzą one iteracyjny i cykliczny proces. Zarządzanie ryzykiem, pokazane na środku, ułatwia powodzenie pozostałych komponentów. Źródło: International AI Safety Report 2026.


Pozostałe wyzwania obejmują ograniczoną standaryzację, co utrudnia zgodność i ocenę, a także ograniczone dowody dotyczące skuteczności w rzeczywistych warunkach. Ponadto konteksty instytucjonalne, kulturowe i polityczne różnią się na całym świecie, co oznacza, że podejścia do identyfikowania i zarządzania ryzykami, w tym do akceptowalnych progów ryzyka, mogą się różnić w poszczególnych regionach. Dyskusja w tej sekcji na temat podejść do zarządzania ryzykiem ma charakter opisowy: ma na celu poinformowanie podmiotów w ekosystemie AI o obecnych globalnych podejściach do zarządzania ryzykiem. O ile są dostępne, omawia się dowody dotyczące skuteczności i ograniczeń tych podejść, jednak rekomendacje polityczne wykraczają poza zakres niniejszego opracowania.

###@ Składniki zarządzania ryzykiem

Zarządzanie ryzykiem jest procesem iteracyjnym z praktykami i metodami obejmującymi cały cykl rozwoju i wdrażania AI, ale które współdziałają spójnie (‡969). Zarządzanie ryzykiem dla AI ogólnego przeznaczenia może obejmować role szerokiego grona podmiotów, w tym: naukowców ds. danych, inżynierów modeli, audytorów, ekspertów dziedzinowych, kierownictwa, użytkowników końcowych, społeczności dotkniętych skutkami, dostawców zewnętrznych, decydentów, rządów, organizacji normalizacyjnych oraz organizacji społeczeństwa obywatelskiego (‡970, ‡971, ‡972). Wiodące standardy zarządzania ryzykiem są często współdziałające, ale używają różnej terminologii do opisu elementów zarządzania ryzykiem (‡973, ‡974). Zwykle mają cztery powiązane ze sobą komponenty (Postać 3.4): identyfikowanie; analizowanie i ocenia-nie; łagodzenie; oraz zarządzanie ryzykiem (‡970, ‡973, ‡975, ‡976). Poniższe tabele przedstawiają przykładowe metody, techniki i narzędzia. Praktyki nadal ewoluują, więc tabele nie są wyczerpujące, a ich zastosowanie będzie się różnić w zależności od kontekstu.

###@ Identyfikacja ryzyka

Identyfikacja ryzyka to proces znajdowania, rozpoznawania i opisywania ryzyk. Kompleksowa identyfikacja ryzyka zazwyczaj obejmuje oceny sterowane zdolnościami, które testują, czy modele posiadają określone niebezpieczne zdolności (‡977), a także modelowanie ryzyka (‡978) i prognozowanie (‡715*), wykorzystywane do badania istniejących i pojawiających się ryzyk. Tabela 3.1 przedstawia różne przykłady praktyk identyfikacji ryzyka. Identyfikacja ryzyka korzysta również z zaangażowania odpowiednich ekspertów i społeczności w celu zrozumienia szerszego kontekstu, w jaki sposób ryzyka się ujawniają (‡979, ‡980). Mechanizmy takie jak programy nagród za znalezienie błędów mogą wspierać ten proces, zachęcając do identyfikowania wcześniej nieznanych podatności (‡981) (Tabela 3.1). Kluczowym celem identyfikacji ryzyka jest uwzględnienie zarówno dobrze znanych i dobrze rozumianych ryzyk, jak i potencjalnych przyszłych ryzyk, które pozostają niepewne lub słabo scharakteryzowane (‡982). Ma to szczególne znaczenie dla AI ogólnego przeznaczenia, gdzie wiele ryzyk może nie być jeszcze w pełni zrozumianych lub możliwych do zaobserwowania (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb programy bug bounty
  Programy nagród za błędy lub programy ujawniania podatności motywują do znajdowania i zgłaszania podatności w systemach AI. Kilku programistów wdrożyło programy nagród za błędy (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Konsultacja ekspercka
  Eksperci domenowi, użytkownicy i dotknięte społeczności dostarczają informacji na temat prawdopodobnych ryzyk. Pojawiają się wytyczne dotyczące partycypacyjnej i inkluzywnej sztucznej inteligencji (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Diagram ryby (Ishikawa)
  Diagramy rybich ości są dobrze ugruntowanymi narzędziami analizy przyczyn źródłowych, a badacze zaproponowali ich wykorzystanie do ustrukturyzowanej analizy incydentów związanych z ryzykiem w AI (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prognozowanie
  Prognozowanie to proces przewidywania przyszłych zdarzeń lub trendów na podstawie analizy danych z przeszłości i teraźniejszości. Jest wykorzystywane do porównywania względnego prawdopodobieństwa, na przykład, różnych wyników ekonomicznych wynikających z zaawansowanej sztucznej inteligencji (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Taksonomia ryzyka
  Taksonomie ryzyka są sposobem kategoryzowania i porządkowania ryzyk w wielu wymiarach. Istnieje kilka takich, które opisują ryzyka związane z AI ogólnego przeznaczenia (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Planowanie scenariuszy
  Planowanie scenariuszowe polega na opracowywaniu wiarygodnych przyszłych scenariuszy i analizowaniu tego, w jaki sposób materializują się ryzyka. Wykorzystuje się je do badania ryzyk i skutków modeli AI (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb modelowanie zagrożeń
  Modelowanie zagrożeń to proces identyfikowania zagrożeń i podatności dla systemu. Liczni deweloperzy AI podkreślają jego użycie w celu przewidywania potencjalnych scenariuszy nadużyć systemów AI (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.1: Przykłady identyfikacji ryzyka w ogólnym zarządzaniu ryzykiem dla sztucznej inteligencji ogólnego przeznaczenia
>white|black||9|11|br Przykładowe metody identyfikacji ryzyka związanego z AI ułożone alfabetycznie. Uwzględnione metody
są zaprojektowane w celu wspierania identyfikacji ryzyka dla wielu różnych typów ryzyka, w tym ryzyk wynikających ze złośliwego użycia, ryzyk wynikających z awarii oraz ryzyk systemowych. Biorąc pod uwagę wciąż wczesny charakter zarządzania ryzykiem dla ogólnego zastosowania sztucznej inteligencji, nie wszystkie metody będą odpowiednie dla każdego dewelopera lub wdrażającego system AI.


>white|orangered|left|14|15.5|bb Modelowanie zagrożeń i taksonomie ryzyka są istotnymi metodami identyfikacji ryzyka

Dwie znaczące metody identyfikowania ryzyk wynikających z ogólnego sztucznego intelektu (general-purpose AI) to modelowanie zagrożeń oraz taksonomie ryzyka. „International AI Safety Report 2026” (sprawozdanie dotyczące bezpieczeństwa AI na arenie międzynarodowej 2026) opisuje modelowanie zagrożeń jako ustrukturyzowany proces mapowania tego, w jaki sposób mogą się materializować ryzyka związane z AI, natomiast taksonomie ryzyka porządkują te ryzyka. Meta, na przykład, stosuje ćwiczenia z modelowania zagrożeń, aby antycypować możliwe scenariusze nadużyć swoich modeli AI (‡990), a Anthropic uwzględnia modelowanie zagrożeń jako część swojego ASL-3 Deployment Standard (‡991). Taksonomie ryzyka i hazardu AI, które zawierają kategorie ryzyka i przykłady, mogą równie dobrze stanowić punkt wyjścia do konceptualizowania, identyfikowania i precyzowania istotnych ryzyk związanych z ogólnym sztucznym intelektem w konkretnych domenach zastosowań (‡906, ‡988, ‡992, ‡993).

###@ Analiza ryzyka i ocena

Analiza ryzyka i ocena to proces określania poziomu ryzyka modelu lub systemu AI oraz porównywania go z ustalonymi kryteriami w celu oceny akceptowalności lub potrzeby zastosowania działań łagodzących (‡994, ‡995, ‡996, ‡997). Obejmuje on takie praktyki, jak pomiar wydajności modelu na benchmarkach (‡998) i ewaluacjach (‡176, ‡715), przeprowadzanie ćwiczeń typu red-teaming (‡999*), oceny wpływu (‡1000) oraz audyty (‡1001, ‡1002). Zobacz Tabela 3.2 w celu zapoznania się z przykładami ogólnego zastosowania analizy ryzyka i oceny dla AI. Metody te są zaprojektowane tak, aby wspierać analizę i ewaluację wielu różnych typów ryzyka jednocześnie.

Kluczowe cele analizy i oceny ryzyka obejmują przeprowadzanie ocen możliwości modelu oraz podatności (‡1003), wykorzystywanie solidnego modelowania ryzyka do informowania decyzji dotyczących progów ryzyka (‡1004, ‡1005) oraz zrozumienie, w jaki sposób systemy AI są wykorzystywane w praktyce, aby ocenić skutki społeczne na dalszych etapach (‡869, ‡904, ‡905, ‡1006). Procesy analizy i oceny ryzyka są często uznawane za bardziej skłonne do identyfikowania ryzyk, gdy uwzględniają niezależny przegląd (‡1001, ‡1007), korzystają z wiedzy specjalistycznej w wielu sektorach (‡1008) oraz obejmują zróżnicowane perspektywy z wielu dziedzin i dyscyplin, a także z perspektyw społeczności dotkniętych skutkami (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Audyty
  Audyty to formalne przeglądy działania i wpływu modeli AI oraz/ lub zgodności organizacji ze standardami, politykami i procedurami, przeprowadzane wewnętrznie lub przez podmiot zewnętrzny. Audytowanie AI to rozwijająca się dziedzina, a istnieje wiele narzędzi i praktyk do audytowania modeli AI oraz praktyk deweloperów modeli AI (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmarky
  Benchmarki są standaryzowane, często ilościowe testy lub metryki używane do oceny i porównywania wydajności systemów AI na stałym zestawie zadań zaprojektowanych tak, aby odzwierciedlać rzeczywiste zastosowanie (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Metoda łuku (Bowtie)
  Metoda muszki (bowtie) to dobrze znana metoda wizualizacji tego, gdzie można dodać zabezpieczenia, aby ograniczać zdarzenia generujące ryzyko. Umożliwia ona wyraźne rozróżnienie między proaktywnym a reaktywnym zarządzaniem ryzykiem (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb metoda Delphi
  Metoda Delphi to technika podejmowania decyzji grupowych, która wykorzystuje serię kwestionariuszy do gromadzenia uzgodnionych stanowisk od panelu ekspertów (‡1020, ‡1021). Była stosowana, aby pomóc w eksplorowaniu możliwych przyszłości z zaawansowaną sztuczną inteligencją (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Testowanie w warunkach rzeczywistych
  Testy w terenie oceniają wydajność i wpływ systemu AI w rzeczywistym, operacyjnym środowisku. Część badań podkreśla testy w terenie jako uzupełnienie oceny modelu przy ocenie rzeczywistych wyników i konsekwencji (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ocena wpływu
  Oceny wpływu oceniają potencjalne skutki technologii lub projektu. Może to obejmować ilościowe określanie, agregowanie i priorytetyzowanie skutków. Na przykład unijne rozporządzenie w sprawie AI (AI Act) wymaga, aby twórcy systemów AI wysokiego ryzyka przeprowadzali Oceny Wpływu na podstawowe prawa (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ocena modelu
  Oceny modeli obejmują procesy i testy służące do oceny oraz pomiaru wydajności modelu AI w danym zadaniu. Istnieje wiele ocen AI, aby ocenić różne możliwości i ryzyka, w tym dotyczące bezpieczeństwa, ochrony (security) oraz wpływu społecznego (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ocena ryzyka probabilistycznego
  Ocena ryzyka probabilistycznego to metodyka służąca do oceny ryzyk związanych ze złożonymi systemami lub procesami, która uwzględnia niepewność. Została zaadaptowana dla zaawansowanych systemów AI (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Testy typu red-teaming
  Red-teamowanie to ćwiczenie, w którym grupa osób lub zautomatyzowane systemy udają przeciwnika i atakują technologiczne systemy organizacji, aby zidentyfikować podatności. Liczne firmy z branży AI mają wewnętrzne praktyki dotyczące red-teamowania systemów AI (‡458, ‡1028). Red-teamowanie może być też prowadzone przez podmioty spoza firm. Zespoły te napotykają wyzwania, takie jak ograniczony dostęp, ale mogą również ujawnić wyraźne spostrzeżenia (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Macierze ryzyka
  Macierze ryzyka są narzędziem wizualnym, które pomaga w priorytetyzowaniu ryzyk w oparciu o prawdopodobieństwo wystąpienia i potencjalny wpływ (‡1027). Niektórzy deweloperzy AI uwzględniają podstawowe macierze ryzyka w swoich ramach Frontier AI Safety Frameworks (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb progi ryzyka / poziomy ryzyka
  Progi ryzyka lub poziomy są ilościowymi albo jakościowymi ograniczeniami, które rozróżniają ryzyka akceptowalne od nieakceptowalnych oraz uruchamiają określone działania zarządzania ryzykiem, gdy zostaną przekroczone. Dla AI ogólnego przeznaczenia są one wyznaczane na podstawie kombinacji możliwości, wpływu, mocy obliczeniowej, zasięgu i innych czynników (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tolerancja ryzyka
  Tolerancja ryzyka odnosi się do poziomu ryzyka, jaki organizacja jest gotowa zaakceptować. W przypadku AI tolerancje ryzyka są często ustalane w sposób niejawny poprzez polityki i praktyki firmy, podczas gdy niektóre reżimy regulacyjne wprost określają ryzyka nieakceptowalne i wiążą z nimi konsekwencje prawne (‡1032). Niektóre firmy opisują swoją tolerancję ryzyka w kategoriach marginalnego ryzyka nowego modelu; to znaczy w jakim stopniu model kontrfaktycznie zwiększa ryzyko ponad ryzyko już stwarzane przez istniejące modele lub inne technologie (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Studia przypadków bezpieczeństwa
  Sprawa bezpieczeństwa to ustrukturyzowany argument, wspierany dowodami, że system jest akceptowalnie bezpieczny do działania w określonym kontekście. Nowsza literatura (‡1037, ‡1038, ‡1039) bada sprawy bezpieczeństwa dla systemów AI na granicy możliwości oraz pewne Frontier AI Safety Frameworks na nie się powołują (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Analiza bezpieczeństwa systemu
  Analiza bezpieczeństwa systemu podkreśla zależności między komponentami i systemem, którego są częścią, aby przewidywać, w jaki sposób zagrożenia na poziomie systemu mogą wynikać z awarii komponentów lub procesów albo z oddziaływań między podsystemami, czynników ludzkich oraz warunków środowiskowych. Podejścia stosowane dla systemów AI w literaturze obejmują analizę procesów w ujęciu systemowo-teoretycznym (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.2: Analiza oceny ryzyka w ogólnym zarządzaniu ryzykiem AI do zastosowań ogólnych
>white|black||9|11|br Przykładowe metody analizy/oceny ryzyka związanego z AI, ułożone alfabetycznie. Ze względu na wczesny charakter ogólnego zarządzania ryzykiem w obszarze AI, nie wszystkie metody będą odpowiednie dla każdego twórcy lub wdrożeniowca AI.


>white|orangered|left|14|15.5|bb Typowe narzędzia analizy ryzyka obejmują benchmarki oraz ewaluacje modeli

Testy porównawcze (benchmarks) i oceny modeli są ustandaryzowanymi testami służącymi do oceny działania ogólnego systemu AI do zadań szczegółowych. Badacze opracowali szeroki zakres benchmarków i ocen, w tym zestawy trudnych pytań wielokrotnego wyboru, problemy z inżynierii oprogramowania oraz zadania związane z pracą w symulowanych środowiskach biurowych (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Oceny szkodliwych możliwości (‡715) są wykorzystywane do sprawdzania, czy ogólnego przeznaczenia model AI lub system posiada szczególnie niebezpieczną wiedzę lub umiejętności, takie jak zdolność do wspierania cyberataków (zob. §2.1.3. Cyberataki).

Wysoce brzemienne w skutkach decyzje podejmowane przez firmy i rządy dotyczące udostępniania modeli częściowo opierają się na tych ocenach (‡1050, ‡1051, ‡1052). Jednak benchmarki istotnie różnią się jakością i zakresem (‡998, ‡1003), a ocena ich wiarygodności może być trudna ze względu na liczne niedociągnięcia w praktykach benchmarkingu (‡902, ‡909, ‡1003, ‡1053*). Na przykład benchmarki mogą stać się „nasycone” – gdy wyniki wielu modeli zbliżają się do wyniku maksymalnego – co oznacza, że nie rozróżniają już w wyraźny sposób modeli. Modele są też coraz częściej zdolne do rozpoznawania niektórych zadań jako ewaluacje i do wykazywania odmiennych zachowań niż te, które wystąpiłyby na podobnych zadaniach w kontekstach wdrożeniowych, z powodu „świadomości sytuacyjnej” (zob. §2.2.2. Utrata kontroli). Wreszcie benchmarki i ewaluacje mają dobrze udokumentowane ograniczenia: w szczególności nie potrafią uchwycić ryzyk związanych z użyciem ogólnego AI w nowych dziedzinach i dla nowych zadań, ponieważ warunki testowe w różnym stopniu różnią się od rzeczywistego użycia (‡913) (zob. §1.2. Aktualne możliwości oraz §3.1. Wyzwania techniczne i instytucjonalne).

>white|orangered|left|14|15.5|bb Red teaming umożliwia przeprowadzanie bardziej ukierunkowanych na konkretne dziedziny ocen ryzyka

Inną powszechną metodą oceny ryzyka są ćwiczenia typu red-teaming. „Red team” to grupa oceniających, którym powierzono zadanie poszukiwania podatności, ograniczeń lub potencjału nadużyć. Ćwiczenia red-teaming mogą być specyficzne dla danej dziedziny i wykonywane przez ekspertów dziedzinowych albo mieć charakter otwarty, aby odkrywać nowe czynniki ryzyka. Na przykład red team może badać ataki „jailbreaking”, które omijają ograniczenia bezpieczeństwa modelu (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). W przeciwieństwie do benchmarków kluczową zaletą red-teaming jest to, że red teamy mogą dostosowywać swoje oceny do konkretnego testowanego systemu. Na przykład red teamy mogą projektować niestandardowe dane wejściowe, aby identyfikować zachowania w najgorszym przypadku, możliwości szkodliwego użycia oraz nieoczekiwane awarie. Jednak może to wymagać specjalnego dostępu do modeli i może nie ujawnić istotnych klas ryzyk (‡999, ‡1028).

Ważne jest to, że brak zidentyfikowanych ryzyk nie oznacza, iż te ryzyka są niskie: wcześniejsze prace pokazują, że błędy często wymykają się wykryciu, szczególnie gdy zespoły typu red team mają ograniczony dostęp lub zasoby (‡1060). Badania podważyły również, czy red-teaming może dostarczać wiarygodnych i możliwych do powtórzenia wyników (‡1061). Skład zespołu red team oraz instrukcje przekazane red-teamersom (‡1062), liczba rund ataku (‡1063) oraz dostęp modelu do narzędzi (‡1064, ‡1065) mogą istotnie wpływać na rezultaty, w tym na pokrytą powierzchnię ryzyka. Kompleksowe wytyczne dotyczące red-teamingu mają na celu sprostanie części z tych wyzwań (‡1066).

###@ Łagodzenie ryzyka

Łagodzenie ryzyka to proces priorytetyzowania, oceny oraz wdrażania mechanizmów kontrolnych i środków zaradczych w celu ograniczenia zidentyfikowanych ryzyk. Przykładami są mechanizmy kontroli dostępu (‡991), ciągłe monitorowanie (‡986) oraz zobowiązania typu if-then (‡700). Łagodzenie ryzyka rodzi kluczowe pytanie: jaki jest akceptowalny poziom ryzyka? Ostatnie ramy i polityki firmowe zaczęły formalizować kryteria „akceptacji ryzyka” (‡965, ‡1040). Jednak wyznaczanie odpowiednich progów pozostaje wyzwaniem, zwłaszcza dla ryzyk o szerokim wpływie społecznym (‡986, ‡1067). Obecnie nie istnieje żaden ustanowiony mechanizm służący do walidacji decyzji dotyczących akceptacji ryzyka podejmowanych przez deweloperów przed wydaniem (‡1005).

Metody ograniczania ryzyka opisane w Tabela 3.3 poniżej są elastyczne i mogą ograniczać różnorodne rodzaje ryzyka, w tym niektóre nieoczekiwane ryzyka. Tabela nie obejmuje technicznych metod ograniczania ryzyka, takich jak trening przeciwników, filtry treści oraz monitorowanie łańcucha rozumowania. Zagadnienia te są omówione w §3.3. Zabezpieczenia techniczne i monitorowanie, a także w całym Raporcie w akapitach „Mitigations” dla każdego ryzyka w §2. Risks.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Zasady akceptowalnego użytkowania
  Polityka akceptowalnego użycia to zbiór zasad i wytycznych dotyczących odpowiedzialnego, etycznego i zgodnego z prawem korzystania z modeli AI. Jest powszechne, że twórcy systemów AI publikują polityki akceptowalnego użycia, a także polityki zabronionego użycia, wraz z nowymi wydaniami modeli (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kontrola dostępu/ weryfikacja użytkownika
  Kontrole dostępu obejmują stosowanie zasad i reguł w celu ograniczania dostępu do modeli AI, danych i systemów w oparciu o role użytkowników, atrybuty oraz inne warunki, aby zapobiegać nieupoważnionemu wykorzystaniu, manipulacji lub naruszeniom poufności danych. Firmy z branży AI często wyłączają konta, które wykazują aktywność związaną z przestępczością (‡486), oraz wdrażają weryfikację użytkowników i procedury Know-Your-Customer, aby zapewnić, że modele są używane wyłącznie przez zaufane podmioty (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Specyfikacja zachowania/modelu
  Specyfikacja zachowania AI to dokument, który określa, jak model AI powinien się zachowywać w różnych sytuacjach. Służy jako plan dla dopasowania AI i bezpieczeństwa, kierując rozwojem modelu, treningiem, ewaluacją oraz jego wyjściami. Kilka firm z branży AI korzysta z dokumentów specyfikacji modelu i udostępnia przynajmniej ich części publicznie (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ciągłe monitorowanie
  Ciągły monitoring to trwający, zautomatyzowany proces obserwowania, analizowania i kontrolowania systemów AI w użyciu, śledzenia ich wydajności oraz ograniczania ich zachowania, aby zapewnić niezawodność, skuteczność i bezpieczeństwo. Dostępnych jest wiele narzędzi do ciągłego monitorowania (‡1073*) oraz technik wspierających
Obserwowalność AI (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Defense-in-depth
  Obrona wielowarstwowa (defence-in-depth) to idea, zgodnie z którą można wdrożyć wiele niezależnych i zachodzących na siebie warstw obrony, tak aby w przypadku gdy jedna zawiedzie, pozostałe nadal były skuteczne (‡1075, ‡1076). Wiele Ram Bezpieczeństwa dla Sztucznej Inteligencji na Granicy Systemu odnosi się do niej (np. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoring ekosystemu
  To proces monitorowania szerszego ekosystemu AI, w tym śledzenia zasobów obliczeniowych i sprzętu, pochodzenia modeli, pochodzenia danych oraz wzorców użytkowania. Literatura badawcza omawia takie monitorowanie w odniesieniu do ryzyk związanych z ogólnego przeznaczenia AI (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Zobowiązania warunkowe typu if-then
  Zobowiązania warunkowe typu if-then stanowią zbiór technicznych i organizacyjnych protokołów oraz zobowiązań służących do zarządzania ryzykiem w miarę wzrostu możliwości modeli AI. Kilku twórców AI stosuje tego rodzaju zobowiązania jako część swoich Ram Bezpieczeństwa Frontier AI (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Czerwone linie lub zakazy
  Czerwone linie to konkretne granice wyrażone jako możliwości, wpływ lub rodzaje zastosowań. Pojęcie to występuje w publicznych wystąpieniach i inicjatywach, a także w zakazach regulacyjnych (‡1079, ‡1080, ‡1081). Literatura wskazuje również ograniczenia podejść opartych na czerwonych liniach, w tym trudności związane z osiągnięciem konsensusu i egzekwowalnością.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie wydania i wdrożenia
  Strategie wydania i wdrożenia dla ogólnego przeznaczenia AI mogą obejmować użycie stopniowych wydań lub dostępu do API, aby zapewnić dostępność większej liczby opcji ograniczania ryzyka w przypadku nadużyć lub nieoczekiwanej szkody (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.3: Łagodzenie ryzyka w ogólnym zarządzaniu ryzykiem dla AI o ogólnym przeznaczeniu
>white|black||9|11|br Przykładowe metody łagodzenia ryzyka w AI wymienione alfabetycznie. Uwzględnione metody są zaprojektowane tak, aby równocześnie wspierać łagodzenie ryzyka dla wielu różnych typów ryzyka, w tym ryzyk wynikających ze złośliwego użycia, ryzyk wynikających z nieprawidłowego działania oraz ryzyk systemowych. Ze względu na wczesny, początkowy charakter zarządzania ryzykiem w przypadku ogólnego zastosowania AI nie wszystkie metody będą odpowiednie dla każdego dewelopera ani wdrożeniowca AI.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Postać 3.5: Ilustracja podejścia obrony w głąb za pomocą „diagramu szwajcarskiego sera”
>white|black||9|11|br Wiele warstw obrony może zrekompensować wady w poszczególnych warstwach. Obecne techniki zarządzania ryzykiem dla AI mają wady, ale ich nakładanie może zapewnić znacznie silniejszą ochronę przed ryzykami. Źródło: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Strategie obrony wielowarstwowej i zwolnienia są ważnymi narzędziami łagodzenia ryzyka

Model „obrony w głąb” może wspierać ogólne zarządzanie ryzykiem dla AI. W tym kontekście „obrona w głąb” odnosi się do połączenia środków technicznych, organizacyjnych i społecznych stosowanych na różnych etapach rozwoju i wdrożenia (Rysunek 3.5). Oznacza to tworzenie warstw niezależnych zabezpieczeń, tak aby w razie awarii jednej warstwy inne warstwy nadal mogły zapobiegać szkodom. Często przytaczanym przykładem modelu „obrony w głąb” jest zestaw środków prewencyjnych wdrażanych w celu zapobiegania chorobom zakaźnym. Szczepienia, maseczki i mycie rąk, między innymi, mogą znacząco zmniejszyć ryzyko zakażenia w połączeniu, mimo że żadna z tych metod nie jest w pojedynkę w 100% skuteczna (‡1083*). Dla ogólnego AI „obrona w głąb” obejmuje mechanizmy kontroli, które nie znajdują się same w modelu AI, lecz w szerszym ekosystemie. Obejmuje to (na przykład) mechanizmy kontroli dotyczące materiałów potrzebnych do przeprowadzenia biologicznego ataku, takich jak odczynniki (‡1084, ‡1085). Jednak środki „obrony w głąb” w pierwszej kolejności dotyczą ryzyk związanych z wypadkami, wadliwym działaniem i złośliwym użyciem oraz mogą odgrywać mniejszą rolę w zarządzaniu ryzykami systemowymi (zob. §3.5. Budowanie odporności społecznej).

Strategia wydania i wdrożenia w firmie jest ważnym elementem ograniczania ryzyka. Decyzje dotyczące tego, w jaki sposób modele są udostępniane użytkownikom, mogą w znacznym stopniu wpływać na poziom narażenia na ryzyko (‡1082). Różne opcje wydania i wdrożenia obejmują stopniowe udostępnianie do ograniczonych grup użytkowników, dostęp za pośrednictwem kontrolowanych usług online (takich jak API) oraz wykorzystanie umów licencyjnych i polityk dotyczących dozwolonego użytku, które prawnie zabraniają niektórych szkodliwych zastosowań (‡176, ‡1086, ‡1087). §3.4. Modele o otwartych wagach omawia bardziej szczegółowo, w jaki sposób udostępnianie wag modelu wpływa na ryzyka.

###@ Zarządzanie ryzykiem

Nadzór nad ryzykiem to proces, w ramach którego oceny, decyzje i działania w zakresie zarządzania ryzykiem są powiązane ze strategią i celami organizacji lub innego podmiotu (‡1088, ‡1089). Tabela 3.4 przedstawia przegląd typowych technik nadzoru nad ryzykiem. Jak pokazano na Postać 3.4, nadzór nad ryzykiem można rozumieć jako trzon zarządzania ryzykiem, ponieważ ułatwia on skuteczne funkcjonowanie pozostałych elementów zarządzania ryzykiem. Zapewnia on odpowiedzialność, przejrzystość i jasność, które wspierają podejmowanie świadomych decyzji w zakresie zarządzania ryzykiem. Nadzór nad ryzykiem może obejmować praktyki takie jak raportowanie incydentów (‡1090), przydzielanie odpowiedzialności za ryzyko (‡965) oraz ochrona sygnalistów (‡1091). Szerzej, nadzór nad ryzykiem może obejmować wytyczne, ramy, ustawodawstwo, regulacje, krajowe i międzynarodowe standardy, a także inicjatywy szkoleniowe i edukacyjne. Kluczowym celem nadzoru nad ryzykiem jest ustanowienie polityk organizacyjnych i mechanizmów, które wyjaśniają, w jaki sposób obowiązki związane z zarządzaniem ryzykiem są rozdzielane w obrębie organizacji lub innego podmiotu, aby wspierać odpowiedni nadzór i rozliczalność (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentacja
  Praktyki dokumentacyjne pomagają śledzić kluczowe informacje o systemach AI, takie jak dane treningowe, decyzje projektowe, zamierzone zastosowania, ograniczenia i ryzyka. „Karty modeli” i „karty systemów”, które zawierają informacje o tym, jak wytrenowano i oceniono model lub system AI, są przykładami istotnych dobrych praktyk w zakresie dokumentowania AI (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Raportowanie incydentów
  Raportowanie incydentów to proces systematycznego dokumentowania i udostępniania przypadków, w których rozwijanie lub wdrażanie AI spowodowało bezpośrednie lub pośrednie szkody. Istnieje kilka platform, które ułatwiają raportowanie incydentów dla AI (‡1096, ‡1097), oraz frameworki ułatwiające skuteczniejsze raportowanie incydentów związanych z AI (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ramy zarządzania ryzykiem
  Ramy zarządzania ryzykiem są planami organizacyjnymi służącymi do ograniczania luk w zakresie pokrycia ryzyka, koordynowania różnych działań w ramach zarządzania ryzykiem oraz wdrażania mechanizmów kontroli i równowagi. Ramy dotyczące ogólnego przeznaczenia AI (‡986, ‡1098) często odwołują się do innych środków wymienionych w tej sekcji.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rejestr ryzyk
  Rejestr ryzyk to repozytorium różnych ryzyk, ich priorytetyzacji, właścicieli oraz planów łagodzenia skutków. Są one stosunkowo powszechne w wielu branżach, w tym w cyberbezpieczeństwie (‡1099), i czasami są wykorzystywane do spełnienia wymagań zgodności regulacyjnej.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Przydział odpowiedzialności za ryzyko
  Przydział ról i odpowiedzialności za zarządzanie ryzykiem w organizacji może uporządkować wewnętrzny nadzór nad podejmowaniem decyzji (‡1002, ‡1093). Takie ustalenia odzwierciedlają niektóre ramy zarządzania, w tym unijny Kodeks praktyk AI o ogólnym przeznaczeniu (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Raporty przejrzystości
  Raporty przejrzystości opisują praktyki zarządzania ryzykiem firmy AI poprzez publiczne ujawnianie określonych informacji lub poprzez udostępnianie dokumentacji organizacjom branżowym albo organom rządowym. Na przykład liczne firmy AI składają raporty przejrzystości Hiroshima AI Process (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ochrona sygnalistów
  Ponieważ duża część rozwoju AI odbywa się za zamkniętymi drzwiami, niektóre ramy zarządzania obejmują ochronę sygnalistów, aby umożliwić ujawnianie potencjalnych zagrożeń właściwym organom (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.4: Zarządzanie ryzykiem w zakresie ogólnych AI w zarządzaniu ryzykiem systemów do zastosowań ogólnych
>white|black||9|11|br Przykładowe metody zarządzania ryzykiem w AI wymieniono alfabetycznie. Uwzględnione metody mają na celu wspieranie zarządzania ryzykiem dla wielu różnych typów ryzyka jednocześnie, w tym ryzyka wynikającego ze złośliwego wykorzystania, ryzyka związanego z awariami oraz ryzyka systemowego. Biorąc pod uwagę wczesny (nienastawiony jeszcze) charakter zarządzania ryzykiem w przypadku ogólnego AI, nie wszystkie metody będą odpowiednie dla każdego twórcy lub wdrożeniowca AI.


>white|orangered|left|14|15.5|bb Dokumentacja i przejrzystość są elementami zarządzania ryzykiem

Mechanizmy dokumentowania oraz przejrzystości instytucjonalnej, wraz z praktykami udostępniania informacji, ułatwiają zewnętrzną kontrolę i wspierają działania służące zarządzaniu ryzykami związanymi z ogólnodostępną sztuczną inteligencją (‡1101, ‡1102). Stało się powszechną praktyką publikowanie wyników testów przed wdrożeniem w postaci „model card” lub „system card”, wraz z podstawowymi szczegółami dotyczącymi modelu lub systemu, w tym tego, jak był trenowany, oraz jakie są jego potencjalne ograniczenia (‡1094, ‡1095). Niektórzy deweloperzy publikują również raporty przejrzystości zawierające bardziej ogólne informacje o stosowanych przez nich praktykach zarządzania ryzykiem (‡1103). Inne elementy dokumentacji i przejrzystości obejmują monitorowanie i raportowanie incydentów (‡176, ‡1083*, ‡1103) oraz udostępnianie informacji, które mogą być ułatwiane przez podmioty trzecie, takie jak Frontier Model Forum. Niektóre ramy regulacyjne, takie jak AI Act w UE lub California’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), w niektórych przypadkach nakładają obowiązek udostępniania informacji na temat ryzyk związanych z ogólnodostępną sztuczną inteligencją.

>white|orangered|left|14|15.5|bb Zaangażowanie kierownictwa i systemy motywacyjne kształtują praktyki zarządzania ryzykiem

Kultura organizacyjna, struktura przywództwa i systemy motywacyjne wpływają na działania związane z zarządzaniem ryzykiem na różne sposoby (‡1105). Zaangażowanie kierownictwa i struktury motywacyjne często są istotne dla tego, w jaki sposób polityki zarządzania ryzykiem działają w praktyce. Niektórzy deweloperzy mają wewnętrzne panele decyzyjne, które rozważają, jak bezpiecznie i odpowiedzialnie projektować, rozwijać oraz przeglądać nowe systemy AI. Organy nadzorcze i komitety doradcze, fundusze powiernicze lub rady ds. etyki AI mogą również służyć jako mechanizmy udzielania wskazówek w obszarze zarządzania ryzykiem oraz zapewniania nadzoru organizacyjnego (‡1092*, ‡1106, ‡1107, ‡1108). Naukowcy twierdzili, że trudności wynikające z dobrowolnego samoregulowania oznaczają, iż audyt zewnętrzny, weryfikacja i standaryzacja mogłyby pomóc wzmocnić ogólne zarządzanie ryzykiem dla AI ogólnego przeznaczenia (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Ramy zarządzania ryzykiem w organizacji, przejrzystości oraz raportowania ryzyka

Kilka nowych inicjatyw koncentruje się na procesach zarządzania ryzykiem, dokumentacji i przejrzystości. W obecnej formie unijny Kodeks postępowania dla sztucznej inteligencji ogólnego przeznaczenia pełni funkcję dobrowolnych ram służących wskazywaniu praktyk dotyczących przejrzystości, praw autorskich oraz bezpieczeństwa i ochrony, aby wspierać zgodność z postanowieniami Aktu w sprawie AI Unii Europejskiej dotyczącymi sztucznej inteligencji ogólnego przeznaczenia (‡965). Od grudnia 2025 r. ponad dwadzieścia firm† podpisało. Ramy sprawozdawcze G7 Hiroshima AI Process (HAIP) (‡1100) są pierwszym międzynarodowym zestawem ram dla dobrowolnego publicznego raportowania praktyk organizacyjnego zarządzania ryzykiem dla zaawansowanych systemów AI. Co najmniej 20 deweloperów opublikowało publiczne raporty przejrzystości obejmujące identyfikację ryzyka, metryki oceny, strategie łagodzenia ryzyka oraz procesy dotyczące bezpieczeństwa danych.

Twórcy AI przyjęli dobrowolne zobowiązania dotyczące przejrzystości. W Chinach zobowiązania złożone przez 17 chińskich firm AI, skoordynowane przez AI Industry Alliance of China, zostały opublikowane w grudniu 2024 (‡1113) i zaktualizowane w 2025 (‡1114). Podczas majowego AI Seoul Summit w 2024 roku w Korei Południowej 16 twórców AI z wielu krajów podpisało dobrowolne zobowiązania, aby publikować Frontier AI Safety Frameworks dla swoich najbardziej zdolnych modeli i systemów oraz aby wdrażać praktyki zarządzania ryzykiem w całym cyklu opracowywania i wdrażania modeli (‡1052).

    Notatka † -- Sygnatariusze na dzień grudnia 2025 obejmują: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing oraz WRITER.

>white|orangered|left|14|15.5|bb Frontierowe ramy Bezpieczeństwa AI stały się znaczącym podejściem organizacyjnym do zarządzania ryzykiem związanym ze sztuczną inteligencją

Od 2023 roku kilku czołowych programistów AI dobrowolnie publikuje dokumenty opisujące, w jaki sposób planują identyfikować i reagować na poważne ryzyka wynikające z ich najbardziej zaawansowanych systemów. Te Ramy Bezpieczeństwa AI „Frontier” opisują, jak programista AI planuje oceniać, monitorować i kontrolować swoje najbardziej zaawansowane modele i systemy przed wdrożeniem i w jego trakcie. Ramy te mają wiele podobieństw, ale różnią się w kluczowych aspektach (‡1115, ‡1116). Większość koncentruje się na ryzykach związanych z zagrożeniami chemicznymi, biologicznymi, radiologicznymi i nuklearnymi (CBRN), zaawansowanymi możliwościami cybernetycznymi oraz zaawansowanym, autonomicznym zachowaniem (‡1115, ‡1117). Mniejszość ram uwzględnia dodatkowe domeny ryzyka, takie jak niezgodna z prawem dyskryminacja na masową skalę oraz wykorzystywanie seksualne dzieci.

Kilku programistów zaktualizowało swoje frameworki w 2025, dodając nowe sekcje dotyczące szkodliwej manipulacji, ryzyka niezgodności oraz autonomicznej replikacji i adaptacji (‡1078, ‡1118). Chociaż wiele frameworków opisuje podobne podejścia do zarządzania ryzykiem – w tym modelowanie zagrożeń, red-teaming i oceny niebezpiecznych możliwości – różnią się one w definicjach poziomów ryzyka i progów, częstotliwości ewaluacji, buforach między ewaluacjami a progami oraz w stopniu kompletności swoich zobowiązań dotyczących ograniczania ryzyka (na przykład czy obejmują one usuwanie wag modelu, czy tylko wstrzymanie prac) (‡1115, ‡1119). Aby uzyskać więcej informacji, zobacz Tabela 3.5.

>white|orangered|left|14|15.5|bb Wiele działań w ramach Frontier AI Safety opiera się na zobowiązaniach typu jeśli-wtedy

Kluczową częścią Ram Bezpieczeństwa Frontier AI są „zobowiązania if-then”. Są to warunkowe protokoły, które uruchamiają określone reakcje, gdy modele i systemy AI osiągną zdefiniowane progowe poziomy zdolności (‡1120). Na przykład zobowiązanie if-then może stanowić, że jeśli stwierdzono, iż model ma zdolność do znaczącego wspomagania nowicjuszy w tworzeniu i wdrażaniu broni CBRN, to deweloper wdroży ulepszone środki bezpieczeństwa, kontrole wdrożenia oraz monitorowanie w czasie rzeczywistym (‡991*).

W 2025 kilku twórców AI ogłosiło, że nowe modele wyzwoliły wczesne alarmy ostrzegawcze lub że nie mogli wykluczyć możliwości, iż dalsza ocena wykaże, że modele przekroczyły progi zdolności. Skłoniło ich to do zastosowania podwyższonych zabezpieczeń jako środka ostrożności (‡7, ‡33, ‡1121*). Ramy Bezpieczeństwa Frontier AI Frameworks zazwyczaj wymagają wstępnej oceny zdolności przed działaniami ograniczającymi ryzyko, a także analizy ryzyka rezydualnego lub uzasadnienia bezpieczeństwa, często opartego na red-teaming, po wdrożeniu takich działań. Zobacz Tabela 3.5, aby uzyskać szczegółowe informacje.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Ramy gotowości 2 (‡1078*)
  Zidentyfikowane ryzyka:
1. Zdolności biologiczne i chemiczne
2. Możliwości w zakresie cyberbezpieczeństwa
3. Możliwości samodoskonalenia sztucznej inteligencji
  Poziomy ryzyka lub równoważne oraz powiązane zabezpieczenia:
- Wysoki: Może wzmacniać istniejące ścieżki prowadzące do poważnej szkody (wymaga kontroli bezpieczeństwa i zabezpieczeń)
- Krytyczne: Mogłoby wprowadzić bezprecedensowo nowe ścieżki prowadzące do poważnej szkody (Wstrzymać dalszy rozwój do czasu, aż określone zabezpieczenia oraz standardy kontroli bezpieczeństwa osiągną poziom Krytyczny)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Polityka Odpowiedzialnego Skalowania 2.2 (‡991*)
  Zidentyfikowane ryzyka:
1. Bronie CBRN
2. Autonomiczne badania i rozwój sztucznej inteligencji (AI R&D)
3. Operacje cybernetyczne (w ocenie)
  Poziomy ryzyka lub równoważne oraz powiązane środki zabezpieczające:
  Poziomy Bezpieczeństwa AI (ASL)
- ASL-1: Brak istotnego katastrofalnego ryzyka
- ASL-2: Wczesne oznaki niebezpiecznych możliwości (Modele muszą spełniać standardy wdrożenia i bezpieczeństwa ASL-2)
- ASL-3: Znacząco zwiększone ryzyko katastrofalnego niewłaściwego użycia (Modele muszą spełniać standardy wdrożenia i/lub bezpieczeństwa ASL-3)
- ASL-4+: Przyszłe klasyfikacje (jeszcze nieokreślone)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Ramy Bezpieczeństwa dla Frontiera 3.0 (‡1040*)
  Zidentyfikowane ryzyka:
1. Nadużycie
    a. CBRN
    b. Cyber
    c. Szkodliwa manipulacja
2. Badania i rozwój w uczeniu maszynowym
3. Niedopasowanie/ rozumowanie instrumentalne
  Poziomy ryzyka lub odpowiedniki oraz powiązane zabezpieczenia:
  Poziomy Krytycznych Zdolności
    Poziomy zdolności, przy których, przy braku działań łagodzących (procedury bezpieczeństwa dla wdrożeń oraz środki łagodzące bezpieczeństwo zgodne z poziomami bezpieczeństwa RAND 2, 3 lub 4 (‡1122)), modele lub systemy AI mogą stwarzać podwyższone ryzyko poważnej szkody. Poziomy zdolności obejmują „wczesną ocenę ostrzegawczą”, z określonymi „progami alarmowania”.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Framework AI Frontier 1.1 (‡990*)
  Zidentyfikowane ryzyka:
1. Cyberbezpieczeństwo
2. Ryzyko chemiczne i biologiczne
  Poziomy ryzyka lub równoważne oraz powiązane środki zabezpieczające:
  Poziomy progów ryzyka
- Umiarkowane (wydanie z odpowiednimi środkami bezpieczeństwa i działaniami łagodzącymi)
- igh (nie zwalniaj)
- Krytyczne (zatrzymaj rozwój)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Ramy Bezpieczeństwa Modelu Frontier (‡1123*)
  Zidentyfikowane ryzyka:
1. Rozprzestrzenianie broni CBRN
2. Złośliwe działania w cyberprzestrzeni
3. Zautomatyzowane badania i rozwój AI
  Poziomy ryzyka lub równoważne i powiązane zabezpieczenia:
  Krytyczne progi zdolności
    Możliwości modelu, które potencjalnie mogą spowodować znaczne szkody dla społeczeństwa w przypadku niewłaściwego użycia. (Jeśli progi zostaną spełnione lub przekroczone, model nie zostanie udostępniony publicznie bez odpowiednich środków ograniczania ryzyka)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Framework zarządzania w ramach Frontier (‡1124*)
  Zidentyfikowane ryzyka:
1. Bronie CBRN
2. Złośliwe działania w cyberprzestrzeni
3. Zaawansowana autonomia (w tym badania i rozwój AI)
  Poziomy ryzyka lub równoważne i powiązane zabezpieczenia:
  Poziomy ryzyka
- Niski lub Średni (wdrożenie dozwolone zgodnie z wymaganiami Programu Odpowiedzialnej AI)
- Wysokie lub Krytyczne (Dalszy przegląd i środki zaradcze
wymagane)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Ocena ryzyka Frontier AI (‡1029*)
  Zidentyfikowane ryzyka:
1. Cyberprzestępstwo
2. CBRN
3. Perswazja i manipulacja
4. Nielegalna dyskryminacja na skalę masową
  Poziomy ryzyka lub równoważne oraz powiązane zabezpieczenia:
  Progi ryzyka - wyniki ryzyka modelu (MR)
- MR1 lub MR2 (Wyniki oceny są dokumentowane przez zespoły inżynierskie)
- MR3 (Środki mitygacji ryzyka oraz wyniki oceny są dokumentowane przez zespoły inżynierskie i okresowo przeglądane)
- MR4 (Należy przeprowadzić szczegółową ocenę ryzyka i wymagane jest zatwierdzenie przez kierownika jednostki biznesowej)
- MR5 (Szczegółowa ocena ryzyka powinna zostać przeprowadzona i zatwierdzona przez niezależny komitet, np. komitet ds. etyki AI firmy NVIDIA)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Secure AI Frontier Model Framework (‡1125*)
  Zidentyfikowane ryzyka:
1. Złośliwe wykorzystanie (np. złośliwe oprogramowanie, wykorzystywanie seksualne dzieci)
2. Szkoda w zwykłym, niemalicyjnym użyciu, np. wyniki prowadzące do nielegalnej dyskryminacji lub generowania niebezpiecznego kodu
  Poziomy ryzyka lub równoważne oraz powiązane zabezpieczenia:
  Prawdopodobieństwo i dotkliwość szkody w kontekście
- Niski
- Średni
- Wysoki
- Bardzo wysoki
    (Założono środki zarządzania ryzykiem i kontrole bezpieczeństwa dla wszystkich systemów i procesów; dodatkowe środki zaradcze należy dostosować do systemu AI i danego przypadku użycia, w którym model jest wdrażany)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Polityka gotowości AGI (‡1127*)
  Zidentyfikowane ryzyka:
1. Cyberprzestępstwo
2. Zautomatyzowane badania i rozwój AI
3. Autonomiczna replikacja i adaptacja
4. Pomoc w zakresie broni biologicznej
  Poziomy ryzyka lub równoważne oraz powiązane zabezpieczenia:
  Krytyczne progi zdolności
    Ilościowe progi na benchmarkach możliwości (Jeśli zostaną przekroczone, przeprowadzić niebezpieczne oceny możliwości, środki bezpieczeństwa informacji oraz mitygacje wdrożeniowe lub wstrzymać rozwój)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Polityka gotowości AGI Magic: AGI (‡1127*)
  Zidentyfikowane ryzyka:
1. Cyberprzestępstwo
2. Zautomatyzowane badania i rozwój AI
3. Autonomiczne replikowanie i adaptacja
4. Pomoc w zakresie broni biologicznej
  Poziomy ryzyka lub równoważne oraz powiązane zabezpieczenia:
  Krytyczne progi zdolności
    Liczbowe progi na benchmarkach zdolności (Jeśli zostaną przekroczone, przeprowadź niebezpieczne oceny zdolności, środki bezpieczeństwa informacji i ograniczenia wdrożeniowe lub wstrzymaj rozwój)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: Ramy Bezpieczeństwa AI (‡1128*)
  Zidentyfikowane ryzyka:
1. Utrata kontroli
2. Nadużycie (np. biochemiczna broń biologiczna
  Poziomy ryzyka lub równoważne oraz powiązane zabezpieczenia:
  Poziomy ryzyka
- Niskie ryzyko (Wdrażaj systemy AI, ale wykonuj późniejsze monitorowanie, aby zarządzać ryzykiem)
- Zidentyfikowane ryzyko (Albo udostępnianie systemów AI Open wyłącznie upoważnionym użytkownikom w celu ograniczenia ryzyka, albo wstrzymanie wdrożenia do czasu podjęcia dodatkowych środków bezpieczeństwa, w zależności od przypadku użycia)
- Wysokie ryzyko (Nie wdrażaj systemów AI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Ramowy system Bezpieczeństwa AI dla Frontiru (‡1129*)
  Zidentyfikowane ryzyka:
1. Zagrożenia biologiczne
2. Offensywne cyberbezpieczeństwo
3. Autonomiczna praca i zaawansowana manipulacja
  Poziomy ryzyka lub równoważne i powiązane środki zabezpieczające:
  Poziomy ryzyka
- Poziom 1 (Podstawowe zabezpieczenia minimalizujące ryzyko i umożliwiające potencjalne udostępnienie jako oprogramowanie open source)
- Poziom 2 (monitorowanie w czasie rzeczywistym, filtrowanie promptów, wykrywanie anomalii behawioralnych, kontrole dostępu, red-teaming i symulacje przeciwnika)
- Poziom 3 (Zaawansowane zabezpieczenia obejmujące red- teaming, etapowe wdrożenia, testy odporności na ataki, szyfrowanie, wielostronną kontrolę dostępu i architekturę typu zero-trust)
- Poziom 4 (maksymalne procedury bezpieczeństwa dla modeli o wysokim ryzyku i maksymalne środki bezpieczeństwa)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.5: Ramy Frontier AI Safety
>white|black||9|11|br Pierwszy zestaw Ram Bezpieczeństwa dla Frontier AI, które zostały opublikowane przez część twórców systemów AI, którzy podpisali Zobowiązania Frontier AI Safety. Ramy obejmują podobne ryzyka (z niewielkimi różnicami) i stosują różne poziomy ryzyka oraz podejścia do zarządzania ryzykiem.


>white|orangered|left|14|15.5|bb Skuteczność Ram bezpieczeństwa Frontier AI jest niepewna

Ramy Bezpieczeństwa Frontier AI mogą pełnić funkcję narzędzi zarządzania ryzykiem w określonych warunkach i dla pewnych kategorii ryzyka, które mają wiarygodną ścieżkę prowadzącą do szkody (‡1117). Jednocześnie kilka analiz podejmuje kwestie dotyczące ich jasności i zakresu (‡111, ‡986) oraz dotyczące odporności progów możliwości i ryzyka AI (‡1031, ‡1130). Istniejące ramy zwykle koncentrują się na wycinku domen ryzyka. W rezultacie niektóre istotne ryzyka, takie jak niezgodne z prawem nadzorowanie (‡1131, ‡1132) oraz intymne obrazy bez zgody (‡287), otrzymują mniejszy nacisk. W odróżnieniu od podejść do zarządzania ryzykiem z innych sektorów, takich jak lotnictwo lub energetyka jądrowa (‡1133*), Ramy Bezpieczeństwa Frontier AI zazwyczaj nie stosują jawnych ilościowych progów ryzyka (‡1134).

Zewnętrzne oceny zgodności deweloperów z ich ramami Frontier AI Safety są jak dotąd ograniczone, po części dlatego, że większość ram jest nowa, dostępnych publicznie informacji jest mało, a nie istnieją standardowe zewnętrzne audyty. Ich skuteczność będzie również zależeć od tego, jak dobrze – i w jakim stopniu – zobowiązania są wdrażane w praktyce. Same te ramy mogą nie zapewniać skutecznego zarządzania ryzykiem, ponieważ ich praktyczny wpływ zależy od tego, jak dobrze – i w jakim stopniu – są wdrażane. Do tej pory nie w pełni odpowiadają międzynarodowym standardom zarządzania ryzykiem (‡1135). Badanie dotyczące wcześniejszych dobrowolnych zobowiązań wykazało nierównomierne wypełnianie poszczególnych środków, co sugeruje, że przestrzeganie dobrowolnych zobowiązań prawdopodobnie będzie się różnić między firmami i domenami (‡1109).

Wzięte razem, Ramy Dobrowolnego Bezpieczeństwa AI Frontier stanowią najbardziej szczegółową formę dobrowolnego zarządzania ryzykiem na poziomie organizacyjnym, obecnie stosowaną, ale różnią się znacznie pod względem zakresu, progów i egzekwowalności.

###@ Inicjatywy regulacyjne i zarządcze

>white|orangered|left|14|15.5|bb Kilka jurysdykcji wprowadziło przepisy z wymogami dotyczącymi przejrzystości

Wiele wczesnych podejść regulacyjnych wprowadza wymogi prawne mające na celu zwiększenie standaryzacji i przejrzystości w zarządzaniu ryzykiem. Rozporządzenie w sprawie AI (EU AI Act), które weszło w życie w 2024, ustanawia wymogi dotyczące przejrzystości, praw autorskich i bezpieczeństwa dla modeli AI o zastosowaniach ogólnego przeznaczenia. W 2025 opublikowano unijny Kodeks praktyk w zakresie AI o zastosowaniach ogólnego przeznaczenia, aby wspierać zgodność z tymi zobowiązaniami poprzez dostarczanie wytycznych dotyczących dokumentacji modelu i praw autorskich, a także – dla najbardziej zaawansowanych modeli – praktyk zarządzania ryzykiem, takich jak ewaluacje, ocena i ograniczanie ryzyka, bezpieczeństwo informacji oraz raportowanie poważnych incydentów (‡965).

Inne przykłady nowych wymogów regulacyjnych obejmują południowokoreańską Ustawę ramową w sprawie rozwoju sztucznej inteligencji i ustanowienia zaufania, która wprowadza wymogi dla „systemów AI o wysokim wpływie” w sektorach krytycznych (‡1136), oraz kalifornijską ustawę SB 53, która ustanawia wymogi dotyczące przejrzystości w zakresie ram bezpieczeństwa oraz raportowania incydentów (‡1104). Biorąc pod uwagę, jak niedawno te wymagania zostały ustanowione, zbyt wcześnie jest, aby szczegółowo ocenić, w jaki sposób wpłyną one na praktyki zarządzania ryzykiem lub na rzeczywiste wyniki ryzyka.

>white|orangered|left|14|15.5|bb Szersze inicjatywy w zakresie zarządzania oferują dobrowolne wytyczne

Wiele regionalnych i międzyregionalnych ram zarządzania ustanawia obecnie wspólne oczekiwania dotyczące zarządzania ryzykami wynikającymi z ogólnego przeznaczenia AI, dostarczając nieobowiązujących wskazówek dla decydentów i organizacji. Chińska „AI Safety Governance Framework 2.0”, opublikowana w 2025, zapewnia ustrukturyzowane wskazówki dotyczące kategoryzacji ryzyka oraz środków zaradczych w całym procesie rozwoju i wdrażania AI (‡1137). Państwa Członkowskie ASEAN opublikowały „ASEAN Expanded Guide on AI Governance and Ethics (Generative AI)”, która dostarcza wskazówek w zakresie zarządzania i etyki dla AI ogólnego przeznaczenia oraz ma wspierać większą zgodność polityk między Państwami Członkowskimi ASEAN (‡1138). Ponadto inicjatywy kierowane przez ekspertów, takie jak „Singapore Consensus”, opracowane przez naukowców AI z wielu krajów, określają priorytety badawcze dla bezpieczeństwa AI ogólnego przeznaczenia w obszarach oceny ryzyka, rozwoju i kontroli (‡690).

###@ Aktualizacje

Od czasu publikacji ostatniego Raportu (styczeń 2025) krajobraz zarządzania ryzykiem dla AI ogólnego przeznaczenia uległ zmianie, wraz z publikacją nowych zasobów, takich jak unijny Kodeks postępowania dla AI ogólnego przeznaczenia, G7 HAIP Reporting Framework, chińskie krajowe ramy zarządzania bezpieczeństwem AI 2.0 oraz różne Frontier AI Safety Frameworks opracowane przez deweloperów AI. Inicjatywy te opisują podejścia i praktyki stosowane przez deweloperów AI w celu zarządzania ryzykami związanymi z systemami AI ogólnego przeznaczenia (‡1115). Istnieje znaczne zróżnicowanie między Frontier AI Safety Frameworks oraz między raportami dotyczącymi przejrzystości HAIP (‡1103), odzwierciedlające różnice w praktykach organizacyjnych, priorytetyzacji ryzyk oraz w początkowym etapie ekosystemu zarządzania ryzykiem dla AI ogólnego przeznaczenia. Zaufany ekosystem, w którym różni interesariusze AI wnoszą uzupełniające praktyki zarządzania ryzykiem w całym cyklu życia, może przyczynić się do skutecznego zarządzania ryzykiem (‡690).

###@ Luki w dowodach

Brakuje dowodów na: jak mierzyć dotkliwość, rozpowszechnienie i horyzont czasowy pojawiających się ryzyk; w jakim stopniu ryzyka te można ograniczać w realnych warunkach; oraz jak skutecznie zachęcać lub egzekwować przyjęcie działań ograniczających przez zróżnicowanych aktorów. Potrzebne są dalsze badania, aby zrozumieć, jak powszechne są poszczególne ryzyka oraz na ile różnią się między regionami świata, w szczególności dla regionów takich jak Azja, Afryka i Ameryka Łacińska, które szybko się cyfryzują. Ponieważ modele AI otrzymują coraz większą sprawczość i autorytet, a stan nauki w zakresie ryzyk związanych z ogólnego przeznaczenia AI postępuje, podejścia do zarządzania ryzykiem również będą musiały się rozwijać (‡639, ‡1139).

Niektóre działania ograniczające ryzyko zyskują na popularności (‡690, ‡956), ale potrzeba więcej badań, aby zrozumieć, na ile odporne w praktyce są działania ograniczające ryzyko i środki ochronne dla różnych społeczności i podmiotów działających w obszarze AI (w tym dla małych i średnich przedsiębiorstw). Większy dostęp do danych dotyczących wdrożeń i użytkowania modeli w rzeczywistym świecie jest istotny dla takich ocen. Ponadto działania z zakresu zarządzania ryzykiem obecnie bardzo się różnią między wiodącymi firmami AI. Argumentowano, że motywacje twórców nie są dobrze dopasowane do rzetelnej oceny ryzyka i zarządzania nim (‡934). Nadal istnieje luka dowodowa dotycząca tego, w jakim stopniu spełniane są różne dobrowolne zobowiązania, jakie przeszkody napotykają firmy w pełnym przestrzeganiu tych zobowiązań oraz jak integrują one Ramy Bezpieczeństwa Frontier AI z szerszymi praktykami zarządzania ryzykiem w obszarze AI.

###@ Wyzwania dla decydentów politycznych

Kluczowe wyzwania obejmują ustalenie, jak priorytetyzować zróżnicowane ryzyka stwarzane przez ogólnego przeznaczenia sztuczną inteligencję, wyjaśnienie, które podmioty są najlepiej przygotowane do ograniczania tych ryzyk oraz zrozumienie zachęt i ograniczeń, które kształtują ich działania. Dowody wskazują, że decydenci polityczni mają obecnie ograniczony dostęp do informacji na temat tego, jak twórcy i wdrażający systemy AI testują, oceniają i monitorują pojawiające się ryzyka, a także na temat skuteczności różnych praktyk łagodzenia (‡1140). Badacze i decydenci polityczni omawiali działania na rzecz przejrzystości oraz bardziej systematyczne raportowanie incydentów jako możliwe sposoby informowania o priorytetyzacji ryzyk, budowania zaufania i wzmacniania zachęt do odpowiedzialnego rozwoju (‡957). W praktyce zarządzanie ryzykiem obejmuje wielu aktorów w całym łańcuchu wartości AI – takich jak dostawcy danych i usług w chmurze, twórcy modeli oraz platformy hostujące modele – z których każdy ma odmienne możliwości oceny i zarządzania różnymi ryzykami (‡1141). Ograniczone udostępnianie informacji między tymi aktorami utrudnia ustalenie, które ryzyka są najbardziej prawdopodobne lub najbardziej istotne, zwłaszcza gdy uwzględnia się skutki społeczne na dalszych etapach.

