##########
>white|orangered|left|14|30|hr Sekcja 3.4
### 3.4. Modele open-source
>white|orangered|left|24|30|hb Modele z otwartymi wagami

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Kluczowe informacje
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Poziom dostępu, jaki firmy AI zapewniają do „wag” swoich modeli, wpływa na ryzyka, jakie te modele stwarzają. Wagi to parametry matematyczne umożliwiające modelom AI przetwarzanie danych wejściowych i generowanie wyjść. Dla dowolnego modelu firmy mogą zdecydować się na utrzymanie wag w pełnej tajemnicy, udostępnienie części użytkowników w ograniczonym zakresie lub umożliwienie każdemu pobrania ich w całości. Modele, których wagi są powszechnie dostępne, nazywa się „modelami open-weight”.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Modele z otwartymi wagami ułatwiają badania i innowacje, ale ich zabezpieczenia mogą być łatwiej usuwane. Na całym świecie różni aktorzy – zwłaszcza ci, którzy dysponują mniejszymi zasobami – mogą wykorzystywać modele z otwartymi wagami do celów badawczych i komercyjnych. Jednak w porównaniu do modeli z zamkniętymi wagami modele z otwartymi wagami są łatwiej modyfikowane, aby wykazywać potencjalnie szkodliwe zachowania, a ich kontrola jest trudniejsza.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Udostępnianie modeli o otwartych wagach jest nieodwracalne. Po udostępnieniu nie można przywrócić wag modelu. Utrudnia to łagodzenie potencjalnych szkód wynikających z udostępnienia modelu o niebezpiecznych możliwościach.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Od czasu publikacji ostatniego Raportu (styczeń 2025) duże wydania o otwartych wagach zmniejszyły lukę w możliwościach w porównaniu z wiodącymi modelami zamkniętymi. Chińscy deweloperzy DeepSeek i Alibaba wydali odpowiednio swoje modele R1 i Qwen, które osiągnęły wyniki porównywalne z wiodącymi modelami zamkniętymi, podczas gdy OpenAI opublikowało pierwsze modele o otwartych wagach od 2019 roku. Szacuje się obecnie, że możliwości wiodących modeli zamkniętych są o mniej niż jeden rok przed możliwościami wiodących modeli o otwartych wagach w kluczowych benchmarkach dla AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Kluczowym wyzwaniem polityki publicznej jest uzyskanie korzyści, jakie zapewniają modele o otwartej wadze, przy jednoczesnym zarządzaniu ich charakterystycznymi ryzykami. Jednym ze sposobów jest ocena modeli o otwartej wadze w kategoriach ich „ryzyka krańcowego”: w jakim stopniu ich udostępnienie w ujęciu kontrfaktycznym zwiększa społeczne ryzyko ponad to, które jest już stwarzane przez istniejące modele lub inne technologie. Jednak w praktyce jest to skomplikowane. Niewielkie wzrosty ryzyka krańcowego w czasie mogą również sumować się do znacznych wzrostów łącznego ryzyka.
>oldlace|black||11|15|br      


Modele o otwartych wagach, których parametry są publicznie dostępne do pobrania, mają odrębne implikacje dla wielu wyzwań omawianych w poprzednich sekcjach. „Wagi” modelu AI zawierają kluczowe informacje, które umożliwiają mu generowanie użytecznych odpowiedzi dla użytkowników. Po opublikowaniu tych wag nie da się już ich wycofać: każdy może je pobrać, przeanalizować, zmodyfikować, udostępnić i używać na własnych komputerach lub kontach w chmurze. Gdy wagi są dostępne jawnie, inni mogą łatwiej budować na ich podstawie i modyfikować model, zaspokajając zróżnicowane potrzeby i napędzając innowacje (‡1317). Jednak dzięki temu samemu mechanizmowi użytkownicy działający w złej wierze mogą równie łatwo usuwać zabezpieczenia i modyfikować modele o otwartych wagach do szkodliwych zastosowań (‡1122, ‡1160). Pojawiło się zatem pytanie, czy niektóre modele o otwartych wagach powinny podlegać szczególnym wymaganiom (np. bardziej rygorystycznym testom przed udostępnieniem) czy, przeciwnie, powinny otrzymać szczególne zwolnienia (np. z wymogów dotyczących raportowania regulacyjnego) (‡1033).

