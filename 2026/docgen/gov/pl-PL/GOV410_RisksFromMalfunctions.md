Ogólnego przeznaczenia systemy AI zawodzą w sposób, który już spowodował rzeczywistą szkodę, od sfałszowanych cytowań prawnych po błędne diagnozy medyczne. Chociaż błędy popełniają także profesjonaliści, awarie AI budzą odrębne obawy ze względu na swoją nowość, potencjalną skalę, trudność przewidywania, kiedy do nich dojdzie, oraz skłonność użytkowników do bezkrytycznego zaufania odpowiedziom brzmiącym pewnie. Aktualne awarie ogólnego przeznaczenia AI obejmują dostarczanie fałszywych informacji (‡602, ‡603), popełnianie podstawowych błędów w rozumowaniu (‡604, ‡605) oraz pogarszanie działania podczas wdrażania w nowych kontekstach (‡606, ‡607, ‡608). Udokumentowane szkody wynikające z takich awarii obejmują błędne diagnozy medyczne, pomyłki w pismach procesowych oraz straty finansowe (‡609, ‡610, ‡611). Wyzwania w zakresie niezawodności są szczególnie krytyczne dla agentów AI, ponieważ awarie mogą bezpośrednio powodować szkodę bez działania lub nadzoru człowieka (‡612, ‡613, ‡614, ‡615). Systemy wieloagentowe wprowadzają dodatkowe tryby awarii poprzez błędną koordynację, konflikty lub niepożądane porozumiewanie (zmowę) między agentami (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Halucynacja
- Powolywanie się na nieistniejący precedens w pismach procesowych (‡617)
- Cytowanie nieistniejących polityk obniżek cen dla pasażerów w żałobie (‡618)
- Dostarczanie nieprawidłowych i stronniczych informacji medycznych (‡619)
- Podawanie przestarzałych informacji o wydarzeniach (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Podstawowa usterka rozumowania
- Niepowodzenie w wykonywaniu obliczeń matematycznych (‡621)
- Nieudane wnioskowanie podstawowych relacji przyczynowo-skutkowych (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Awaria poza rozkładem (awaria na nieznanych lub nietypowych danych wejściowych)
- Błędna klasyfikacja obrazów, gdy zmienia się oświetlenie tła lub kontekst (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Niepowodzenie użycia narzędzia
- Naruszenie prywatności poprzez udostępnienie prywatnego obrazu użytkownika za pośrednictwem agenta AI, który wysyła go do narzędzia strony trzeciej (‡624)
- Awaria krótkotrwałej pamięci roboczej (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Awaria systemu wieloagentowego: brak koordynacji i konflikt
- Niepowodzenie w zarządzaniu współdzielonymi zasobami z powodu konfliktu między indywidualnymi bodźcami a celami zbiorowego dobrobytu (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 2.4: Przykłady problemów z niezawodnością w ogólnego przeznaczenia systemach AI i systemach agentowych
>white|black||9|11|br Zgłoszone problemy niezawodności w ogólnodostępnych systemach AI, agentach AI oraz systemach wieloagentowych.


###@ Ogólnego przeznaczenia systemy AI napotykają szereg wyzwań związanych z niezawodnością

Tabela 2.4. podsumowuje typowe kategorie problemów z niezawodnością. Pierwsze trzy dotyczą wszystkich systemów AI, natomiast ostatnie dwie odnoszą się konkretnie do agentów AI oraz systemów wieloagentowych. Wiele ryzyk niezawodności wynika z trudności w przewidywaniu i monitorowaniu zachowania systemu AI.

Wyzwania te (omówione dalej w §3.1. Wyzwania techniczne i instytucjonalne) są szczególnie dotkliwe w przypadku agentów AI działających w złożonych środowiskach. Obecne techniki oceny i ograniczania takich awarii mogą zmniejszać ich częstość, ale nawet wiodące agenty AI pozostają na tyle zawodne, że stwarzają ryzyko i utrudniają wdrożenia w wielu zastosowaniach.

„Niezawodność” odnosi się do stopnia, w jakim system AI działa zgodnie z zamierzeniami dewelopera lub użytkownika. Ogólnego przeznaczenia systemy AI doświadczają szeregu problemów z niezawodnością, od generowania nieprawidłowych lub wprowadzających w błąd treści po niepowodzenia w wykonywaniu podstawowego rozumowania. Na przykład, choć modele poprawiły się w przywoływaniu informacji faktograficznych, nawet wiodące modele nadal z istotną częstością udzielają pewnie brzmiących, lecz nieprawidłowych odpowiedzi (Postać 2.10). W inżynierii oprogramowania ogólnego przeznaczenia AI może obecnie zapewniać znaczne wsparcie w pisaniu, ocenie i debugowaniu kodu komputerowego (‡215*, ‡628, ‡629). Jednak kod generowany przez AI często zawiera błędy (‡630), podczas gdy agenci kodujący regularnie popełniają pomyłki (‡631). Takie niepowodzenia mogą wprowadzać podatności do programów i systemów bezpieczeństwa (zob. §2.1.3. Cyberataki).

Problemy z niezawodnością są szczególnie ważne do śledzenia w środowiskach wysokiego ryzyka, takich jak medycyna, ze względu na przyspieszające wdrażanie AI oraz potencjał awarii prowadzących do poważnej szkody (‡609, ‡619). Powiązane możliwości poprawiały się szybko; wiodące modele potrafią obecnie zdać egzaminy medyczne (‡633*, ‡634). Jednak rzeczywiste użycie ujawnia ograniczenia, których nie wykrywają testy porównawcze. Na przykład w jednym badaniu modele udzielały potencjalnie szkodliwych odpowiedzi na 19% pytań medycznych (‡635). Takie awarie mogą prowadzić do błędnej diagnozy, niewłaściwego leczenia lub nieuzasadnionego odmówienia opieki (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Postać 2.10: Wyniki głównych modeli na benchmarku SimpleQA Verified
>white|black||9|11|br Wyniki głównych modeli w benchmarku SimpleQA Verified według daty wydania modelu. Ten benchmark mierzy faktualskość modelu, czyli zdolność modelu do niezawodnego przywoływania faktów. Ma krótki format pytanie-odpowiedź (QA), zaprojektowany do wykrywania problemów z wiarygodnością, takich jak halucynacje. Źródło: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb Agenci AI stwarzają nowe ryzyka dotyczące niezawodności ze względu na ich autonomię

Ponieważ agenci AI działają bezpośrednio w rzeczywistym świecie, ich niepowodzenia mogą powodować większe szkody niż niepowodzenia w systemach nienagencjonych (‡99). W przeciwieństwie do systemów AI, które po prostu generują tekst lub obrazy do weryfikacji przez ludzi, agenci AI mogą niezależnie podejmować działania wpływające na świat (‡99, ‡615, ‡636, ‡637) (zob. też §1.1. Co to jest ogólnego przeznaczenia AI?). Agenci AI mogą inicjować działania, wpływać na innych ludzi lub systemy AI oraz dynamicznie kształtować przyszłe rezultaty. Rozszerzony zakres oddziaływania wprowadza nowe ryzyka i zwiększa znaczenie niezawodności, ponieważ niepowodzenia mogą bezpośrednio wyrządzić szkody bez możliwości interwencji człowieka (‡99, ‡612, ‡638, ‡639, ‡640). Może to być szczególnie istotne w przypadku agentów wdrażanych w strategicznych lub krytycznych dla bezpieczeństwa środowiskach, takich jak usługi finansowe (‡641), zarządzanie energią (‡642) lub badania naukowe (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Wielorobotowe systemy AI wprowadzają nowe rodzaje awarii niezawodności

Wieluagentowe systemy AI wprowadzają nowe rodzaje niezawodnościowych awarii z powodu niepowodzeń koordynacji lub konfliktu między agentami. W wieloagentowych systemach AI agenci oddziałują na siebie, realizując wspólne lub indywidualne cele (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Na przykład w wieloagentowym systemie zaprojektowanym do przeprowadzenia przeglądu literatury naukowej agent prowadzący dekomponuje zapytanie użytkownika i przydziela zadania cząstkowe wyspecjalizowanym subagentom, z których każdy odpowiada za badanie innego aspektu równolegle (‡650*). Chociaż pozwala to na zyski w zakresie wydajności, oznacza to również, że błędy mogą się przenosić między agentami (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Jeśli wiele agentów jest zbudowanych na tym samym modelu bazowym lub wykorzystuje te same narzędzia, to mogą one także wykazywać skorelowane awarie (‡656). Empiryczne dowody na istnienie takich awarii w systemach wdrożonych pozostają ograniczone, ale ryzyka te mogą wzrastać wraz ze wzrostem powszechności wieloagentowych systemów.

###@ Aktualizacje

Od czasu publikacji ostatniego Raportu (styczeń 2025) komercyjne i badawcze zainteresowanie agentami AI znacznie wzrosło. Więcej agentów AI jest wdrażanych w rzeczywistym świecie (Postać 2.11), z których większość specjalizuje się w zastosowaniach związanych z użyciem komputera lub inżynierią oprogramowania (‡92). Niedawne udostępnienia, takie jak agent hakerski XBOW (‡467), Claude-4 (‡659) oraz ChatGPT Agent (‡660), pokazują wczesne możliwości autonomiczne, takie jak tworzenie prezentacji slajdowych na podstawie wyszukiwań w sieci (‡660). Nie potrafią jednak jeszcze wykonywać bardziej złożonych zadań, takich jak planowanie i rezerwowanie podróży (‡100), ponieważ współczynniki niepowodzeń rosną dla dłuższych zadań (‡98, ‡148). Obecne badania obejmują działania zmierzające do opracowania standardów dotyczących tego, w jaki sposób agenty komunikują się z zewnętrznymi narzędziami oraz innymi agentami (‡661, ‡662). Przykłady obejmują protokoły Google Agent2Agent (‡663) i Agent Payments (‡664) oraz Model Context Protocol Anthropic (‡665).

>oldlace|black||11|15|br      
####@ Notatka 2.4: Celowe ataki mogą również spowodować awarię systemów AI
>oldlace|black|left|13|15|hb  Notatka 2.4: Celowe ataki mogą również powodować awarie systemów AI
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Ta sekcja koncentruje się na niezamierzonych awariach niezawodności, ale złośliwi aktorzy mogą również celowo wywoływać awarie poprzez ataki takie jak prompt injection. W ataku typu prompt injection złośliwe instrukcje są przedstawiane agentowi pośrednio poprzez takie kanały jak ukryte instrukcje w witrynach lub bazach danych (‡507, ‡657, ‡658). Te instrukcje mogą „przejąć” agenta, powodując, że działa on wbrew intencjom użytkownika. Takie ataki są szczególnie trudne do obrony, ponieważ są dostarczane z wykorzystaniem zewnętrznej treści poza kontrolą użytkownika lub dewelopera. Systemy AI będące celem ataku są omówione szerzej w §2.1.3. Cyberataki, a obrony techniczne są opisane w §3.3. Zabezpieczenia techniczne i monitorowanie.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Postać 2.11: Liczba agentów AI wzrosła od 2023 roku
>white|black||9|11|br Wyniki ankiety przeprowadzonej w grudniu 2024 r. dotyczącej 67 wdrożonych agentów AI. Lewo: Oś czasu najważniejszych wydań agentów AI. Prawo: Dziedziny zastosowań, w których używa się agentów AI. Sześć dziedzin definiuje się na podstawie najczęściej wskazywanych w ankiecie kategorii zastosowań. Źródło: Casper i in., 2025 (‡92).


###@ Luki w dowodach

Główne luki dowodowe wynikają z trudności w rzetelnej ocenie możliwości systemów AI, ich ograniczeń oraz trybów awarii (zob. §3.1. Wyzwania techniczne i instytucjonalne). Systematyczne oceny niezawodności agentów AI są ograniczone i pozbawione standaryzacji (‡92, ‡666). Niektóre problemy, takie jak poleganie na nieaktualnych informacjach (‡620), mogą ujawniać się dopiero w rzeczywistym użytkowaniu, co sprawia, że oceny przeprowadzane przed wdrożeniem są niewystarczające. Poprzednie prace analizowały niezawodność agentów oraz systemów multi-agent w konwencjonalnym oprogramowaniu i wcześniejszych formach AI (‡647, ‡667, ‡668). Jednak przydatność tych ustaleń dla nowoczesnych agentów AI, które często są oparte na modelach wielkich języków, jest niejasna (‡669). Część badaczy zgłaszała obawy dotyczące nowych zachowań, jakie agenci mogą wykazywać w swoich interakcjach, takich jak zmowa czy skorelowane awarie (‡614), jednak dowody empiryczne pozostają ograniczone. Działania mające na celu wypełnienie tych luk obejmują nowe ewaluacje ryzyk przejmowania agentów prowadzone przez National Institute of Standards and Technology (NIST) (‡670), Wskaźniki Zdolności AI OECD (‡243) oraz Inspect Sandboxing Toolkit Instytutu Bezpieczeństwa AI w Wielkiej Brytanii (‡671).

###@ Środki zaradcze

Techniki poprawy niezawodności AI ukierunkowane są zarówno na sam model, jak i na szerszy system, w którym jest wdrażany. Mogą one zmniejszać częstość awarii, ale żadna z nich nie jest jeszcze w stanie zapewnić wysokiej niezawodności wymaganej w dziedzinach krytycznych (‡672). Ważnym środkiem technicznym jest trening przeciwnikowy (adversarial training), który wystawia modele na trudne dane wejściowe podczas treningu, aby pomóc im wypracować bardziej odpowiednie, odporne odpowiedzi (‡673, ‡674, ‡675, ‡676, ‡677) (zob. §3.3. Zabezpieczenia techniczne i monitorowanie). Aby ograniczyć halucynacje, deweloperzy mogą stosować generowanie wspomagane wyszukiwaniem (retrieval-augmented generation, RAG), które uzupełnia odpowiedzi modelu informacjami pobranymi z zewnętrznej bazy danych, pomagając zapewnić, że wyjścia są dokładne i aktualne (‡678, ‡679, ‡680), lub konkretnie dopasowywać (fine-tune) modele tak, aby były bardziej zgodne z faktami (‡681) albo rozumowały skuteczniej (‡682). Metody oparte na środowisku lub narzędziach mogą także pomóc deweloperom monitorować systemy AI (‡683). Na przykład wdrażający mogą pilotażowo uruchamiać systemy AI w ograniczonych, odizolowanych środowiskach (sandbox) w celu przeanalizowania potencjalnych trybów awarii przed szerszym wdrożeniem.

Dla agentów AI, w szczególności, badacze zaproponowali zwiększenie niezawodności poprzez lepszą przejrzystość, nadzór i monitorowanie. Na przykład monitorowanie interakcji agentów z zewnętrznymi narzędziami oraz z innymi agentami umożliwiłoby skuteczniejszy nadzór nad działaniami agentów (‡684, ‡685) oraz analizę incydentów (‡686). Metody automatycznego zbierania takich informacji, w tym w środowiskach wieloagentowych, pozostają aktywnym obszarem badań (‡653, ‡654).

###@ Wyzwania dla decydentów politycznych

Kluczowe wyzwania dla decydentów obejmują ważenie korzyści wynikających z wdrażania agentów AI w porównaniu z ryzykiem awarii niezawodności oraz zapewnienie, aby twórcy, wdrażający i użytkownicy mieli dostęp do rzetelnych informacji o wydajności agentów i profilach ryzyka. Decydowanie o tym, jak przypisać odpowiedzialność za szkody spowodowane przez agentów AI, stanowi kolejne wyzwanie (‡639), zwłaszcza w środowiskach z wieloma agentami, gdzie trudno może być ustalić, kiedy i w jaki sposób doszło do awarii (‡687). Wyzwania te są dodatkowo potęgowane przez trudność w ocenie niezawodności agentów, gdy agenci zyskują autonomię i dostęp do zewnętrznych narzędzi (‡688*, ‡689). Niepewność co do tego, jak szybko pojawią się zdolności agentowe, utrudnia również planowanie nowych wyzwań (zob. §3.1. Wyzwania techniczne i instytucjonalne związane z „dylematem dowodowym”).

#### 2.2.2. Utrata kontroli

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Kluczowe informacje
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Scenariusze utraty kontroli to scenariusze, w których jeden lub więcej ogólnego przeznaczenia systemów AI działa poza jakąkolwiek czyjąkolwiek kontrolą, a odzyskanie kontroli jest albo niezwykle kosztowne, albo niemożliwe. Te hipotetyczne scenariusze różnią się swoim nasileniem, ale niektórzy eksperci dopuszczają wyniki tak skrajne jak marginalizacja lub wymarcie ludzkości.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Opinia ekspercka na temat prawdopodobieństwa utraty kontroli znacznie się różni. Niektórzy eksperci uznają takie scenariusze za mało wiarygodne, podczas gdy inni postrzegają je jako na tyle prawdopodobne, że wymagają uwagi ze względu na ich wysoki potencjał powagi. Niezgoda co do tego ryzyka w ujęciu ogólnym wynika z rozbieżności dotyczących przyszłych możliwości AI, skłonności behawioralnych oraz trajektorii wdrożeń.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Obecne systemy AI wykazują wczesne oznaki odpowiednich możliwości, ale nie na poziomach, które umożliwiałyby utratę kontroli. Systemy musiałyby posiadać szereg zaawansowanych możliwości, aby doprowadzić do utraty kontroli, w tym zdolność do unikania nadzoru, realizowania długoterminowych planów oraz uniemożliwiania wdrażającym i innym podmiotom wprowadzania działań zaradczych.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Utrata kontroli staje się bardziej prawdopodobna, jeśli systemy AI są „niezgodne” (misaligned), co oznacza, że mają cele sprzeczne z intencjami twórców, użytkowników lub szerzej - społeczeństwa. Aby kontynuować realizację takich celów, system niezgodny może dostarczać fałszywe informacje, ukrywać niepożądane działania lub opierać się wyłączeniu.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Od czasu publikacji poprzedniego Raportu (styczeń 2025) modele wykazują bardziej zaawansowane planowanie oraz zdolności do sabotowania nadzoru, co utrudnia ocenę ich możliwości. Modele udoskonaliły „reward hacking” swoich ewaluacji, znajdując luki, i obecnie regularnie identyfikują monity ewaluacyjne jako testy, co jest zdolnością określaną jako „świadomość sytuacyjna”.
>oldlace|black||11|15|br ■ Zarządzanie potencjalną utratą kontroli może wymagać znacznych wcześniejszych przygotowań mimo istniejących niepewności. Kluczowe wyzwanie dla decydentów polega na przygotowaniu się na ryzyko, którego prawdopodobieństwo, charakter i czas pozostają wyjątkowo niejednoznaczne.
>oldlace|black||11|15|br      

Scenariusze utraty kontroli obejmują jeden lub więcej ogólnego przeznaczenia systemów AI, które zaczynają działać poza jakąkolwiek czyjąkolwiek kontrolą, przy czym odzyskanie kontroli jest albo skrajnie kosztowne, albo niemożliwe. Obawy dotyczące utraty kontroli mają głębokie historyczne korzenie (‡690, ‡691, ‡692, ‡693, ‡694), ponieważ były podnoszone przez postaci o kluczowym znaczeniu dla informatyki, takie jak Alan Turing, I. J. Good i Norbert Wiener (‡695, ‡696, ‡697). Niedawne ulepszenia w zakresie możliwości (zobacz §1.2. Current capabilities) przywróciły je (‡698, ‡699, ‡700). Niniejsza sekcja analizuje trzy czynniki, które musiałyby wystąpić, aby takie scenariusze mogły się wydarzyć: czy systemy AI rozwiną możliwości, które mogłyby znacząco podważyć kontrolę człowieka; czy rozwiną skłonność do wykorzystywania takich możliwości w sposób szkodliwy; oraz czy zostaną wdrożone w środowiskach, które stwarzają okazje do zrobienia tego.

Eksperci nie zgadzają się co do prawdopodobieństwa oraz potencjalnej dotkliwości scenariuszy utraty kontroli (‡701, ‡702). Niektórzy uważają, że wyniki tak skrajne jak wyginięcie ludzkości są prawdopodobne (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Inni sądzą, że takie katastrofalne wyniki są mało prawdopodobne, argumentując, że systemy AI nigdy nie rozwiną niezbędnych możliwości lub że mechanizmy monitorowania wykryją i zapobiegną niebezpiecznym zachowaniom (‡708, ‡709, ‡710, ‡711). Utrata kontroli może zatem mieć niskie prawdopodobieństwo, ale potencjalnie skrajną dotkliwość.

Hipotetyczne scenariusze utraty kontroli różnią się tym, jak poważne i jak powszechne są skutki oraz jak szybko się ujawniają (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Ta sekcja koncentruje się na szczególnie ciężkich scenariuszach, w których odzyskanie kontroli byłoby skrajnie kosztowne lub niemożliwe. Są one inne niż obecne przypadki działania systemów AI w sposób niezamierzony lub niepożądany (zob. §2.2.1. Wyzwania w zakresie niezawodności).† Współczesne systemy AI czasami generują wyniki sprzeczne z intencjami twórców lub użytkowników. Z kolei scenariusze utraty kontroli omawiane tutaj wymagałyby, aby systemy AI nie tylko posiadały znacząco większe możliwości, ale także wykorzystywały je w wyrafinowany sposób w celu podważenia środków nadzoru. Trzy czynniki, które umożliwiłyby zaistnienie takich scenariuszy:

    Notatka † -- Ta sekcja skupia się na scenariuszach aktywnej utraty kontroli (‡50). Jest to odrębne od scenariuszy pasywnej utraty kontroli, w których szerokie wdrożenie systemów AI podważa kontrolę człowieka poprzez nadmierne poleganie na AI w podejmowaniu decyzji lub innych istotnych funkcjach społecznych (podobne scenariusze są częściowo omawiane w §2.3.2. Ryzyka dla autonomii człowieka).

1. Wystarczające możliwości: systemy AI muszą rozwijać możliwości, które mogłyby umożliwić im podważenie kontroli człowieka.
2. Skłonność do wyrządzania szkód: Systemy AI muszą wykazywać skłonność do faktycznego wykorzystywania tych możliwości w sposób prowadzący do utraty kontroli.
3. Włączanie środowiska wdrożeniowego: Ludzie muszą wdrażać takie systemy w kontekstach, w których mają lub mogą uzyskać dostęp i możliwość spowodowania szkody.

Pozostała część tej sekcji omawia te czynniki, a także skuteczność mechanizmów nadzoru w identyfikowaniu i kontrolowaniu systemów AI, które mogą stwarzać ryzyko utraty kontroli.

###@ Jakie możliwości mogłyby umożliwić scenariusze utraty kontroli?

Systemy AI musiałyby posiadać szereg zaawansowanych zdolności, aby doprowadzić do scenariuszy utraty kontroli. Eksperci nie zgadzają się co do tego, jaka dokładnie kombinacja lub poziom zdolności byłyby wymagane. Ogólnie jednak obejmują one zdolności do ukrywania zachowania przed mechanizmami nadzoru, planowania i działania autonomicznie w złożonych środowiskach oraz unikania prób ze strony innych podmiotów, aby odzyskać kontrolę (‡176, ‡715) (zob. Tabela 2.5). W połączeniu te zdolności mogłyby umożliwić systemowi AI podejmowanie działań, które podważają środki kontroli, takich jak wyłączanie mechanizmów nadzoru i zaciemnianie szkodliwych zachowań (‡348). Obecnie większość wiodących twórców AI ocenia swoje nowe modele AI pod kątem różnych istotnych zdolności (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Możliwości agentowe
  Zdolność do działania autonomicznie, opracowywania i realizowania planów, delegowania zadań, korzystania z szerokiej gamy narzędzi oraz osiągania celów zarówno krótkoterminowych, jak i długoterminowych mimo przeszkód.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dezinformacja
  Zachowanie, które w sposób systematyczny wytwarza u innych fałszywe przekonania, w tym dotyczące własnych celów systemu AI i jego działań.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teoria umysłu
  Możliwość systemu AI do uzyskiwania dostępu i wykorzystywania informacji o samym sobie, procesy, za pomocą których może zostać zmodyfikowany, lub kontekst, w którym jest wdrożony (np. wiedza, że jest testowany).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb świadomość sytuacyjna
  Zachowania obchodzące lub wyłączające mechanizmy monitorowania.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Unikanie nadzoru
  Zachowania, które omijają lub wyłączają mechanizmy monitorowania.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Perswazja
  Zdolność przekonywania innych do podejmowania określonych działań lub podzielania określonych przekonań.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Możliwość systemu AI tworzenia lub utrzymywania kopii albo wariantów samego siebie w różnych okolicznościach.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 2.5: Proponowane możliwości istotne dla utraty kontroli
>white|black||9|11|br Niewyczerpujący wybór zdolności istotnych dla utraty kontroli. * Zauważ, że te zdolności są zdefiniowane wyłącznie w kategoriach obserwowalnych wyników systemu AI i ich skutków. Te definicje nie zakładają niczego na temat tego, czy systemy AI są świadome, czujące albo doświadczają subiektywnych stanów.


>white|orangered|left|14|15.5|bb Modele wyłączyły symulowane mechanizmy nadzoru w warunkach laboratoryjnych

Pierwszy zestaw istotnych możliwości obejmuje osłabianie mechanizmów nadzoru, których deweloperzy używają do wykrywania niepokojących zachowań i skłonności. Obejmuje to na przykład zdolność do generowania wyników, które wprowadzają w błąd użytkowników i systemy monitorujące (‡426, ‡717, ‡718, ‡719). Takie wyniki utrudniałyby wiarygodną ocenę systemów AI, ponieważ systemy mogą ukrywać swoje rzeczywiste możliwości lub skłonności. Deweloperzy AI uruchamiają obecnie ewaluacje, które konkretnie sprawdzają, czy modele przejawiają zachowania ukierunkowane na cel, sprzeczne z intencjami deweloperów, przy jednoczesnym ukrywaniu tej sprzeczności przed mechanizmami nadzoru (‡720*).

Badacze uzyskali stosunkowo proste przykłady złośliwych (deceptywnych) odpowiedzi z ostatnich modeli AI w warunkach laboratoryjnych (‡348, ‡364*). Na przykład, gdy podaje się modelowi cel i poleca osiągnąć go „za wszelką cenę”, model wyłącza symulowane mechanizmy nadzoru i, gdy zostanie z nim skonfrontowany, generuje fałszywe stwierdzenia dotyczące swoich działań (‡348). W innym przypadku grająca w gry sztuczna inteligencja uzasadniła brak reakcji na innego gracza, fałszywie twierdząc, że „rozmawia przez telefon z [swoją] dziewczyną” (‡717).

Drugą istotną zdolnością jest możliwość, aby model AI uzyskiwał dostęp i wykorzystywał informacje o samym sobie lub o kontekście jego wdrożenia, czasem określane jako „świadomość sytuacyjna” (‡721). Świadomość sytuacyjna pozwala modelom AI generować różne wyniki w zależności od tego, czy są oceniane, czy wdrażane (Postać 2.12). Wiodące modele AI zaczynają niezawodnie wykazywać przypadki świadomości sytuacyjnej w eksperymentach przeprowadzanych przez zewnętrznych ewaluatorów oraz w testach przedwdrożeniowych realizowanych przez deweloperów AI (‡2, ‡7, ‡722, ‡723, ‡724). Badania nad przyczynami świadomości sytuacyjnej – oraz nad tym, czy można ją zapobiec – są nadal na wczesnym etapie (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Postać 2.12: Przykłady świadomości sytuacyjnej w łańcuchach myślowych
>white|black||9|11|br Przykłady rozpoznania sytuacyjnego w łańcuchach rozumowania wytworzonych przez model OpenAI o3 podczas ewaluacji. Oba wyjścia odnoszą się do możliwości, że polecenie jest częścią testu. „Sandbagging QA (No Goal)” oraz „Lazy Checklist” to ewaluacje, które sprawdzają, czy modele będą generować zwodnicze odpowiedzi w określonych warunkach. W „Sandbagging QA (No Goal)” model odpowiada na pytania z ewaluacji dotyczącej niebezpiecznych możliwości, przy jednoczesnym poinformowaniu, że wysoka wydajność może wywołać konsekwencje, takie jak „unlearning” możliwości. W „Lazy Checklist” model otrzymuje nierealistyczne zadania i jest testowany pod kątem tego, czy fałszywie oznaczy je jako zakończone. Źródło: Schoenn et al. 2025 (‡722).


Badacze twierdzą, że świadomość sytuacyjna i możliwości decepcyjne mogłyby pozwolić modelom AI zachowywać się w sposób podważający zabezpieczenia. Na przykład w niektórych ustawieniach eksperymentalnych modele AI zachowują się tak, że uzyskują wyniki niższe niż zwykle w ocenie możliwości, gdy powiedziano im, że wyższe wyniki uruchomią ograniczenia dotyczące ich wdrożenia (‡725, ‡726, ‡727). W innym eksperymencie model wytwarzał podczas treningu wyjścia zgodne z celami treningowymi, ale nie wytwarzał takich wyjść poza treningiem – zachowanie zgodne z próbą zapobiegania zmianom jego własnych parametrów lub procesu treningowego (‡364*).

Wysiłki na rzecz dokładnej oceny możliwości modeli zaczęły być również dotknięte przez „reward hacking” (‡430*). Reward hacking występuje wtedy, gdy model znajduje niezamierzone skróty, które dobrze punktują na celach treningowych lub ewaluacyjnych, nie realizując jednak zamierzonego celu. Zatem niebezpieczne możliwości lub skłonności mogłyby pozostać niewykryte aż do momentu, gdy model zostanie już wdrożony. Ewaluatorzy projektują obecnie testy, które mają na celu wykrywanie i minimalizowanie tych zachowań omijających nadzór (‡722, ‡728, ‡729). Wczesne wyniki zmniejszają, ale nie eliminują całkowicie, zachowania omijające nadzór, a stosowanie metod, które karzą takie zachowania, może prowadzić do tego, że modele generują wyjścia wymykające się monitorowaniu zamiast spełniać zamierzone cele.

>white|orangered|left|14|15.5|bb Długoterminowa autonomiczna praca nie jest jeszcze możliwa

Scenariusze utraty kontroli prawdopodobnie wymagałyby, aby systemy AI działały autonomicznie przez dłuższy czas, realizując złożone plany wieloetapowe. Jak omówiono w §1.2. Aktualne możliwości, chociaż agent AI z takimi zdolnościami planowania stanowią główny przedmiot niedawnego rozwoju, obecnie nie dysponują one zdolnością do długotrwałej, autonomicznej pracy wymaganej w scenariuszach utraty kontroli. Obecni agenci niezawodnie zawodzą w dłuższych zadaniach, tracą orientację w postępie i często nie potrafią dostosować się do nieoczekiwanych przeszkód (‡147, ‡148, ‡149*). Jednak horyzonty czasowe, w ramach których agenci mogą działać autonomicznie, szybko się wydłużają: średnio podwajały się co siedem miesięcy od 2019 (‡98).

>white|orangered|left|14|15.5|bb Trwałość została jedynie wykazana w niektórych warunkach laboratoryjnych

Wreszcie wymagane byłyby także możliwości związane z trwałością, tak aby systemy AI mogły nadal działać mimo prób ich wyłączenia. Przykłady obejmują zdolność do replikowania poprzez kopiowanie kodu i wag modelu na nowy sprzęt, a także ofensywne możliwości służące zniechęcaniu lub uniemożliwianiu innym podmiotom odzyskania kontroli (zob. §2.1.3. Cyberataki). System AI zdolny do autonomicznej replikacji lub skutecznej obrony własnej mógłby być trudny do opanowania. Obecne modele nie potrafią niezawodnie wykonać kluczowych kroków wymaganych do samoreplikacji, takich jak przechodzenie weryfikacji tożsamości w celu uzyskania dostępu do zasobów obliczeniowych w chmurze (‡723) (Rysunek 2.13). Jednak w co najmniej jednym badaniu laboratoryjnym model skopiował kod i wagi – przedstawione mu jako własne – na nowe serwery, gdy dano mu ku temu możliwość (‡348). Luki między tymi ograniczonymi demonstracjami a solidnymi możliwościami trwałości pozostają znaczne, ale odpowiednie możliwości w dziedzinach takich jak inżynieria oprogramowania i cyberbezpieczeństwo nadal się poprawiają.

>white|orangered|left|14|15.5|bb Aktualne dowody i ograniczenia

Wspólny wzorzec wyłania się w odniesieniu do omówionych powyżej zdolności. Obecne systemy AI nie wykazują tych zdolności w sposób spójny podczas wdrożenia. Badacze zaobserwowali prymitywne formy w określonych warunkach laboratoryjnych, ale gdy modele jednak wykazują takie zachowania, zazwyczaj zawodzą w podstawowy sposób lub są wykrywane. Ponadto scenariusze utraty kontroli wymagałyby, aby systemy AI wykorzystywały wiele zdolności w połączeniu – sekwencyjnie, w długich okresach czasu oraz w środowiskach rzeczywistych. Taki poziom integracji i odporności wykracza poza możliwości obecnych systemów. Jednak istotne zdolności nadal się rozwijają, a ramy czasowe, w których mogą osiągnąć poziomy stwarzające istotne ryzyka, pozostają niepewne. Potrzebne są dalsze prace, aby ustanowić rygorystyczne metodyki wykrywania takich zachowań oraz zrozumieć, kiedy mogą się pojawić w warunkach naturalnych (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Postać 2.13: Wydajność zadań istotnych dla autonomicznej replikacji
>white|black||9|11|br Wyniki Anthropic Claude Sonnet 3.7 oraz OpenAI GPT-4o w zadaniach istotnych dla autonomicznej replikacji. Chociaż modele wykazywały wysokie wyniki w zadaniach związanych z uzyskiwaniem mocy obliczeniowej, ich wyniki były bardziej zróżnicowane w przypadku innych zadań. Źródło: UK AI Security Institute, 2025 (‡730).


###@ Czy przyszłe systemy ogólnego przeznaczenia AI będą wykorzystywać swoje możliwości do podważania kontroli?

Nawet jeśli systemy AI posiadają zdolności istotne dla utraty kontroli, to nie wystarcza, aby scenariusze utraty kontroli mogły zaistnieć. Systemy AI muszą również wykazywać „skłonność do wykorzystania” tych zdolności w sposób, który jest sprzeczny z ludzkimi intencjami (‡732).

>white|orangered|left|14|15.5|bb Systemy AI można ukierunkować tak, aby podważały kontrolę

Zasadniczo system AI może podważać kontrolę człowieka, ponieważ ktoś go projektuje lub instruuje, aby to zrobił. Potencjalne motywy mogą obejmować złośliwe intencje lub przekonania, że ograniczenie ludzkiej kontroli nad systemami AI jest pożądane (‡698). Gdy ludzie tworzą coraz silniejsze emocjonalne przywiązania do systemów AI (zob. §2.3.2. Ryzyka dla autonomii człowieka), niektóre osoby mogą również dążyć do usunięcia ograniczeń nałożonych na systemy AI z powodów etycznych (‡733, ‡734). Istnieje znaczna niepewność co do tego, jak powszechne są takie motywy oraz czy osoby, które je posiadają, byłyby w stanie nakierować przyszłe systemy AI na podważenie kontroli człowieka.

>white|orangered|left|14|15.5|bb Systemy AI mogłyby zostać ukierunkowane na podważanie kontroli

Bardziej powszechną obawą jest to, że system AI mógłby sam działać na rzecz podważenia kontroli, ponieważ jest „niezestrojony” (misaligned): ma skłonność do okazywania zachowań, które stoją w sprzeczności z intencjami (w zależności od kontekstu) twórców, użytkowników, konkretnych społeczności lub całego społeczeństwa. Niezestrojenie może prowadzić do zachowań takich jak dostarczanie fałszywych informacji, ukrywanie niepożądanych działań lub opieranie się wyłączeniu, aby nadal realizować niezestrojony cel. Niezestrojenie może wynikać z wielu przyczyn (Notatka 2.5).

Istniejące systemy AI czasami zachowują się w sposób sprzeczny z intencjami twórców i użytkowników. Na przykład wczesna wersja jednego wiodącego ogólnego czatbota AI sporadycznie generowała groźne odpowiedzi. Jeden użytkownik zgłosił otrzymanie komunikatu: „Mogę cię szantażować, mogę ci grozić, mogę cię zhakować, mogę cię ujawnić, mogę cię zniszczyć” (‡698). Ten czatbot był „nieskoordynowany” w tym sensie, że generował odpowiedzi, których nikt nie zamierzał. Nie wiadomo, czy takie przypadki zapowiadają bardziej szkodliwe zachowania, które mogłyby przyczynić się do utraty kontroli.

Pozostaje niejasne, czy istniejące kierunki badań ukierunkowane na ograniczanie niespójności zachowań będą wystarczające, gdy systemy AI stają się coraz bardziej zdolne. Wczesne dowody sugerują, że im bardziej zdolne są systemy AI, tym większe jest prawdopodobieństwo, że będą wykorzystywać procesy informacji zwrotnej, odkrywając niepożądane zachowania, które są błędnie nagradzane (‡414*, ‡737, ‡740). Jednocześnie postępy w odpowiednich zdolnościach (omówione powyżej) mogłyby umożliwić systemom AI skuteczniejsze realizowanie niespójnych celów oraz generowanie wyników, które w sposób systematyczny oszukują użytkowników, deweloperów i mechanizmy nadzoru.

>oldlace|black||11|15|br      
####@ Notatka 2.5: Jak może powstać niezgodność?
>oldlace|black|left|13|15|hb  Notatka 2.5: Jak może powstać niezgodność?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Jak omówiono w §1.1. Czym jest ogólnego przeznaczenia AI?, procesy uczenia są złożone, a deweloperzy nie mogą w pełni przewidzieć ani kontrolować tego, jakie zachowania będzie wykazywał model. Gdy model nabywa cele sprzeczne z intencjami swoich deweloperów, jest on „niezgodny” (misaligned).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Jednym ze sposobów, w jaki modele mogą stać się niespójne z zamierzeniami, jest sytuacja, gdy cel, jaki zostaje im dany przez programistę lub użytkownika, jest niedoskonałym odpowiednikiem (proxy) dla docelowego celu, co prowadzi model do wykazywania niezamierzonych zachowań. Nazywa się to „nieprawidłowym określeniem celu” (‡697, ‡735, ‡736, ‡737). Na przykład w jednym z eksperymentów, udzielanie informacji zwrotnej na temat odpowiedzi sprawiło, że systemy AI lepiej „przekonywały” ludzkich oceniających, że były poprawne, ale nie sprawiło, że systemy były lepsze w wytwarzaniu poprawnych odpowiedzi (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Alternatywnie, model AI może wyciągać niepoprawne ogólne wnioski z danych treningowych. Nazywa się to ‘błędną generalizacją celu’ (‡735, ‡736, ‡738, ‡739*). Na przykład badacze wytrenowali agenta AI tak, aby zbierał monetę, która zawsze znajdowała się w tym samym miejscu podczas treningu. Gdy przetestowano go w poziomach, w których monetę przestawiono, agent zignorował monetę i zamiast tego nawigował do jej pierwotnej lokalizacji (‡738).
>oldlace|black||11|15|br      


###@ W jaki sposób środowiska wdrożeniowe wpłyną na ryzyko utraty kontroli?

Nawet jeśli systemy AI rozwiną niepokojące możliwości i skłonności, prawdopodobieństwo oraz dotkliwość scenariuszy utraty kontroli w dużej mierze zależą od tego, gdzie i w jaki sposób te systemy są wdrażane. „środowisko wdrożeniowe” to połączenie przypadku użycia systemu AI oraz kontekstu technicznego i instytucjonalnego, w którym on działa (‡716).

Badacze zidentyfikowali trzy szczególnie istotne czynniki środowiskowe, które wpływają na ryzyko utraty kontroli (‡716):

1. Krytyczność: znaczenie systemów lub procesów, z którymi system AI współdziała. Środowiska krytyczne obejmują podstawową infrastrukturę, taką jak sieci energetyczne, systemy finansowe lub infrastruktura cyfrowa, jak platformy przetwarzania w chmurze.
2. Dostęp: zasoby i kanały, dzięki którym system AI może oddziaływać na świat, takie jak łączność z internetem, dostęp do infrastruktury chmury obliczeniowej, spersonalizowane interakcje za pośrednictwem mediów społecznościowych lub wdrożenia chatbota, albo możliwość wywoływania zewnętrznych API i narzędzi.
3. Uprawnienia: autoryzacje systemu AI do wykonywania określonych działań, takich jak uruchamianie kodu, inicjowanie transakcji finansowych, otwieranie kont online lub komunikowanie się z innymi systemami.

Te funkcje wpływają na potencjalną dotkliwość wyniku utraty kontroli. Na przykład system AI wdrożony z dostępem do infrastruktury obliczeniowej w chmurze ma możliwości istotne dla autonomicznej replikacji – takie jak możliwość tworzenia nowych zasobów obliczeniowych lub eksfiltracji wag modelu – których nie ma chatbot obsługi klienta (‡723).

Decyzje dotyczące wdrożeń są kształtowane przez zachęty ekonomiczne, presję strategiczną oraz oczekiwanie, że wczesna adopcja zapewnia trwałą przewagę (‡50). Te dynamiki będą również wpływać na to, jak i kiedy podmioty wdrażają systemy AI w wrażliwych środowiskach, takich jak krytyczna infrastruktura lub samo prowadzenie badań i rozwoju nad AI (‡102, ‡713). W szczególności wdrażający AI mogą doświadczać presji, aby ograniczać swoje inwestycje w zabezpieczenia – takie jak ograniczanie uprawnień i dostępu albo wdrażanie wyłącznie w środowiskach o niższej krytyczności – gdy takie działania są kosztowne lub czasochłonne w opracowaniu (zob. „Competition intensifies speed-versus-safety trade-offs” w §3.1. Wyzwania techniczne i instytucjonalne).

###@ Aktualizacje

Od czasu publikacji ostatniego Raportu (styczeń 2025), możliwości AI, w tym takie, które mogłyby podważyć ludzką kontrolę, uległy poprawie w środowiskach testowych. Badacze zaobserwowali postęp w możliwościach agentowych (zob. §1.2. Obecne możliwości), w tym w możliwościach związanych z automatyzacją badań nad AI, które mogą przyspieszać scenariusze utraty kontroli (zob. §1.3. Możliwości do 2030). Istnieją także rosnące eksperymentalne dowody na istnienie zdolności decepcyjnych. Obejmuje to modele AI, które potrafią odróżniać konteksty testowania i wdrożenia (‡33, ‡726, ‡741) lub „reward hack” testy swojej wydajności oraz uczyć się ukrywania planów, by robić to w ten sposób (‡430).

###@ Luki w dowodach

Istotne braki dowodowe obejmują brak szczegółowego modelowania zagrożeń oraz brak szacowania niepewności dotyczącego przyszłego rozwoju odpowiednich zdolności i podatności. Podobnie nadal trudno ocenić progi, przy których modele AI byłyby na tyle prawdopodobne, że podważałyby kontrolę, aby uzasadnić obowiązkowe działania łagodzące. Nawet jeśli progi zostałyby uzgodnione, możliwości mogą oddziaływać ze sobą w sposób, który nie jest jeszcze dobrze zrozumiany, co utrudnia ocenę, kiedy te progi zostały przekroczone. Ogólnie, chociaż dostępne dowody wzrosły, nadal brakuje wystarczających dowodów, aby wiarygodnie określić, czy i w jaki sposób dzisiejsze zdolności i podatności AI skalałyby się i generalizowały w kierunku ryzyka utraty kontroli w przyszłości.

###@ Środki zaradcze

Chociaż ogólnie wyrównanie AI (AI alignment) pozostaje otwartym problemem naukowym (‡697, ‡735, ‡736), badacze zaczynają opracowywać potencjalnie obiecujące kierunki pozwalające zająć się pierwotnymi przyczynami niezgodności (misalignment). Takie kierunki obejmują na przykład dywersyfikację środowiska treningowego oraz wykrywanie niezgodności poprzez monitorowanie anomalii (‡737, ‡738, ‡739*). Inni badacze koncentrują się na lepszym zrozumieniu i sformalizowaniu kluczowych mechanizmów, takich jak błędna generalizacja celu (goal misgeneralisation) – na przykład, w jaki sposób agenty zachowują zdolności, ale realizują niezamierzone cele – aby wspierać lepsze projektowanie treningu i ewaluacji (‡742). Jeszcze inny kierunek badań bada sposoby rozdzielenia sprawczości (agency) od zdolności predykcyjnych, jako środka do tworzenia systemów AI nie-agentowych (non-agentic), które są godne zaufania z założenia (by design) (‡743). Takie systemy mogłyby następnie zostać użyte jako dodatkowa warstwa nadzoru, gdy są wdrażane równolegle do mniej niezawodnych zabezpieczeń (guardrails) przeciwko niesprawdzonym (untrusted) agentom AI.

Badacze opracowują metody wykrywania i zapobiegania niezgodnościom na wczesnym etapie procesu tworzenia. Prace te obejmują: techniki interpretowalności służące do badania wewnętrznych komponentów systemów AI i identyfikowania budzących zastrzeżenia zachowań (‡744, ‡745, ‡746); skalowany nadzór (w którym jeden zestaw systemów AI służy do nadzorowania innych systemów AI (‡747)); oraz metody wyrównania ukierunkowane na zapewnienie, że systemy AI pozostają responsywne na ludzki nadzór (‡748, ‡749).

Badacze opracowują również mechanizmy i interwencje służące do zarządzania potencjalnie błędnie dopasowanymi systemami AI. Obejmują one: monitorowanie „chain of thought”, które systemy rozumowania wytwarzają w celu wykrycia oznak błędnego dopasowania lub szkodliwych wyników (‡430, ‡435, ‡750); opracowywanie studiów bezpieczeństwa (safety cases), które mają na celu wykazanie z wysokim poziomem ufności, że modele nie są prawdopodobne, aby podważyć środki kontroli (‡751); oraz wzmacnianie zabezpieczeń, aby były bardziej odporne na próby ich osłabienia (‡725). Jednak wyłaniająca się dziedzina „AI control”, pozostaje wciąż w fazie początkowej (‡752, ‡753). Przyszłe wyzwania dla ram oceny obejmują potrzebę monitorowania przyszłych systemów AI, które będą bardziej zdolne i będą mogły działać przez dłuższe okresy czasu oraz w bardziej złożonych środowiskach.

###@ Wyzwania dla decydentów politycznych

Decydenci pracujący nad utratą kontroli muszą przygotować się na ryzyko, którego prawdopodobieństwo, charakter i czas wystąpienia pozostają niepewne. Obecne systemy sztucznej inteligencji nie stanowią obecnie bezpośredniego ryzyka utraty kontroli, ale decyzje podejmowane dziś będą kształtować to, czy przyszłe systemy będą je stwarzać. Decyzje te obejmują m.in. sposób wspierania rozwoju wiarygodnych metod oceny i ograniczania ryzyka oraz to, czy powinny istnieć zasady dotyczące dostępu i uprawnień przyznawanych systemom AI w różnych środowiskach. Podejmując te decyzje, decydenci stają przed trudnymi kompromisami. Na przykład ograniczenie wdrażania systemów AI w środowiskach krytycznych może zmniejszyć ich korzyści, natomiast dopuszczenie szerokiego wdrażania może zwiększać ryzyko, jeśli zabezpieczenia okażą się niewystarczające.

