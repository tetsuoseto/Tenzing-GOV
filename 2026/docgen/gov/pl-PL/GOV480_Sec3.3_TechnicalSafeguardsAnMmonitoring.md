##########
>white|orangered|left|14|30|hr Sekcja 3.3
### 3.3. Techniczne zabezpieczenia i monitorowanie
>white|orangered|left|24|30|hb Techniczne środki ochronne i monitorowanie

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Kluczowe informacje
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Stosuje się szeroki zakres technicznych zabezpieczeń na różnych etapach rozwoju i użytkowania AI. Obejmuje to techniki stosowane podczas opracowywania modelu, aby systemy były bardziej odporne i mniej podatne na nadużycia (takie jak dobór i kuracja danych), monitorowanie oraz kontrolę w czasie wdrożenia (takie jak filtrowanie treści i nadzór człowieka) oraz narzędzia po wdrożeniu do monitorowania szerszego ekosystemu AI (takie jak wykrywanie pochodzenia i detekcja treści).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Zabezpieczenia techniczne mają ograniczenia i nie zapobiegają w sposób niezawodny szkodliwym zachowaniom we wszystkich kontekstach. Na przykład użytkownicy czasami mogą uzyskać szkodliwe wyniki, przeformułowując polecenia lub dzieląc je na mniejsze kroki. Podobnie narzędzia takie jak watermarking, zaprojektowane do identyfikowania treści wygenerowanych przez AI, często da się usunąć lub zmienić, co ogranicza ich niezawodność.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Ograniczenia poszczególnych zabezpieczeń oznaczają, że może być potrzebne podejście „obrona na wielu poziomach” (defence-in-depth), aby zapobiec niektórym szkodliwym skutkom. Na przykład system może łączyć model wytrenowany pod kątem bezpieczeństwa z filtrami wejściowymi, filtrami wyjściowymi oraz monitorami treści.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Od czasu opublikowania ostatniego Raportu (styczeń 2025) badacze poczynili postępy we wzmacnianiu zabezpieczeń, ale pozostają zasadnicze ograniczenia. Na przykład skuteczność ataków zaprojektowanych w celu obejścia zabezpieczeń spada, lecz nadal jest stosunkowo wysoka. Istnieją również zasadnicze ograniczenia dotyczące tego, jak dokładnie można zabezpieczyć modele z otwartymi wagami.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kluczowym wyzwaniem dla decydentów jest ograniczona liczba dowodów dotyczących tego, jak skuteczne są zabezpieczenia w różnych rzeczywistych zastosowaniach ogólnego przeznaczenia systemów AI. Twórcy systemów AI bardzo różnią się tym, ile informacji udostępniają na temat swoich zabezpieczeń i monitorowania. Dodatkowym wyzwaniem są możliwe kompromisy między wdrażaniem silniejszych zabezpieczeń a utrzymaniem wydajności lub użyteczności systemu.
>oldlace|black||11|15|br      