###@ Tło modeli o otwartych wagach

>white|orangered||14|15.5|bb Modele o otwartym dostępie do wag mogą być, ale nie muszą być, modelami „open source”

Chociaż często określa się je jako „open source”, większość publicznie udostępnianych modeli dokładniej opisuje się jako „open-weight”. Dzieje się tak, ponieważ choć deweloperzy udostępniają wagi modelu, nie publikują powiązanego kodu treningowego ani zbiorów danych. Ponadto oprogramowanie typu open source zwykle charakteryzuje się dopuszczalnymi licencjami, które nakładają minimalne wymagania na podmioty działające dalej, które używają lub modyfikują oprogramowanie (‡1318). Na przykład modele Llama firmy Meta mają restrykcyjne warunki licencyjne i obejmują wyłącznie kod do wnioskowania, a nie kod treningowy, dlatego zazwyczaj nie uznaje się ich za open source (‡1319, ‡1320). Opcje udostępniania modeli istnieją w spektrum od w pełni zamkniętych do w pełni open source, przy czym w każdym punkcie występują odmienne kompromisy w zakresie ryzyka i korzyści (‡1086*, ‡1320, ‡1321). Tabela 3.9 opisuje te opcje.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Całkowicie zamknięte
  Użytkownicy nie mogą w ogóle bezpośrednio wchodzić w interakcję z modelem
  Przykłady: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Zdalny dostęp
  Użytkownicy mogą wchodzić w interakcje wyłącznie za pośrednictwem określonej aplikacji lub interfejsu, takiego jak aplikacja mobilnego chatbota
  Przykłady: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Dostęp do modelu przez API
  Użytkownicy mogą wysyłać zapytania do modelu za pośrednictwem kodu, umożliwiając użycie w aplikacjach zewnętrznych
  Przykłady: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Dostęp do API w celu dostrajania
  Użytkownicy mogą dostroić model do swoich konkretnych potrzeb
  Przykłady: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Otwarte wagi: wagi dostępne do pobrania
  Użytkownicy mogą pobrać model i uruchomić go na własnych komputerach
  Przykłady: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Wagi, dane i kod dostępne do pobrania z ograniczeniami dotyczącymi użytkowania
  Użytkownicy mogą pobrać i uruchomić model, a także kod do wnioskowania i szkolenia, jednak istnieją pewne ograniczenia licencyjne dotyczące jego użycia
  Przykłady: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Całkowicie otwarte: wagi, dane i kod dostępne do pobrania bez ograniczeń w użytkowaniu
  Użytkownicy mają pełną swobodę pobierania, używania i modyfikowania modelu, pełnego kodu oraz danych
  Przykłady: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabela 3.9: Opcje udostępniania modelu od w pełni zamkniętych do w pełni otwartych
>white|black||9|11|br Ilustracyjny przegląd opcji udostępniania modeli, od w pełni zamkniętych modeli (modele są prywatne i przechowywane wyłącznie do użytku zastrzeżonego) po w pełni otwarte i modele o otwartym kodzie źródłowym (wagi modeli, dane i kod są swobodnie i publicznie dostępne bez ograniczeń w zakresie użycia, modyfikacji i udostępniania). Modele mieszczące się w pierwszych czterech kategoriach są często określane jako „zamknięte”. Ta sekcja skupia się na trzech dolnych wierszach. Źródło: zaadaptowano z Bommasani, 2024 (‡1317).


###@ Korzyści i ryzyka

>white|orangered|left|14|15.5|bb Modele o otwartym dostępie do wag mogą być łatwiej dostosowywane i oceniane

