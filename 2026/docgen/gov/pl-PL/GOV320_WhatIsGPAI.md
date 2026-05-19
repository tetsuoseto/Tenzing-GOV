###@ Czym są ogólnego przeznaczenia systemy sztucznej inteligencji?

Ogólnego przeznaczenia systemy AI to programy komputerowe, które uczą się wzorców z dużych ilości danych, umożliwiając im wykonywanie różnorodnych zadań, zamiast bycia wyspecjalizowanymi dla jednej konkretnej funkcji lub dziedziny (zob. Tabela 1.1). Aby tworzyć takie systemy, programiści AI przeprowadzają wieloetapowy proces, który wymaga znacznych zasobów obliczeniowych, dużych zbiorów danych i wyspecjalizowanej wiedzy (zob. Tabela 1.2). Zasoby obliczeniowe (często skracane do „compute”) są potrzebne zarówno do opracowywania, jak i wdrażania systemów AI; obejmują wyspecjalizowane układy scalone, a także oprogramowanie i infrastrukturę niezbędne do ich uruchamiania.† Ponieważ są trenowane na dużych, zróżnicowanych zbiorach danych, ogólnego przeznaczenia systemy AI mogą wykonywać wiele różnych zadań, takich jak streszczanie tekstu, generowanie obrazów czy pisanie kodu komputerowego. Ta sekcja wyjaśnia, w jaki sposób tworzy się ogólnego przeznaczenia systemy AI, czym są modele „reasoning” oraz w jaki sposób decyzje polityczne kształtują rozwój ogólnego przeznaczenia systemów AI.

    Notatka † -- Termin ‘compute’ może również odnosić się do pomiaru liczby obliczeń, jakie procesor może wykonać (zwykle mierzonego w operacjach zmiennoprzecinkowych na sekundę) lub konkretnie do samego sprzętu (takiego jak jednostki przetwarzania grafiki), który wykonuje te obliczenia.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Systemy językowe
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Polecenie A (‡3*)
- EXAONE 4.0 (‡4*)
- Gemini 3 Pro (‡5*)
- GLM-4.5 (‡6*)
- GPT-5(‡7*)
- Hunyuan-Large (‡8*)
- Kimi K2 (‡9*)
- Mistral 3.1 (‡10*)
- Qwen3 (‡11*)
- DeepSeek-V3.2 (‡12*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ generatory obrazów
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Obraz (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Generatory wideo
- Kosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Widzę 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotyka i systemy nawigacji
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Predyktory różnorodnych klas struktur biomolekularnych
- AlphaFold 3 (‡27)
- Wzmacniaj (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ agenci AI
- AlphaEvolve (‡31*)
- Agent ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- Naukowiec AI-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 1.1: Ogólne typy sztucznej inteligencji
>white|black||9|11|br Istnieje kilka różnych typów ogólnego przeznaczenia AI. W niniejszym Raporcie modele, które potrafią przewidywać informacje strukturalne dla zróżnicowanych klas cząsteczek, są uznawane za „ogólnego przeznaczenia” AI, ponieważ mogą być adaptowane do różnych zadań. Na przykład modele wytrenowane do przewidywania struktury białek mają zastosowanie do wielu innych zadań, takich jak przewidywanie interakcji białek, przewidywanie miejsc wiązania małych cząsteczek oraz przewidywanie i projektowanie cyklicznych peptydów (‡40).


>white|orangered|left|13|15|bb Uczenie głębokie stanowi podstawę ogólnego sztucznego intelektu

Badacze budują uniwersalne modele AI ogólnego przeznaczenia w procesie zwanym „deep learning”, który uczy modele na podstawie przykładów (‡41). W przeciwieństwie do inżynierii oprogramowania modele uczenia głębokiego uczą się wykonywać zadania na podstawie danych, zamiast polegać na ręcznie zapisanych instrukcjach. Przetwarzając duże ilości danych, takich jak obrazy, tekst lub dźwięk, modele te odkrywają sposoby reprezentowania tych danych, tworząc wewnętrzne reprezentacje wzorców (takich jak kształty, skojarzenia słów czy struktury dźwiękowe), które pomagają modelowi rozpoznawać zależności i generować wyniki zgodne z jego celem uczenia. Następnie wykorzystują te wyuczone wewnętrzne reprezentacje jako abstrakcyjne cechy do analizy nowych, podobnych danych i generowania wyników w tym samym stylu. Na przykład uniwersalny model AI wyszkolony na wystarczająco dużej liczbie przykładów romantycznej poezji angielskiej z XIX wieku może rozpoznawać nowe wiersze w tym stylu i wytwarzać nowy materiał w podobnym stylu.

Na bardziej szczegółowym poziomie uczenie głębokie działa poprzez przetwarzanie danych warstwami połączonych ze sobą węzłów informacji. Węzły te są często nazywane „neuronami”, ponieważ są luźno inspirowane neuronami w biologicznych mózgach („sieci neuronowe”) (Postać 1.1) (‡42).Gdy informacja przepływa z jednej warstwy neuronów do następnej, model stopniowo przekształca dane w bardziej abstrakcyjne reprezentacje jako zbiory wyuczonych cech – wzorców, które model automatycznie odkrył w danych, zamiast tych ręcznie zakodowanych. Na przykład w modelu do przetwarzania obrazów pierwsze warstwy mogą uczyć się wykrywania prostych cech, takich jak krawędzie lub podstawowe kształty, podczas gdy głębsze warstwy łączą te cechy, aby wyłonić bardziej złożone wzorce, takie jak twarze lub obiekty.

Cechy na wszystkich warstwach są odkrywane w procesie optymalizacji, który definiuje procedurę uczenia. Podczas treningu, gdy model popełnia błędy, algorytmy uczenia głębokiego dostosowują siłę różnych połączeń między neuronami, aby poprawić wydajność modelu. Siłę każdego połączenia między węzłami często nazywa się „wagą”. To warstwowe podejście nadaje uczeniu głębokiemu jego nazwę.

Uczenie głębokie okazało się bardzo skuteczne w umożliwianiu systemom AI wykonywania zadań, które wcześniej uznawano za trudne dla tradycyjnych, ręcznie programowanych systemów obliczeniowych oraz innych wcześniejszych metod AI opartych na logice symbolicznej lub regułach. Większość obecnie wiodących w stanie sztuki, ogólnego przeznaczenia modeli AI opiera się na określonej architekturze sieci neuronowych znanej jako „transformer” (‡43, ‡44). Transformatory wykorzystują mechanizm „uwagi” (‡45), który pomaga modelowi skupiać się na najbardziej istotnych fragmentach danych wejściowych podczas przetwarzania informacji, takich jak określanie, które słowa w zdaniu są najbardziej znaczące dla zrozumienia jego znaczenia. Ten konkretny sposób budowania modeli doprowadził do znacznych usprawnień w tłumaczeniu (‡43), przetwarzaniu języka naturalnego (‡46), rozpoznawaniu obrazów (‡47) oraz rozpoznawaniu mowy (‡48, ‡49), ostatecznie prowadząc do opracowania dziś najbardziej zaawansowanych modeli.

![fig1.1](images/fig1.1_neural_network.png)

##### Postać 1.1: Ilustracyjna reprezentacja „sieci neuronowej”
>white|black||9|11|br Dzisiejsze ogólnego przeznaczenia modele AI są oparte na tych sieciach, które są luźno inspirowane biologicznymi mózgami. Różne sieci mają różne rozmiary i architektury. Jednak wszystkie składają się z połączonych jednostek przetwarzających informacje zwanych „neuronami”, gdzie siły połączeń między neuronami są nazywane „wagami”. Wagi są aktualizowane podczas treningu na podstawie dużych ilości danych. Źródło: International AI Safety Report 2025 (‡50) (zmodyfikowane).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Postać 1.2: Schematyczna reprezentacja etapów rozwoju ogólnego AI o przeznaczeniu ogólnym
>white|black|left|9|11|br Międzynarodowy Raport Bezpieczeństwa AI 2026.


>white|orangered|left|13|15|bb Ogólnego przeznaczenia AI jest rozwijane etapami

Opracowanie ogólnego systemu AI wymaga wielu etapów, od początkowego trenowania modelu po monitorowanie i aktualizacje po wdrożeniu (Postać 1.2). W praktyce kroki te często nakładają się na siebie w sposób iteracyjny. Każdy etap wymaga innych nakładów zasobów (np. danych, pracy, mocy obliczeniowej) oraz innych technik, a niekiedy są one realizowane przez różnych programistów (Postać 1.2 oraz Tabela 1.2).

Na przykład wstępne trenowanie modelu na ogół wymaga dużych ilości mocy obliczeniowej i danych, przez co etap ten jest szczególnie wrażliwy na polityki wpływające na dostęp do zasobów obliczeniowych lub danych treningowych (‡51, ‡52). Podobnie przygotowywanie danych i niektóre metody dostrajania modelu obecnie obejmują duże ilości pracy ludzkiej przy wstępnym oznaczaniu danych (‡53). W związku z tym etap ten jest wrażliwy na zmiany kosztów pracy, polityk platform lub regulacji wpływających na transgraniczne ustalenia dotyczące zleceń.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Zbieranie danych i ich przygotowanie
> 
  Przed wytrenowaniem ogólnego modelu AI twórcy i specjaliści ds. danych gromadzą, czyszczą, selekcjonują i standaryzują surowe dane treningowe do postaci, z której model może się uczyć. Może to być proces pracochłonny. Zbiory danych treningowych stojące za najnowocześniejszymi modelami obejmują ogromną liczbę przykładów z całego internetu.
  Zespoły często opracowują wyrafinowane metody filtrowania, aby ograniczać szkodliwe treści, eliminować zduplikowane dane oraz poprawiać reprezentację w różnych obszarach i źródłach (‡54, ‡55). Pielęgnacja danych może również pomóc ograniczyć naruszenia praw autorskich i prywatności, usuwać przykłady zawierające niebezpieczną wiedzę, obsługiwać wiele języków oraz usprawniać dokumentację dotyczącą proweniencji danych (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Wstępne trenowanie (pierwszy etap trenowania)

  Podczas wstępnego trenowania twórcy dostarczają modelom ogromne ilości zróżnicowanych danych, aby zaszczepić szeroką bazę wiedzy i zrozumienie kontekstu. Proces ten tworzy „model bazowy”. Jest to wysoce wymagający pod względem danych i mocy obliczeniowej proces.

  Podczas wstępnego trenowania modele są narażane na miliardy lub biliony przykładów treści, takich jak obrazy, teksty lub dźwięk. Dzięki temu narażeniu model stopniowo odkrywa abstrakcyjne cechy służące do reprezentowania danych i uczy się, w jaki sposób te cechy są ze sobą powiązane, co pozwala mu rozumieć nowe dane wejściowe w kontekście. Ten proces wstępnego trenowania trwa tygodnie lub miesiące (‡59) i wykorzystuje dziesiątki lub setki tysięcy jednostek przetwarzania grafiki (GPU) albo jednostek przetwarzania tensorów (TPU) (‡60) – wyspecjalizowane układy komputerowe zaprojektowane do szybkiego wykonywania wielu takich obliczeń. Niektórzy programiści prowadzą wstępne trenowanie przy użyciu własnych zasobów obliczeniowych, podczas gdy inni korzystają z zasobów udostępnianych przez wyspecjalizowanych dostawców mocy obliczeniowej.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Trenowanie po treningu i dostrajanie (drugi etap treningu)

  „Post-training” dalej udoskonala model bazowy, aby zoptymalizować go pod kątem konkretnego zastosowania. Jest to proces umiarkowanie wymagający obliczeniowo i bardzo pracochłonny. Przesunięcie w kierunku wykorzystywania „danych syntetycznych” – sztucznie generowanych informacji naśladujących dane z rzeczywistego świata, ale tworzonych przy użyciu algorytmów lub symulacji – pomaga sprawić, że ten etap jest mniej pracochłonny.
  Uczenie po treningu obejmuje różne techniki dostrajania oraz inne modyfikacje. „Dostrajanie nadzorowane” polega na dalszym trenowaniu wytrenowanego modelu na określonych zbiorach danych w celu poprawy jego wydajności w danej dziedzinie (‡61, ‡62). Na przykład ogólnego przeznaczenia model można dalej trenować na dużym korpusie obrazów radiologicznych. „Uczenie ze wzmocnieniem” (RL) polega na poprawie wydajności modelu poprzez „nagadzanie” modelu (dostarczanie pozytywnego sprzężenia zwrotnego) za pożądane wyniki oraz „karaniu” modelu (dostarczanie negatywnego sprzężenia zwrotnego) za niepożądane wyniki. Ma dwie wyraźne podkategorie. „Uczenie ze wzmocnieniem z wykorzystaniem informacji zwrotnej od człowieka” polega na nagradzaniu wyników zgodnych z preferencjami człowieka i karaniu tych, które są z nimi niezgodne, na podstawie informacji zwrotnej od człowieka (‡63, ‡64*). „Uczenie ze wzmocnieniem z weryfikowalnymi nagrodami” (RLVR) jest stosowane do poprawiania wydajności modelu w zadaniach wymagających poprawności merytorycznej, takich jak generowanie matematyczne lub kodu. Deweloperzy zazwyczaj naprzemiennie stosują techniki uczenia po treningu i uruchamiają testy, aż wyniki pokażą, że model spełnia oczekiwane wymagania.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Integracja systemu

  Programiści łączą jeden lub więcej ogólnego przeznaczenia modeli AI z innymi komponentami, aby utworzyć „system AI”, gotowy do użycia. GPT-5 (na przykład) to ogólnego przeznaczenia model AI, który przetwarza tekst, obrazy i dźwięk, podczas gdy ChatGPT to ogólnego przeznaczenia system AI, który łączy kilka modeli o różnej wielkości i możliwościach z interfejsem czatu, przetwarzaniem treści, dostępem do sieci oraz integracją aplikacji, aby stworzyć działający produkt.
  Oprócz uruchamiania modeli AI, dodatkowe komponenty w systemie AI mają również na celu zwiększenie możliwości, użyteczności i bezpieczeństwa. Na przykład system może być wyposażony w filtr, który wykrywa i blokuje wejścia lub wyjścia modelu zawierające szkodliwe treści (‡65*). Deweloperzy coraz częściej wykorzystują też „rusztowanie” – dodatkowe oprogramowanie budowane wokół ogólnego modelu AI, które umożliwia planowanie z wyprzedzeniem, realizowanie celów i interakcję ze światem (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Wdrożenie i wydanie
  Wdrażanie to proces udostępniania zintegrowanego systemu AI do zamierzonego zastosowania. Deweloperzy i osoby wdrażające implementują systemy AI w rzeczywistych aplikacjach, produktach lub usługach. Deweloperzy mogą wdrażać systemy AI wewnętrznie (do własnego użytku) lub zewnętrznie (dla prywatnych klientów lub do użytku publicznego). Podczas wdrażania systemów AI zewnętrznie firmy często zapewniają użytkownikom dostęp za pośrednictwem internetowych interfejsów użytkownika lub interfejsów programowania aplikacji (API), które umożliwiają użytkownikom dostęp i uruchomienie systemu. Na przykład jedna firma może zaprojektować dedykowanego czatbota obsługi klienta, który jest zasilany przez ogólnego przeznaczenia system AI innej firmy.
  „wdrożenie systemu AI” oznacza udostępnienie modelu do rzeczywistego wykorzystania przy zintegrowanych narzędziach i interfejsach, natomiast „udostępnienie modelu” obejmuje udostępnienie innym modelu bazowego – albo jako open-weight (do pobrania parametry), albo jako closed-weight (wyłącznie dostęp przez API). Zob. §3.4. Modele open-weight.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Monitorowanie po wdrożeniu i aktualizacje

  Deweloperzy często zbierają i analizują opinie użytkowników, śledzą metryki wpływu i wydajności oraz wprowadzają iteracyjne usprawnienia, aby rozwiązywać problemy wykryte podczas rzeczywistego użytkowania (‡67). Usprawnienia są wprowadzane poprzez aktualizację integracji systemowych, często poprzez ciągłe dopracowywanie (continual fine-tuning) oraz udostępnianie modelom dostępu do zewnętrznych baz danych z (najnowszymi) faktami. Pozwala to utrzymywać duże modele AI w aktualnym stanie bez ponownego przeprowadzania pełnego procesu wstępnego trenowania (‡68*). Umożliwia to kumulowanie możliwości w kolejnych rundach trenowania przy zachowaniu stabilności i zmniejszeniu kosztów obliczeniowych.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 1.2: Ogólne etapy rozwoju AI do zastosowań ogólnych
>white|black||9|11|br Na każdym ogólnym etapie rozwoju sztucznej inteligencji model AI jest ulepszany do zastosowań następczych i ostatecznie wdrażany jako w pełni zintegrowany system AI, monitorowany oraz aktualizowany.


>white|orangered|left|13|15|bb Systemy rozumowania generują „łańcuchy myśli” podczas wnioskowania, aby poprawić wydajność

Wnioskowanie zachodzi, gdy ktoś używa modelu AI po jego wytrenowaniu. Na przykład, do wnioskowania dochodzi wtedy, gdy osoba prosi system AI o zaplanowanie wycieczki, a model leżący u jego podstaw wykorzystuje odpowiednie aspekty tego, czego się nauczył w zakresie geografii, transportu i kuchni, aby wygenerować plan podróży.

W ciągu ostatniej dekady postępy w możliwościach AI w dużej mierze wynikały z większych przebiegów treningowych; to znaczy ze zwiększania ilości mocy obliczeniowej używanej do trenowania modelu AI. Ostatnio jednak badacze osiągnęli więcej korzyści, pozwalając modelom przetwarzać informacje przez dłuższy czas oraz trenując je do generowania jawnych kroków rozumowania podczas wykonywania zadania (‡69*, ‡70). Systemy AI działające w ten sposób nazywa się „systemami rozumowania”, a pośrednie wyjaśnienia, przez które przechodzą podczas rozwiązywania problemu lub odpowiadania na pytanie, nazywa się „łańcuchami myśli”. Systemy rozumowania wymagają większych zasobów obliczeniowych w momencie użycia, aby generować te zaawansowane łańcuchy myśli (‡71, ‡72, ‡73, ‡74), a także większych zasobów podczas treningu, aby nauczyły się rozumować lepiej. W praktyce te możliwości rozumowania pozwalają systemom AI rozwiązywać bardziej złożone problemy, iteracyjnie dekomponując zadanie na mniejsze kroki. Tabela 1.3 przedstawia przykład systemu niewykorzystującego rozumowania oraz systemu rozumowania rozwiązujących to samo zadanie.

Systemy rozumowania osiągnęły duże przełomy w możliwościach w trudnych problemach. Na przykład w 2025 r. systemy rozumowania wyspecjalizowane do rozwiązywania zadań matematycznych, takie jak Google Gemini Deep Think oraz nieudostępniony, eksperymentalny model OpenAI, rozwiązały zadania Międzynarodowej Olimpiady Matematycznej (w zorganizowanym środowisku testowym) na poziomie równoważnym ludzkiej wydajności za medal złoty (‡75, ‡76). Systemy rozumowania wykazały znaczący postęp w dziedzinach formalnych, takich jak matematyka, łamigłówki logiczne i ustrukturyzowane pytania naukowe, gdzie rozumowanie krok po kroku może być w sposób jawny zweryfikowane (‡77). Jednak systemy rozumowania mogą również zawodzić, generując nieistotne, nieproduktywne lub powtarzalne łańcuchy toków myślowych (‡78, ‡79).

###@ Aktualizacje dotyczące metod szkolenia

Od czasu publikacji ostatniego Raportu (styczeń 2025) metoda szkoleniowa o nazwie „distillation” znacznie zwiększyła efektywność, z jaką niektóre modele mogą być dostrajane. Distillation polega na trenowaniu modelu „student” na wyjściach potężniejszego (zwykle większego) modelu „teacher”, dzięki czemu model student może bezpośrednio naśladować wyjścia modelu teacher (‡80). Na przykład DeepSeek opracował duży model o nazwie DeepSeek-R1, który doskonale radzi sobie z rozumowaniem typu chain-of-thought. R1 generował wyjścia z rozumowaniem, które następnie wykorzystano do dostrajania mniejszych modeli student, w tym DeepSeek-V3. DeepSeek-V3 zachowuje dużą część możliwości matematycznych, programistycznych i analizy dokumentów R1 oraz według doniesień był dostrajany za około $10,000 USD (chociaż nie podano kosztów jego pre-training) (‡81). Jest to prawdopodobnie o rzędy wielkości mniej niż koszt dostrajania podobnie zdolnych, większych modeli.

![table1.3](images/table1.3_example_reasoning.png)

##### Tabela 1.3: Przykład systemu nierozumującego (po lewej) w porównaniu do systemu rozumującego (po prawej)
>white|black||9|11|br Rozwiązując tę samą zagadkę, te przykłady są przerobione z prawdziwych odpowiedzi udzielanych przez systemy AI. System rozumowania poświęca więcej czasu i mocy obliczeniowej na „myślenie”, konstruując „chain of thought” przed podaniem ostatecznej odpowiedzi.

![figure.3](images/fig1.3_AI_agent.png)

##### Postać 1.3: Ilustracyjna reprezentacja agenta AI
>white|black||9|11|br Model AI (środek), który został skonfigurowany tak, aby iteracyjnie planować, rozumować i korzystać z narzędzi w celu realizacji zadań w świecie rzeczywistym. Źródło: International AI Safety Report 2026.


Distylacja może więc stanowić tani i skuteczny sposób, aby modele zyskały bardziej zaawansowane możliwości (‡82). Niektórzy badacze wykorzystali distylację do dostrajania bardzo zdolnych modeli, używając zaledwie 1,000 przykładów wygenerowanych przez modele stanu-sztuki (‡83). Ponieważ distylacja wymaga istniejącego wcześniej modelu-nauczyciela, nie można jej bezpośrednio użyć do podnoszenia możliwości modeli stanu-sztuki. Może jednak przyspieszyć upowszechnianie zaawansowanych możliwości AI, nawet w przypadku modeli z zamkniętym kodem źródłowym (‡84*).

Wraz z postępem technologicznym w zakresie „rozproszonego przetwarzania” oraz zdecentralizowanego trenowania (podejścia, w których programiści używają wielu procesorów, serwerów lub centrów danych współpracujących ze sobą w celu przeprowadzenia trenowania lub wnioskowania w AI (‡85, ‡86, ‡87)), stopień, w jakim wiele projektów rozwoju AI opiera się na dużej skali, scentralizowanej infrastrukturze obliczeniowej, został zmniejszony. Coraz częściej umożliwia to mniej zasobnym podmiotom rozwijanie i wdrażanie potężnych systemów.

###@ Aktualizacje dotyczące agentów AI

Odkąd ostatni Raport (styczeń 2025), postępy w tym, jak programiści łączą modele AI z narzędziami, umożliwiły rozwój coraz bardziej wydajnych agentów AI. Agenci AI są zaprojektowani do realizowania celów, które często użytkownicy określają w języku naturalnym. Aby osiągnąć te cele, otrzymują dostęp do narzędzi, takich jak pamięć, interfejs komputerowy i przeglądarki internetowe. Te narzędzia oraz kod używany do łączenia ich z modelem określa się jako „scaffolding”, i pomagają one agentom AI autonomicznie oddziaływać ze światem, tworzyć plany, zapamiętywać ważne szczegóły oraz realizować cele (‡88*, ‡89) przy znacznie mniejszym nadzorze lub wsparciu ze strony ludzi. Na przykład Manus AI to popularny agent AI, który potrafi automatyzować różne zadania, w tym wyszukiwanie w sieci Web, rozwój oprogramowania i zakupy online (‡90). Postać 1.3 przedstawia prosty przykład agenta AI składającego się z ogólnego modelu AI „brain”, który może iteracyjnie planować, rozumować oraz korzystać z narzędzi do pamięci, przeglądania sieci Web i obsługi komputera.

Infrastruktura cyfrowa dla agentów AI rozwija się (‡91), a oni stają się coraz bardziej powszechni w różnych branżach (‡92, ‡93, ‡94). Agenci AI zostały opracowane do zadań takich jak badania (‡37), inżynieria oprogramowania (‡95), sterowanie robotami (‡96) oraz obsługa klienta (‡97). Trwające badania i rozwój doprowadziły do tego, że agenci AI lub systemy wieloagentowe stają się stopniowo bardziej zdolne i bardziej autonomiczne. Badacze oszacowali, że złożoność zadań testowych oprogramowania, które agenci AI potrafią realizować, podwaja się mniej więcej co siedem miesięcy (zob. też §1.2. Bieżące możliwości) (‡98). Eksperci twierdzą, że coraz bardziej zdolne agenty AI będą prowadzić zarówno do znaczących szans, jak i ryzyk (‡99, ‡100*) (zob. §2.2.1. Wyzwania niezawodności).

###@ Luki w dowodach

Główne luki dowodowe dotyczące procesu rozwoju ogólnego systemu AI wynikają z braku publicznie dostępnych informacji na temat tego, w jaki sposób są one opracowywane. Niektórzy deweloperzy są bardzo transparentni w kwestii tego, jak rozwijają ogólne systemy AI (‡1, ‡101). Jednak ogólnie stopień publicznej i wiedzy decydentów politycznych na temat tego, jak większość zaawansowanych modeli jest rozwijana, zabezpieczana, oceniana i wdrażana, jest ograniczony. Dotyczy to szczególnie systemów AI wdrażanych wewnętrznie, które są wykorzystywane w firmach zajmujących się AI, lecz nie są używane ani rozumiane przez podmioty zewnętrzne (‡102, ‡103). Ta ograniczona widoczność zewnętrzna rodzi wyzwania dla przejrzystości i nadzoru. Różni badacze wskazywali na ograniczoną i niespójną przejrzystość w obszarze danych treningowych (‡104, ‡105, ‡106), ogólnych modeli AI (‡107, ‡108), agentów AI (‡92), ewaluacji (‡109), pipeline’ów rozwojowych (‡110) oraz bezpieczeństwa (‡111). Ograniczenia w zakresie ujawniania na zewnątrz czasami są konieczne, aby chronić tajemnice handlowe firm i własność intelektualną. Jednocześnie niska przejrzystość utrudnia niezależnym badaczom i decydentom politycznym analizowanie ogólnych modeli i systemów AI.