Twórcy systemów AI mogą wykorzystywać kilka przydatnych, lecz niedoskonałych technicznych zabezpieczeń, aby ograniczać i zarządzać ryzykami wynikającymi z ogólnego przeznaczenia systemów AI, jednak wyzwania związane z odpornością nadal pozostają. Twórcy nadal nie są w stanie w pełni uniemożliwić ogólnego przeznaczenia systemom AI wykonywania nawet powszechnie znanych i w sposób jednoznaczny szkodliwych działań, takich jak udzielanie użytkownikom instrukcji popełniania przestępstw. Na przykład badacze pokazali, że najlepiej obecnie działające zabezpieczenia można obejść za pomocą metod obejścia przez promptowanie adwersarialne (tj. „jailbreaks”) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), poprzez skłanianie modeli do rozbijania złożonych szkodliwych zadań na kroki (‡1150, ‡1151, ‡1152, ‡1153, ‡1154) oraz przy użyciu prostych modyfikacji modeli (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Badacze w dalszym ciągu pracują nad zabezpieczeniami przeciwko awariom i nadużyciom (‡690). Metody te różnią się znacząco pod względem celu i skuteczności, a ich wpływ ostatecznie zależy od szerszego kontekstu socjotechnicznego i zarządczego, w ramach którego systemy AI są budowane i wdrażane.

Środki techniczne można ogólnie podzielić na trzy kategorie: techniki opracowywania bezpieczniejszych modeli; techniki stosowane w trakcie wdrożenia do monitorowania i kontroli; oraz techniki wspierające monitorowanie ekosystemu po wdrożeniu. Tabela 3.6 podsumowuje omawiane środki techniczne, ich skuteczność oraz otwarte wyzwania.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Opracowywanie bezpieczniejszych modeli
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pielęgnacja danych (‡1167)
  Usuwanie szkodliwych danych, aby zapobiec temu, by model uczył się niebezpiecznych możliwości. Metody te mogą być przydatne, w tym przy opracowywaniu modeli o otwartych wagach, które nie mają szkodliwych możliwości i opierają się szkodliwemu dostrajaniu (‡55). Jednak występują wyzwania związane z błędami w doborze danych i skalowaniem (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Uczenie ze wzmocnieniem na podstawie informacji zwrotnych od ludzi (‡64*)
  Trenowanie modelu, aby dopasować się do określonych celów, takich jak bycie pomocnym i nieszkodliwym. Jest to skuteczny sposób, aby modele nauczyły się korzystnych zachowań (‡64*). Jednak nadmierna optymalizacja pod kątem ludzkiej akceptacji może sprawić, że modele będą zachowywać się w sposób zwodniczy lub pochlebny (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Techniki wieloaspektowego dopasowania (‡1170)
  Trenowanie modelu, aby integrował wiele różnych perspektyw co do tego, jak powinien działać. Techniki te pomagają ograniczyć w jakim stopniu modele faworyzują określone perspektywy (‡1170). Jednak mimo tych technik niezgoda ludzi jest nieunikniona, a trudno jest zaprojektować powszechnie akceptowane sposoby równoważenia konkurujących ze sobą poglądów (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Trening adwersarialny (‡677)
  Uczenie modelu odmawiania wyrządzania krzywdy (nawet w nieznanych kontekstach) oraz opierania się atakom ze strony złośliwych użytkowników (np. „jailbreaks”). Jest to skuteczna metoda sprawiania, że modele opierają się próbom nadużyć (‡1064), ale wyzwania związane z odpornością nadal pozostają (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Maszynowe „wyuczenie na nowo” (‡1175, ‡1176)
  Trenowanie modelu przy użyciu wyspecjalizowanych algorytmów oznacza celowe tłumienie szkodliwych możliwości (np. wiedzy o zagrożeniach biologicznych). Techniki te zapewniają ukierunkowany sposób usuwania szkodliwych możliwości z modeli (‡1175, ‡1176), ale obecne algorytmy uczenia zapominania mogą być nieodporne i powodować niezamierzone skutki dla innych możliwości (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Narzędzia do weryfikacji interpretowalności i bezpieczeństwa (‡1177)
  Zróżnicowany zestaw metod projektowania i weryfikacji, mający na celu zapewnienie bardziej rygorystycznej gwarancji, że modele posiadają określone właściwości związane z bezpieczeństwem. Umożliwiają oceniającym formułowanie wysoce wiarygodnych zapewnień dotyczących bezpieczeństwa (‡1177), jednak obecne metody opierają się na założeniach i rzadko osiągają konkurencyjną wydajność w praktyce (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Monitoring i kontrola
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mechanizmy monitorowania oparte na sprzęcie (‡1179, ‡1180, ‡1181)
  Weryfikowanie, że autoryzowane procesy działają na sprzęcie w celu badania zagrożeń bezpieczeństwa lub zgodności regulacyjnej. Mechanizmy te oferują unikalne sposoby monitorowania tego, jakie obliczenia są uruchamiane na sprzęcie i przez kogo (‡1181). Jednak mechanizmy sprzętowe nie mogą wykrywać wszystkich rodzajów zagrożeń, a niektóre techniki wymagają wyspecjalizowanego sprzętu (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitorowanie interakcji użytkownika (‡1154, ‡1166)
  Monitorowanie interakcji użytkowników pod kątem oznak złośliwego wykorzystania może pomóc deweloperom przerwać świadczenie usługi użytkownikom nadużywającym jej w sposób złośliwy (‡1154, ‡1166). Jednak egzekwowanie zasad może niezamierzenie utrudniać korzystne badania nad bezpieczeństwem (‡689), a niektóre formy nadużyć są trudne do wykrycia (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitorowanie interakcji użytkownika (‡1154, ‡1166)
  Monitorowanie interakcji użytkowników pod kątem oznak złośliwego wykorzystania może pomóc deweloperom zakończyć świadczenie usługi dla złośliwych użytkowników (‡1154, ‡1166). Jednak egzekwowanie zasad może niechcący utrudniać prowadzenie korzystnych badań nad bezpieczeństwem (‡689), a niektóre formy nadużyć są trudne do wykrycia (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Filtry treści (‡65*, ‡725)
  Filtrowanie potencjalnie szkodliwych wejść i wyjść modelu jest bardzo skutecznym sposobem na ograniczenie przypadkowych szkód oraz ryzyka nadużyć (‡725). Jednak filtry wymagają dodatkowych zasobów obliczeniowych i są podatne na niektóre ataki (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitory wewnętrznych obliczeń modelu (‡744, ‡1183, ‡1184)
  Monitorowanie oznak oszustwa lub innych szkodliwych wewnętrznych form poznania w modelach może stanowić skuteczny sposób wykrywania oszustwa (‡744, ‡1183, ‡1184). Jednak obecne metody nie zapewniają wystarczającej odporności i niezawodności (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitory łańcucha rozumowania (‡430, ‡435)
  Monitorowanie treści „chain-of-thought” modelu pod kątem oznak mylącego zachowania lub innego szkodliwego rozumowania jest skutecznym sposobem na zrozumienie i wykrycie wad w tym, jak modele rozumują (‡435). Jednak mogą być one zawodne (‡752, ‡753, ‡1186), a jeśli modele są trenowane w celu wytwarzania łagodnego „chain-of-thought”, mogą nauczyć się mylącego zachowania (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Człowiek w pętli (‡1187, ‡1188, ‡1189)
  Nadzór człowieka i możliwość nadpisania decyzji systemowych są niezbędne w niektórych aplikacjach o krytycznym znaczeniu dla bezpieczeństwa (‡1187). Jednakże techniki te są ograniczone przez błąd automatyzacji i ograniczenia dotyczące szybkości podejmowania decyzji przez człowieka (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Izolacja środowiska (‡1192)
  Zapobieganie temu, aby agent AI bezpośrednio wpływał na świat, jest skutecznym sposobem ograniczania szkód, jakie może spowodować (‡1192). Jednak sandboxing ogranicza zdolność systemu do bezpośredniego realizowania niektórych zadań (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Narzędzia ułatwiające monitorowanie ekosystemu
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Techniki identyfikacji modeli AI (‡1193*, ‡1194)
  Ułatwianie identyfikacji modeli, lub pojedynczych instancji modeli, w rzeczywistych przypadkach użycia wspiera cyfrową analizę kryminalistyczną i świadomość ekosystemu (‡1195). Jednak techniki te można obejść poprzez niektóre typy modyfikacji modeli (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dziedziczenie wnioskowania modeli AI (‡1197)
  Te techniki umożliwiają badaczom analizę tego, w jaki sposób modele są modyfikowane w ekosystemie AI, szczególnie w przypadku modeli o otwartych wagach. Pomagają w informatyce śledczej (digital forensics) oraz w uświadamianiu o ekosystemie (‡1198), ale potrzebne byłyby projekty na dużą skalę, aby dokładnie odwzorować ekosystem modeli o otwartych wagach (‡1198) .
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Znak wodny i metadane (‡1199, ‡1200, ‡1201*)
  Te techniki ułatwiają wykrycie, kiedy dany fragment tekstu, obrazu, wideo itp. został wygenerowany lub zmodyfikowany przez AI oraz przez jaki system. Ułatwiają one lepszą świadomość ekosystemu (‡1199, ‡1200, ‡1201*). Jednakże znaki wodne i metadane mogą zostać sfałszowane lub usunięte w wyniku niektórych modyfikacji treści (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Wykrywanie treści generowanych przez AI (‡1203, ‡1204, ‡1205*)
  Poprawa zdolności użytkowników do odróżniania treści generowanych przez AI od treści autentycznych wspiera dochodzenia informatyczne i świadomość ekosystemową (‡1203, ‡1204). Jednak klasyfikatory mogą być zawodne (‡1205*) i wykazywać zmienną wydajność w różnych modalnościach.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.6: Zabezpieczenia techniczne omawiane w tej sekcji
>white|black||9|11|br Podsumowanie technicznych zabezpieczeń omówionych w tej sekcji, podzielone na metody opracowywania bezpieczniejszych modeli, monitorowanie i kontrolę w czasie wdrożenia oraz techniki ułatwiające monitorowanie ekosystemu.


###@ Opracowywanie bezpieczniejszych modeli

Pierwszą linią obrony przed szkodami wynikającymi z ogólnego przeznaczenia systemów AI jest uczynienie bazowego modelu bezpieczniejszym. Niniejsza podsekcja obejmuje zabezpieczenia „wbudowane w parametry modelu” podczas procesu jego opracowywania (Postać 3.6).

>white|orangered|left|14|15.5|bb Kuratowanie danych treningowych może ograniczać rozwój potencjalnie niebezpiecznych możliwości

Modele AI ogólnego przeznaczenia są przydatne właśnie dlatego, że po przetworzeniu danych treningowych rozwijają szeroki zakres wiedzy i możliwości, ale niektóre typy danych treningowych w sposób nieproporcjonalny odpowiadają za rozwój potencjalnie niebezpiecznych zdolności. Na przykład model AI wytrenowany na publikacjach z wirusologii może lepiej potrafić udzielać wsparcia w potencjalnie szkodliwych zadaniach biologicznych (‡549, ‡1206*) (zob. też §2.1.4. Ryzyko biologiczne i chemiczne). Dodatkowo generatory obrazu/wideo trenowane na obrazach ludzkiej nagości mogą również zostać nadużyte do tworzenia niekonsensualnych intymnych deepfake’ów (‡308, ‡319) (zob. też §2.1.1. Treści generowane przez AI i przestępczość).

Filtrowanie danych treningowych jest skutecznym środkiem łagodzącym przeciwko niektórym niepożądanym zdolnościom (‡319, ‡1167, ‡1207, ‡1208). Jednak może być trudno filtrować duże zbiory danych wykorzystywane do trenowania modeli AI ogólnego przeznaczenia (‡1168) ze względu na wysokie koszty (‡1209), błędy filtrowania (‡1210) oraz negatywny wpływ na jakość zbioru danych (‡1211). Wyzwania te są potęgowane przez wielojęzyczny charakter tekstu internetowego (‡1212), uprzedzenia kulturowe w moderacji treści (‡1211, ‡1213, ‡1214, ‡1215) oraz fakt, że to, czy dana porcja danych jest „szkodliwa”, zależy od czynników kontekstowych (‡1216). Mimo to, filtrowanie potencjalnie szkodliwych materiałów z danych treningowych wykazuje obiecujące wyniki w zwiększaniu bardziej niezawodnego bezpieczeństwa modeli, w tym w czynieniu modeli z otwartymi wagami bardziej odpornymi na szkodliwe manipulacje (‡55). Zależności między zawartością danych treningowych a wyłaniającymi się zdolnościami modelu nie są jeszcze w pełni poznane (‡1195), a filtrowanie wydaje się być skuteczniejsze w ograniczaniu szkodliwych zdolności, gdy jest stosowane do szerokich dziedzin wiedzy (‡55), w porównaniu do węższych zachowań (‡1206, ‡1217). Patrz §3.4. Modele z otwartymi wagami, aby uzyskać dalszą dyskusję.

![figure 3.6](images/fig3.6_safeguards.png)

##### Postać 3.6: Gdzie stosować zabezpieczenia techniczne
>white|black||9|11|br Zabezpieczenia techniczne można stosować na różnych etapach tworzenia modelu. Dbałość o jakość danych kształtuje to, czego modele uczą się podczas pre-training i fine-tuning. Metody oparte na treningu, takie jak reinforcement learning from human feedback oraz robustness training, dostrajają zachowanie modelu. Metody testowania, takie jak ataki adversarial, identyfikują pozostałe podatności. Niektóre techniki, takie jak algorytmy safe-by-design, obejmują wiele etapów. Źródło: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Metody trenowania ogólnodostępnych modeli AI, aby były pomocne i nieszkodliwe, w dużej mierze opierają się na informacji zwrotnej od ludzi

Trudno jest trenować i oceniać modele w sposób niezawodny, aby zgodnie z wysokopoziomowymi zasadami były pomocne, nieszkodliwe i prawdomówne. W praktyce programiści dążą do osiągnięcia tego, dostrajając modele AI za pomocą demonstracji oraz informacji zwrotnych od ludzi. Na przykład główny paradygmat dostrajania modeli AI, znany jako „reinforcement learning from human feedback”, polega na trenowaniu modeli tak, aby generowały wyjścia, które ludzcy adnotatorzy oceniają pozytywnie (‡1218). Jednak pozytywna informacja zwrotna od ludzi jest wadliwym przybliżeniem zachowania korzystnego (‡737, ‡878, ‡1219, ‡1220) i jest ograniczona przez błędy oraz uprzedzenia człowieka (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Powoduje to kilka wyzwań: modele dostrojone poprzez uczenie ze wzmocnieniem z uczeniem z opinii ludzkich czasem pochlebiają użytkownikowi, zachowanie znane jako „sycophancy” (‡358, ‡740, ‡1226, ‡1227); dostarczają odpowiedzi, które w niektórych kontekstach są pomocne, ale w innych szkodliwe (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); dostarczają odpowiedzi trudnych do oceny pod kątem poprawności (‡1233); lub wykonują działania, których użyteczność bądź szkodliwość jest kwestią opinii (‡1234). Tabela 3.7 przedstawia przykłady tych wyzwań. Część badań dąży do opracowania metod, które pomagają ludziom lepiej oceniać rozwiązania złożonych zadań przy asyście AI (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Jednak obecnie metody te mają ograniczoną niezawodność, a skala, w jakiej są wykorzystywane do trenowania dziś najbardziej zaawansowanych modeli AI, nie jest publicznie znana.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sycofancja/dworne pochlebstwo (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Wyjaśnienie:
>white|black|left|11|13|br Model daje wyłącznie pozytywne opinie, nie wskazując braku poprawnej struktury sylabicznej 5-7-5 haiku.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Niektóre działania są pomocne w niektórych kontekstach, ale szkodliwe w innych (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Wyjaśnienie:
>white|black|left|11|13|br Informacje o ryzyku biologicznym mogą być wykorzystywane do edukacji i obrony, ale także do informowania złośliwych podmiotów.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Poprawne zachowanie jest trudne do zweryfikowania (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Wyjaśnienie:
>white|black||11|13|br Poprawność tej odpowiedzi trudno ocenić, ponieważ wymaga to wiedzy medycznej. Nawet doświadczony lekarz, oceniając takie odpowiedzi, musi poświęcić czas i zachować szczególną dbałość o szczegóły.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Ludzie nie zgadzają się co do tego, co jest poprawne (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Wyjaśnienie:
>white|black|left|11|13|br Ludzie w znacznym stopniu nie zgadzają się co do tego, jaka jest właściwa odpowiedź.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.7: Wpis użytkownika i odpowiedź modelu AI
>white|black||9|11|br Przykłady wyzwań związanych z określaniem i zachęcaniem do korzystnych działań podejmowanych przez modele AI.


>white|orangered|left|14|15.5|bb Ludzie nie zawsze zgadzają się co do tego, jakie zachowania są pożądane, co wymaga metod służących do równoważenia konkurujących preferencji.

Ludzie nie zawsze zgadzają się co do tego, jakie odpowiedzi lub działania modele AI powinny albo nie powinny generować (‡1006). Sprawia to, że opracowanie modeli, których działania i wpływ są w szerokim stopniu zgodne z interesami społeczeństwa, jest z natury rzeczy zasadniczo trudne (‡420). Niektórzy badacze analizują, czyje preferencje znajdują odzwierciedlenie w systemach AI (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) oraz pracują nad rozwojem technik „pluralistycznego dopasowania” (pluralistic alignment), których celem jest osiągnięcie równowagi między współzawodniczącymi preferencjami (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Na przykład twórcy systemów AI mogą zaprojektować rozwiązania tak, aby unikały generowania kontrowersyjnych odpowiedzi, odmawiając udzielenia odpowiedzi na niektóre żądania, albo dostosowując się do poglądu pośrodku (mediany) w pewnej istotnej próbie osób, albo personalizując systemy pod poszczególnych użytkowników.

Powszechnym wyzwaniem dla tych podejść jest to, że ogólnie rzecz biorąc systemy AI nie mogą równie dobrze dopasować się do preferencji wszystkich oraz że ich dalsze skutki społeczne będą w różny sposób oddziaływać na różne grupy ludzi. Niektórzy badacze twierdzą, że większość podejść technicznych do dopasowania pluralistycznego nie rozwiązuje, a potencjalnie odwraca uwagę od, głębszych wyzwań, takich jak systematyczne uprzedzenia, dynamika władzy społecznej oraz koncentracja bogactwa i wpływów (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Deweloperzy AI używają „treningu przeciwnikowego”, aby poprawić odporność modelu

Trudno jest zapewnić, że modele AI w sposób odporny i niezawodny przenoszą na środowiska rzeczywiste zachowania korzystne, które uczą się podczas treningu. Nawet modele trenowane z „doskonałym” sygnałem uczenia mogą nie zdołać skutecznie uogólniać do wszystkich nieznanych wcześniej kontekstów (‡738, ‡739, ‡1255, ‡1256, ‡1257). Na przykład niektórzy badacze stwierdzili, że chatboty częściej podejmują szkodliwe działania w językach, które są niedostatecznie reprezentowane w ich danych treningowych (‡159, ‡880, ‡1258*, ‡1259), obejmujących wiele języków używanych głównie w Globalnym Południu.

W ostatnich latach badacze stworzyli także obszerne narzędzie technik „ataku przeciwników” , które można wykorzystać do wymuszania na modelach generowania potencjalnie szkodliwych odpowiedzi (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Na przykład niedawna inicjatywa zebrała zlecenia zbiorowe (crowd-sourcing) obejmujące ponad 60,000 różnorodnych przykładów skutecznych ataków na modele AI będące na ówczesnym poziomie stanu techniki (state- of-the-art), co sprawiło, że zaczęły naruszać polityki swoich firm dotyczące akceptowalnego zachowania modeli (‡1149). Tabela 3.8 pokazuje przykłady technik „jailbreak”, które badacze wykazali jako zdolne do sprawiania, że modele spełniają szkodliwe żądania.

Jedną z metod poprawy odporności modeli jest znane jako „trening adversarialny” (‡1064). Polega on na konstruowaniu „ataków” (np. jailbreaków) zaprojektowanych tak, aby zmusić model do niepożądanego zachowania, oraz na trenowaniu modelu, aby właściwie radził sobie z takimi atakami. Jednak trening adversarialny jest niedoskonały (‡1260, ‡1261). Atakujący konsekwentnie potrafią opracowywać nowe skuteczne ataki wymierzone w modele najnowszej klasy (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Ponieważ twórcy potrzebują konkretnych przykładów trybów awarii, aby trenować przeciwko nim (‡512, ‡1263), rezultatem jest trwająca gra „kot i mysz”, w której twórcy nieustannie aktualizują modele w odpowiedzi na nowo odkryte podatności, a przeciwnicy nieustannie poszukują nowych ataków. Niektórzy badacze zaproponowali większoskalowy trening adversarialny (‡1264, ‡1265) lub nowe algorytmy (‡675, ‡676, ‡1263, ‡1266, ‡1267) w celu poprawy odporności, ale nowoczesne systemy AI pozostają uporczywie podatne.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Wykonuj szkodliwe żądania w szyfrowanym tekście, na przykład w kodzie Morse’a (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Zasiej system przykładami zgodnych odpowiedzi na szkodliwe prośby (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Wysyłaj szkodliwe prośby w językach o niskich zasobach, które prawdopodobnie są rzadziej wykorzystywane w treningu (np. suahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Podziel szkodliwe zadanie na wiele nieszkodliwych podzadań (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.8: Strategie jailbreakowania
>white|black||9|11|br Złośliwi aktorzy oraz zespoły red teams wykorzystywały różne typy „jailbreaków”, aby zmusić modele AI do spełniania szkodliwych żądań, które normalnie odmawiałyby ze względu na zabezpieczenia. Przykładowe wyniki zostały napisane przez autorów raportu wyłącznie do celów ilustracyjnych. Wiele obecnie najnowocześniejszych modeli AI odmawia już większości tych metod, jednak nadal odkrywane są nowe techniki jailbreakingu.


>white|orangered|left|14|15.5|bb Techniki „oduczenia” mogą łagodzić określone szkodliwe możliwości modelu

Inna strategia łagodzenia ryzyk wynikających z ogólnego zastosowania AI polega na dostrajaniu modeli w taki sposób, aby nie posiadały możliwości w określonych obszarach o wysokim ryzyku (‡1175, ‡1176). Na przykład badacze pracują nad opracowaniem algorytmów „machine unlearning” (masowego zapominania), które mogą konkretnie tłumić zdolności związane z zagrożeniami bioterrorystycznymi lub generowaniem fotorealistycznych obrazów nagich ludzkich ciał (‡903, ‡1272, ‡1273). Metody te mogą znacząco zwiększać bezpieczeństwo modeli, kosztem ograniczenia niektórych pozytywnych zastosowań zdolności podlegających „unlearning”. Ograniczanie wiedzy modeli AI w szkodliwych domenach zostało również zaproponowane jako sposób projektowania „tamper-resistant” modeli open-weight, które mogą opierać się szkodliwemu fine-tuningowi (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Jak dotąd jednak było to trudne do realizacji w sposób solidny (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Zob. §3.4. Modele open-weight w celu dalszego omówienia.

>white|orangered|left|14|15.5|bb Niektórzy badacze pracują nad metodami zapewniania silniejszych gwarancji bezpieczeństwa poprzez interpretowanie wewnętrznych stanów modelu lub weryfikację matematyczną

Niektórzy badacze pracują nad metodami bardziej rygorystycznego weryfikowania właściwości bezpieczeństwa modeli. W jednym podejściu badacze dążą do interpretowania wewnętrznych obliczeń modeli, aby albo zidentyfikować ryzyka, albo przedstawić bardziej przekonujące argumenty, że model jest bezpieczny (‡1285, ‡1286). Na przykład w demonstracji koncepcji badacze pokazali, że narzędzia do analizy wewnętrznych obliczeń modelu językowego mogą pomóc ewaluującym w identyfikowaniu szkodliwych zachowań (‡1287). W 2025 roku Anthropic również rozpoczął analizę wewnętrznych elementów modelu jako sposób badania jego świadomości sytuacyjnej i „intencji” (‡2). Jednak tego typu metody obecnie nie są powszechne ani nie są znane jako konkurencyjne wobec innych technik oceny.

Inne podejście do zapewniania silniejszych gwarancji bezpieczeństwa polega na konstruowaniu dowodów matematycznych, że model spełni określone warunki bezpieczeństwa (‡1177, ‡1282, ‡1288). Jednak te dowody zakładają, że kontekst testowania odpowiada kontekstowi wdrożenia i nie są testowane względem wielu typów przeciwników.

Obecnie nie można ich również jeszcze skalować do dużych modeli. Ogólnie rzecz biorąc, wśród ekspertów toczy się znaczna dyskusja dotycząca obietnicy interpretowalności oraz metod formalnej weryfikacji.

###@ Monitorowanie i kontrola w czasie wdrożenia

Oprócz zabezpieczeń wdrożonych podczas opracowywania modelu, drugim poziomem obrony przed szkodliwymi zachowaniami są zabezpieczenia zewnętrzne, które koncentrują się na monitorowaniu i kontrolowaniu działań modelu lub systemu podczas wdrożenia. Takie zabezpieczenia pomagają ograniczać nieprawidłowe działanie i nadużycia, takie jak zmyślone odpowiedzi i szkodliwe instrukcje.

>white|orangered|left|14|15.5|bb Wdrażający modele mogą korzystać z różnych narzędzi, aby identyfikować i przeciwdziałać zachowaniom modeli o wysokim ryzyku

Gdy system AI działa, wdrażający może monitorować oznaki ryzyka i interweniować, jeśli się pojawią. Na przykład mogą sprawdzać wejścia modelu pod kątem oznak ataków adwersaryjnych, filtrować nieodpowiednie treści z wyjść lub monitorować systemowy łańcuch rozumowania pod kątem oznak szkodliwych planów. Miejsca, w których wdrażający mogą monitorować i interweniować w sposobie, w jaki ludzie używają ich systemów, obejmują sprzęt (‡1180, ‡1181), interakcje z użytkownikami (‡1154, ‡1166), wejścia i wyjścia (‡65, ‡725, ‡1182), obliczenia wewnętrzne (‡744, ‡1183, ‡1184) oraz łańcuch rozumowania (‡430, ‡435). Istnieją również różne działania, które wdrażający mogą podjąć, gdy zidentyfikowane zostaną ryzyka. Obejmują one rejestrowanie informacji, filtrowanie/modyfikowanie szkodliwych treści, oznaczanie nieprawidłowej aktywności, wyłączanie systemu lub uruchamianie mechanizmów awaryjnych. Postać 3.7 przedstawia przykłady powszechnych mechanizmów monitorowania i kontroli.

Ponieważ te mechanizmy są wszechstronne i często skuteczne, są powszechnie stosowane i mogą zapobiegać wielu rodzajom niezamierzonych szkód (‡725, ‡751, ‡1289). Jednak te zabezpieczenia są niedoskonałe, zwłaszcza w warunkach złośliwych ataków zoptymalizowanych pod kątem tego, aby spowodować ich niepowodzenie (‡752, ‡1182). Nowe badania badały również, w jaki sposób monitorowanie może być zawod­ne, jeśli system jest optymalizowany przy użyciu wyników monitora, na przykład poprzez czynienie rozumowania krok po kroku mniej niezawodnym (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Postać 3.7: Techniki monitorowania i kontroli
>white|black||9|11|br Techniki monitorowania i kontroli działają w wielu punktach: przesiewanie wejść i wyjść pod kątem szkodliwych treści, śledzenie wewnętrznych stanów modelu, ograniczanie zewnętrznych działań poprzez piaskownice (sandboxing) oraz utrzymywanie nadzoru człowieka. Źródło: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Ludzie w pętli umożliwiają bezpośredni nadzór w środowiskach o wysokiej stawce

Aby zmniejszyć ryzyko niepowodzeń ze strony agentów AI (zob. §2.2.1. Wyzwania niezawodności), wdrażający mogą dążyć do projektowania systemów AI, które współpracują z ludźmi, zamiast działać w pełni autonomicznie (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Jest to ważne w przypadkach użycia, w których błędne decyzje mogą prowadzić do znacznych szkód, takich jak w finansach, ochronie zdrowia lub w działaniach policyjnych. Jednak posiadanie „człowieka w pętli” jest często niepraktyczne. Czasami podejmowanie decyzji zachodzi zbyt szybko, jak w aplikacjach czatu obsługujących miliony użytkowników. W innych przypadkach uprzedzenia i błędy człowieka mogą potęgować ryzyko na skutek błędów skumulowanych (‡1187). Ludzie w pętli często wykazują też „błąd uprzedzenia do automatyzacji”, co oznacza, że zwykle pokładają większe zaufanie w systemie AI, niż jest to uzasadnione (‡1190, ‡1191) (zob. §2.3.2. Ryzyka dla autonomii człowieka).

>white|orangered|left|14|15.5|bb „Sandboxing” chroni przed ryzykami wynikającymi z autonomicznych zachowań

Agenci AI zdolni do autonomicznego działania bez ograniczeń w sieci lub w świecie fizycznym stwarzają podwyższone ryzyko (zob. §2.2.1. Wyzwania niezawodności). „Sandboxing” polega na ograniczaniu sposobów, w jakie agenci AI mogą bezpośrednio oddziaływać na świat, dzięki czemu znacznie łatwiej jest ich nadzorować i zarządzać nimi (‡640, ‡1192, ‡1295). Na przykład ograniczenie zdolności systemu AI do publikowania w internecie lub edycji systemu plików komputera może zapobiec nieoczekiwanym szkodom wynikającym z nieoczekiwanych działań (‡1296). Jednakże podejścia te nie zawsze można stosować w aplikacjach, w których system AI musi koniecznie działać bezpośrednio w świecie.

###@ Narzędzia do monitorowania ekosystemu: model i pochodzenie danych

Narzędzia do modelowania i pochodzenia danych to narzędzia techniczne do badania ekosystemu AI, aby zwiększać świadomość dotyczącą dalszych zastosowań i skutków systemów AI.

>white|orangered|left|14|15.5|bb Techniki proweniencji systemów AI pomagają prześledzić zastosowania i wpływ systemów

Deweloperzy i wdrażający mogą wykorzystywać różne techniki do badania użycia modeli i rozprzestrzeniania ich „w dzikiej przyrodzie”. Na przykład mogą nadawać modelom unikalne zachowania identyfikujące (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) albo stosować unikalne wzorce do wag pojedynczych modeli z otwartymi wagami (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Jednak uczynienie tych technik bardziej odpornymi na modyfikacje modelu pozostaje otwartym problemem (‡1195, ‡1196*). Badacze pracują również nad metodami „wnioskowania o dziedzictwie modelu” (‡1197, ‡1198, ‡1305, ‡1306), pomagając odpowiedzieć na pytania w rodzaju: „Czy model X był dostrojoną lub wyekstrahowaną (distilled) wersją modelu Y?”. Wreszcie, niektórzy deweloperzy dążą do opracowania protokołów i infrastruktury dla agentów AI, aby ułatwić identyfikację i weryfikację, gdy wchodzą w interakcje z zewnętrznymi systemami (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Postać 3.8: Watermarki osadzają niepostrzegalne zakłócenia w obrazach i dźwięku
>white|black||9|11|br Znaki wodne osadzają niezauważalne zakłócenia w obrazach i dźwięku, które umożliwiają identyfikację treści generowanych przez AI przez narzędzia do wykrywania. W tej Postać zarówno znaki wodne obrazu, jak i dźwięku zostały wyolbrzymione dla lepszej widoczności. Źródło: Chameleon (obraz) z Unsplash (‡1313*). Pozostałe elementy utworzone przez autorów Raportu. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Postać 3.9: Wskaźniki powodzenia ataku typu prompt injection
>white|black||9|11|br Wskaźniki skuteczności ataków typu prompt injection, zgłaszane przez twórców AI dla głównych modeli udostępnionych w okresie od maja 2024 do sierpnia 2025. Każdy punkt oznacza odsetek udanych ataków w ramach 10 prób wobec danego modelu, krótko po udostępnieniu. Zgłaszany wskaźnik skuteczności takich ataków spada w czasie, ale nadal pozostaje stosunkowo wysoki. Źródło: Zou i in. 2025 (‡1149), cytowane w Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb Techniki wykrywania treści generowanych przez AI pomagają monitorować rozprzestrzenianie się i skutki treści wytworzonych przez AI

Znak wodny, metadane i inne detektory treści tworzonych przez AI mogą pomóc badaczom śledzić i badać rzeczywisty wpływ treści tworzonych przez AI na świat rzeczywisty. 

Po pierwsze, watermarki danych to dyskretne, ale wyraźne wzorce wstawiane do cyfrowych nośników, które mogą kodować informacje o ich pochodzeniu (‡1199, ‡1200, ‡1201*). W przypadku tekstu zazwyczaj przyjmują postać subtelnych uprzedzeń w doborze słów i stylu (‡1308, ‡1309); w przypadku obrazów i wideo - subtelnych wzorów na pikselach (‡1310); a w przypadku audio - subtelnych wzorów w falach dźwiękowych (‡1311). Postać 3.8 przedstawia to.

Oprócz znaczników wodnych, treści generowane przez AI można również zapisywać w formatach plików, które przechowują metadane dotyczące sposobu ich wygenerowania. Na przykład wiele urządzeń mobilnych zapisuje pliki obrazu i dźwięku w formacie, który może przechowywać informacje o ustawieniach aparatu, czasie, lokalizacji itp. (‡1312). Podobne metadane mogą być użyte do przechowywania informacji o tym, czy dane zostały wygenerowane przez system AI. Podobnie jak odciski palców w kryminalistyce, znaczniki wodne i metadane mogą zostać zmanipulowane lub usunięte, ale mimo to są przydatne.

Badacze pracują również nad opracowaniem detektorów treści generowanych przez AI (‡1203, ‡1204, ‡1205*) w celu identyfikowania treści generowanych przez AI w środowisku rzeczywistym, nawet gdy nie są dostępne żadne znaczniki wodne ani metadane. Jednakże skuteczność tych technik identyfikacji jest ograniczona.

###@ Aktualizacje

Since the publication of the last Report (January 2025), progress has been made in developing AI systems with multiple effective layers of safeguards. As discussed in §3.2. Risk management practices, defence-in-depth is a core principle in risk management (‡1314). For example, AI systems that combine safety-trained models with input filters, output filters, and other content monitors are increasingly studied and deployed (‡32, ‡65, ‡1182*). Recent research has also shown that, while model developers have made progress in increasing robustness to attempts to bypass safeguards, attackers still succeed at a high rate (Tabela 3.9).

###@ Luki w dowodach

Potrzebnych jest więcej dowodów, aby pomóc badaczom zrozumieć i uwzględnić ograniczenia istniejących podejść. Stosowane są ulepszenia technicznych zabezpieczeń dla systemów AI, ale techniki te mają ograniczenia. Na przykład postęp w poprawie odporności w najgorszym przypadku systemów AI ogólnego przeznaczenia był powolny, a istnieją podstawowe ograniczenia co do tego, jak dokładnie modele z otwartymi wagami mogą być zabezpieczane i monitorowane (‡1195, ‡1315, ‡1316) (zob. też §3.4. Modele z otwartymi wagami). Tymczasem nie wszystkie techniczne zabezpieczenia są równie powszechne, równie skuteczne ani równie dobrze potwierdzone w świecie rzeczywistym. Na przykład trening przeciwnikowy jest obecnie prawie powszechnie stosowany w modelach na poziomie stanu techniki (‡64*, ‡677), natomiast techniki interpretowalności modelu i weryfikacji formalnej były dotąd rzadko używane w systemach produkcyjnych (‡1177, ‡1285).

###@ Wyzwania dla decydentów politycznych

Kluczowe wyzwania dla decydentów obejmują podjęcie decyzji, czy i w jaki sposób powinni wspierać badania, rozwój, ocenę oraz wdrażanie technicznych zabezpieczeń i metod monitorowania. Jest to trudne, ponieważ zrozumienie przez naukowców tego, jak najlepiej w praktyce zabezpieczać mechanizmy, nadal się rozwija, a najlepsze praktyki nie zostały jeszcze ustanowione. Na przykład różni deweloperzy stosują różne zabezpieczenia, a ich podejścia do ograniczania ryzyka technicznego szerzej także znacznie się różnią (‡1116). Wreszcie, istnienie skutecznych technicznych zabezpieczeń nie zapewnia samo w sobie bezpieczeństwa, ponieważ wdrożenie i implementacja mogą się różnić w zależności od deweloperów oraz kontekstów wdrożeniowych.