Modele z otwartymi wagami oferują istotne korzyści dla badań, innowacji i dostępu. Jak omówiono w §1.1. Co to jest ogólna sztuczna inteligencja (AI)?, szkolenie modeli ogólnej sztucznej inteligencji jest niezwykle kosztowne – wiodące modele kosztują setki milionów dolarów, aby je opracować. Publiczne udostępnienie wag modelu umożliwia mniej zasobnym podmiotom odtwarzanie, badanie i rozwijanie istniejących systemów. Bez takiego dostępu społeczności w regionach o niskich zasobach ryzykują wykluczenie z korzyści, jakie niesie AI, co czyni otwarte wagi kluczowymi dla umożliwienia globalnego udziału większości w rozwoju AI (‡1322). Deweloperzy działający dalej w łańcuchu mogą dostrajać modele do różnorodnych zastosowań, na przykład dostosowując je do niedostatecznie obsługiwanych języków mniejszości lub optymalizując wydajność dla konkretnych zadań, takich jak sporządzanie dokumentów prawnych czy robienie notatek medycznych (‡1323, ‡1324*). W ten sposób modele z otwartymi wagami mogą umożliwić większej liczbie osób i społeczności korzystanie z AI oraz czerpanie z niej korzyści, niż byłoby to możliwe w innym przypadku (‡1325). W przypadku modeli, które nie są na tyle wystarczająco zdolne, aby były niebezpieczne, te korzyści mogą przeważać nad dodatkowym ryzykiem otwartego udostępniania wag, choć zależy to od tolerancji na ryzyko właściwych decydentów.

Udostępnienie wag otwartych rozszerza także grono programistów i badaczy, którzy mogą badać model, oceniać jego możliwości, testować podatności i iterować nad ulepszeniami (‡1326, ‡1327). Sprawia to, że istnieje większe prawdopodobieństwo wykrycia zarówno korzystnych zastosowań, jak i szkodliwych wad, choć nie jest to zagwarantowane (‡1328, ‡1329). Użytkownicy mogą również uruchamiać modele z wagami otwartymi na własnych urządzeniach, co pozwala im zachować kontrolę nad wrażliwymi danymi i uniknąć przesyłania ich do serwerów podmiotów trzecich.

Istnieją dodatkowe korzyści, gdy deweloperzy dzielą się informacjami, takimi jak dane treningowe, kod, narzędzia ewaluacyjne i dokumentacja, a także wagami modelu (‡1320, ‡1330, ‡1331, ‡1332*). Dzięki większej ilości informacji deweloperzy działający dalej w łańcuchu oraz inni badacze mogą lepiej zrozumieć modele typu open-weight i dostosować je do nowych zastosowań.

>white|orangered|left|14|15.5|bb Zabezpieczenia modeli o otwartym dostępie są łatwiejsze do usunięcia, co umożliwia potencjalne złośliwe wykorzystanie

Modele o otwartych wagach stwarzają również dodatkowe ryzyka, ponieważ ich zabezpieczenia są łatwiejsze do usunięcia. Chociaż zarówno modele o otwartych wagach, jak i modele zamknięte mogą mieć zabezpieczenia służące do odmawiania szkodliwych żądań użytkowników, te zabezpieczenia są znacznie łatwiejsze do usunięcia w przypadku modeli o otwartych wagach. Złośliwi aktorzy mogą dopracować (fine-tune) model w celu optymalizacji jego działania dla szkodliwych zastosowań, usunąć części kodu zaprojektowane w celu zapobiegania szkodliwemu wykorzystaniu lub cofnąć wcześniejsze dostrajanie bezpieczeństwa (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). W rezultacie otwarte wagi modeli mogą zaostrzać ryzyka nadużyć omawiane w §2.1. Ryzyka wynikające ze złośliwego użycia poprzez umożliwienie większej liczbie aktorów korzystania z istniejących możliwości i ich wzmacniania w celach złośliwych bez nadzoru (‡1122, ‡1315). Chociaż wielu użytkowników nie będzie mieć umiejętności ani motywacji, by usuwać zabezpieczenia w modelach o otwartych wagach, stanowią problem złośliwi aktorzy o silnej motywacji. Ponadto złośliwi aktorzy mogą również być w stanie wykorzystać modele o otwartych wagach do identyfikowania podatności w podobnych modelach zamkniętych (‡1055*). Tego typu wady trudniej jest wykryć, uruchamiając wyłącznie modele zamknięte, ze względu na większą kontrolę i działania monitorujące, które dostawcy modeli zamkniętych są w stanie wdrożyć.

>white|orangered|left|14|15.5|bb Udostępnianie wag modelu jest nieodwracalne

Gdy tylko wagi modelu będą dostępne do publicznego pobrania, nie ma możliwości przeprowadzenia hurtowego wycofania (rollback) wszystkich istniejących kopii. Platformy hostujące w internecie, takie jak GitHub i Hugging Face, mogą usuwać modele ze swoich platform, co utrudnia niektórym podmiotom (aktorom) znalezienie pobieranych kopii i stanowi istotną barierę dla wielu przypadkowych użytkowników o złośliwych intencjach (‡1339). Jednakże zaangażowani aktorzy nadal mogą uzyskiwać kopie, jeśli model został już pobrany i ponownie udostępniony (rehostowany) gdzie indziej albo zapisany lokalnie. Co więcej, deweloperzy działający w downstream, którzy integrują modele open-weight w swoich systemach, również dziedziczą wszelkie wady, takie jak podatności na ataki adwersarialne (‡1055) czy zdolność modelu do omijania systemów monitorowania (zob. §2.2.2. Utrata kontroli) (‡1315). W przeciwieństwie do modeli zamkniętych, w których hostowie mogą powszechnie wdrażać poprawki, twórcy modeli open-weight nie mogą zagwarantować, że aktualizacje zostaną przyjęte przez użytkowników.

###@ Aktualizacje

Od publikacji ostatniego Raportu (styczeń 2025) luka możliwości między wiodącymi modelami otwarto-ważonymi a modelami zamkniętymi uległa zmniejszeniu. Szczególnie istotni stali się chińscy deweloperzy jako dostawcy modeli otwarto-ważonych. W styczniu 2025 firma DeepSeek opublikowała swój model R1, który osiągnął wyniki porównywalne z OpenAI o1 na szeregu benchmarków (‡1340). Modele Qwen firmy Alibaba również zyskały na popularności, zajmując pozycję lidera dla modelu otwarto-ważonego w serwisie Chatbot Arena, szeroko stosowanym benchmarku wydajności, według stanu na sierpień 2025 (‡1341, ‡1342*). W sierpniu 2025 OpenAI opublikowało pierwsze modele otwarto-ważone od czasu wydania GPT-2 w 2019, gpt-oss-120b i gpt-oss-20b. Meta kontynuowała publikowanie modeli Llama z otwartymi wagami. Szacuje się obecnie, że możliwości wiodących modeli zamkniętych są mniejsze niż o rok w porównaniu z wiodącymi modelami otwarto-ważonymi na kluczowych benchmarkach AI (Postać 3.10).

###@ Luki w dowodach

Kluczowa luka dowodowa dotyczy rzeczywistej skuteczności rozwiązań technicznych służących zapobieganiu nadużyciom modeli o otwartych wagach. Badacze zaproponowali różne podejścia, aby uczynić modele odpornymi na manipulacje. Obejmuje to nowe techniki trenowania zaprojektowane tak, aby modele były odporne na szkodliwe modyfikacje (‡1276), filtrowanie szkodliwych treści z danych treningowych (‡55) oraz mechanizmy obrony przed jailbreakami (‡675, ‡676). Techniki te są obecnie wdrażane w rzeczywistych wydaniach dużych twórców. Na przykład OpenAI zastosowało część z tych technik w swoich modelach gpt-oss, raportując, że wersje poddane adversarial fine-tuning nie osiągnęły wysokich progów możliwości (‡1344*). Jednak badania wykazały, że złe podmioty mogą wyłączyć zabezpieczenia, przeucząc modele na szkodliwych przykładach (‡1345, ‡1346). Co więcej, nadal trudno jest wiarygodnie ocenić odporność zabezpieczeń, co sprawia, że ich skuteczność wobec ataków w środowisku rzeczywistym pozostaje niepewna (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Postać 3.10: Luka możliwości między wiodącymi modelami AI open-weight i modelami AI closed
>white|black||9|11|br Wyniki Epoch Capabilities Index (ECI) najlepszych modeli z otwartymi wagami (ciemnoniebieskie) i modeli zamkniętych (jasnoniebieskie) w czasie. ECI łączy wyniki z 39 benchmarków w jedną ogólną skalę możliwości. Najlepsze modele z otwartymi wagami pozostają w tyle o około rok względem modeli zamkniętych. Źródło: Epoch AI, 2025 (‡1343).


###@ Środki zaradcze

Techniczne środki łagodzące ryzyko modeli z otwartą wagą działają w całym procesie rozwoju i wdrażania sztucznej inteligencji (‡1141, ‡1195, ‡1347). Na przykład, gdy modele są opracowywane, programiści i adaptery dla odbiorców końcowych mogą filtrować treści wrażliwe z danych treningowych, aby zminimalizować szkodliwe możliwości. Usunięcie szkodliwych przykładów z danych treningowych modelu może zapobiegać złośliwemu dostrajaniu 10 razy skuteczniej niż obrony dodane po treningu, choć może to również wpływać na korzystne możliwości (‡55). Dostawcy aplikacji AI mogą również wdrożyć mechanizmy zgłaszania incydentów i reagowania na nie (‡1348).

Dodatkowo platformy hostingowe, takie jak HuggingFace i GitHub, mogą ustanawiać warunki świadczenia usług platformy w celu usuwania modeli modyfikowanych do celów szkodliwych (‡1141, ‡1324). Twórcy modeli mogą udostępniać pełny dostęp audytorom przed wydaniem albo zdecydować się na strategię „etapowego” udostępniania – udostępnianie modeli stopniowo coraz większym grupom (‡1086). Może to pomóc wykryć potencjalne nieprawidłowe działanie lub podatności, zanim model zostanie szeroko udostępniony (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Notatka 3.1: Bezpieczeństwo wag modelu
>oldlace|black|left|13|15|hb  Notatka 3.1: Zabezpieczenie wag modelu
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Ryzyka omówione w tej sekcji zakładają, że wagi modelu są udostępniane celowo. Jednak zamknięte wagi modelu mogą również stać się dostępne w wyniku kradzieży lub wycieku. Zamknięte modele kosztują setki milionów dolarów na opracowanie (§1.1. What is general-purpose AI?) i przeciętnie są bardziej zdolne niż modele o otwartych wagach (‡1343). Sprawia to, że są atrakcyjnymi celami dla podmiotów od amatorskich hakerów po państwa dążące do pozyskania wiodących modeli AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Skradzione zamknięte wagi modeli wiązałyby się z ryzykami podobnymi do tych opisanych powyżej dla modeli z otwartymi wagami, ale potencjalnie bez żadnych z zastosowanych zabezpieczeń. Złośliwi aktorzy mogliby usunąć mechanizmy ochronne z najbardziej zaawansowanych modeli. W przeciwieństwie do uprawnionych deweloperów, tacy aktorzy nie byliby ograniczeni reputacyjnymi, prawnymi ani komercyjnymi konsekwencjami, które obecnie motywują firmy z obszaru AI na poziomie frontier do bezpiecznego wdrażania swoich modeli.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Bieżące poziomy bezpieczeństwa różnią się w całej branży i mogą okazać się niewystarczające wobec wyrafinowanych atakujących. Część deweloperów deklaruje zabezpieczanie wag modelu przed zorganizowaną cyberprzestępczością i zagrożeniami ze strony insiderów (‡582), podczas gdy inni nie złożyli żadnych publicznych zobowiązań w zakresie bezpieczeństwa (‡1109, ‡1349). Badania wskazują, że centra danych AI mogą nie być w stanie wytrzymać ataków ze strony najbardziej wyrafinowanych i najlepiej dysponowanych podmiotów (‡582, ‡1350, ‡1351). Na grudzień 2025 roku nie ma potwierdzonych, publicznie udokumentowanych przypadków kradzieży wag modelu. Jednak zgłaszano inne naruszenia bezpieczeństwa w wiodących firmach AI, w tym przeniknięcie do systemów poczty Microsoft (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Zamknięcie tych luk w zabezpieczeniach wymagałoby znacznych nakładów na sprzęt, oprogramowanie, personel oraz bezpieczeństwo obiektów. Niektóre usprawnienia zabezpieczeń można wdrożyć stosunkowo szybko przy skoordynowanych działaniach (‡1122). Inne jednak krytyczne środki, takie jak zabezpieczenie łańcuchów dostaw sprzętu i obiektów, prawdopodobnie zajęłyby lata (‡1122). Prywatne firmy mogą również nie dysponować zasobami ani informacjami, aby samodzielnie opracować odpowiednie ochrony. Na przykład deweloperzy AI nie mają dostępu do sklasyfikowanych informacji o zagrożeniach, które mają rządy (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Wyzwania dla decydentów politycznych

Kluczowym wyzwaniem dla decydentów jest zapewnienie korzyści płynących z udostępniania modeli o otwartych wagach bez istotnego zwiększania ryzyka. Aby uniknąć katastrofalnej szkody, twórcy modeli o otwartych wagach nie powinni udostępniać modeli bez oceny ryzyk, zarówno z wykorzystaniem uznanych metod oceny stosowanych dla modeli zamkniętych, jak i dodatkowych testów, biorąc pod uwagę, że podmioty działające w złej intencji mogą dostrajać modele i usuwać zabezpieczenia bezpieczeństwa. W praktyce może to być trudne, ponieważ rozwój możliwości może być nieprzewidywalny, udostępnienia modeli o otwartych wagach są nieodwracalne, a działania ewaluacyjne są potrzebne, aby przewidzieć, kiedy udostępnienie może stanowić znaczące potencjalne zagrożenie. Jednym ze sposobów jest ocena „ryzyka krańcowego” udostępnień otwartych: w jakim stopniu udostępnienie kontrfaktycznie zwiększa ryzyko społeczne ponad ryzyko już stwarzane przez istniejące modele lub inne technologie (‡556, ‡1033, ‡1354, ‡1355) (zob. §3.2. Praktyki zarządzania ryzykiem). Jednak oszacowanie, w jaki sposób system będzie zwiększać lub zmniejszać ryzyko w kolejnych etapach po jego wdrożeniu, jest złożone i zależne od kontekstu. Przyrostowe zwiększanie ryzyka wraz z kolejnymi udostępnieniami może z czasem potęgować się i prowadzić do znacznych wzrostów całkowitego ryzyka, nawet jeśli ryzyko krańcowe związane z każdym udostępnieniem wydaje się akceptowalne (‡1356, ‡1357). Dwuzastosowanie zdolności AI dodatkowo komplikuje nadzór: cechy umożliwiające korzystne zastosowania w medycynie lub badaniach mogą zostać przerobione na wyrządzanie szkód, a gdy wagi są publiczne, odróżnienie zastosowań legalnych od złośliwych może być trudne. Nie jest też jasne, kto powinien ponosić odpowiedzialność, gdy modele o otwartych wagach są modyfikowane w celach szkodliwych.

