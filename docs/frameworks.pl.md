# Wprowadzenie

Wymienione poniżej frameworki stanowią powszechnie stosowane podejścia do zarządzania specyficznym ryzykiem związanym z systemami sztucznej inteligencji. Pomagają one organizacjom przełożyć ogólne zasady dotyczące wiarygodnej, bezpiecznej i etycznej sztucznej inteligencji na ustrukturyzowane wytyczne, środki kontroli i praktyki obejmujące cały cykl życia sztucznej inteligencji — od projektowania i rozwoju po wdrażanie i monitorowanie. Ramy te wspólnie wspierają proces podejmowania decyzji, ocenę ryzyka, zarządzanie i zgodność z ewoluującymi oczekiwaniami regulacyjnymi i branżowymi w obszarach technicznym, operacyjnym i organizacyjnym.

## NIST’s AI Risk Management Framework (AI RMF)

Źródło: [https://www.nist.gov/itl/ai-risk-management-framework](https://www.nist.gov/itl/ai-risk-management-framework)

Dobrowolne, ogólne ramy mające na celu pomoc organizacjom w systematycznej identyfikacji, ocenie i zarządzaniu ryzykiem w systemach sztucznej inteligencji w całym cyklu ich życia. Kładą one nacisk na zarządzanie, przejrzystość, odpowiedzialność i wiarygodność.

✅ Zalety:

- Zapewniają kompleksowe wytyczne dotyczące zarządzania ryzykiem we wszystkich fazach cyklu życia sztucznej inteligencji.
- Są dobrze dostosowane do globalnych standardów, takich jak ISO i unijna ustawa o sztucznej inteligencji, co ułatwia zapewnienie zgodności z przepisami w wielu krajach.
- Promuje przejrzystość i odpowiedzialność, budując zaufanie i pewność interesariuszy.
- Jest elastyczny i można go dostosować do różnych sektorów i poziomów dojrzałości AI.

❌ Wady:

- Dobrowolność i brak certyfikacji – organizacje nie są zobowiązane do jego stosowania.
- Wytyczne wysokiego szczebla nie zawierają szczegółowych wskazówek operacyjnych („co” kontra „jak”).
- Wymagania dotyczące zasobów i wiedzy specjalistycznej mogą być uciążliwe, zwłaszcza dla małych zespołów.
- Wymaga dostosowania do konkretnych kontekstów; uniwersalne zastosowanie może wydawać się biurokratyczne.

## AI Controls Matrix (AICM)

Link: [https://cloudsecurityalliance.org/artifacts/ai-controls-matrix](https://cloudsecurityalliance.org/artifacts/ai-controls-matrix)

Szczegółowe ramy celów kontroli definiujące 243 kontrole bezpieczeństwa i zarządzania AI w 18 domenach, odnoszące się do norm takich jak ISO 42001, ISO 27001 i NIST AI RMF w celu wspierania bezpiecznego i odpowiedzialnego wdrażania AI.

✅ Zalety:

- Niezależny od dostawcy, kompleksowy zestaw kontroli dostosowanych do ryzyka i bezpieczeństwa AI.
- Odnosi się do wielu międzynarodowych norm, umożliwiając dostosowanie i gotowość do audytu.
- Pomaga wdrożyć zarządzanie poprzez konkretne cele kontroli.

❌ Wady:

- Duży i złożony – może być przytłaczający bez odpowiednich narzędzi lub zaawansowanej wiedzy specjalistycznej.
- Skupia się głównie na środowiskach chmurowych – może wymagać dostosowania do użytku lokalnego/brzegowego.
- Dojrzałość różni się w zależności od dziedziny i wytycznych – niektóre kontrole mogą nie zawierać szczegółowych przykładów dotyczących sztucznej inteligencji. 

## Google’s Secure AI Framework (SAIF)

Źródło: (https://safety.google/intl/en_in/safety/saif/)[https://safety.google/intl/en_in/safety/saif/]

Strategiczna struktura bezpieczeństwa zajmująca się ryzykiem związanym ze sztuczną inteligencją, takim jak naruszenie modelu, zatrucie danych i kwestie prywatności, poprzez integrację zasad bezpieczeństwa na etapach projektowania, rozwoju i wdrażania sztucznej inteligencji.

✅ Zalety:

- Nacisk na bezpieczeństwo dostosowany do rzeczywistych zagrożeń związanych ze sztuczną inteligencją/uczeniem maszynowym, takich jak zatrucie danych i manipulowanie nimi.
- Rozszerza zarządzanie sztuczną inteligencją poza zgodność z przepisami, obejmując również luki techniczne.
- Pomaga ujednolicić bezpieczeństwo z zarządzaniem ryzykiem produktowym i zasadami prywatności.

❌ Wady:

- Nie jest szeroko znormalizowane ani certyfikowane poza ekosystemem Google. (wnioskowane)
- Wysoki poziom — bardziej koncepcyjna mapa ryzyka niż pełne ramy kontroli.

## MIT AI Risk Repository

Źródło: (https://airisk.mit.edu)[https://airisk.mit.edu]

Wyselekcjonowane repozytorium udokumentowanych zagrożeń związanych ze sztuczną inteligencją, trybów awarii i wzorców łagodzenia ryzyka, wspierające badania i praktyki oceny ryzyka. (Ogólne źródło wiedzy na temat ryzyka związanego ze sztuczną inteligencją).

✅ Zalety:

- Zbiorcze informacje na temat ryzyka i udokumentowane przypadki awarii w świecie rzeczywistym.
- Przydatne do badań i porównawczych analiz ryzyka.

❌ Wady:

- Nie określa formalnych ram zarządzania ani kontroli.
- Nie zostało zaprojektowane jako standard zgodności.

## IBM AI Risk Atlas

Źródło: (https://ibm.github.io/ai-atlas-nexus/)[https://ibm.github.io/ai-atlas-nexus/]

Strukturalna taksonomia i baza wiedzy dotycząca ryzyka związanego ze sztuczną inteligencją, pomagająca organizacjom identyfikować, klasyfikować i planować działania łagodzące w całym cyklu życia sztucznej inteligencji.

✅ Zalety:

- Bogata taksonomia wspiera systematyczną identyfikację ryzyka.
- Praktyczna w ocenie ryzyka przedsiębiorstwa.

❌ Wady:

- Nie stanowi samodzielnej struktury zarządzania z mechanizmami kontroli.
- Może wymagać integracji z innymi standardami (ISO, NIST) w celu zapewnienia pełnej zgodności.

## MITRE ATLAS

Źródło: (https://atlas.mitre.org/matrices/ATLAS)[https://atlas.mitre.org/matrices/ATLAS]

Baza wiedzy o działaniach przeciwników, zawierająca katalog rzeczywistych taktyk, technik i procedur stosowanych do ataków na systemy AI, zaprojektowana w celu wsparcia działań zespołów red team, modelowania zagrożeń i testowania zabezpieczeń.

✅ Zalety:

- Dostarcza konkretnych technik przeciwników do praktycznych testów.
- Przydatna dla zespołów ds. bezpieczeństwa budujących proaktywne systemy obrony.

❌ Wady:

- Nie jest to ramy zarządzania ani zarządzania ryzykiem.
- Skupia się na zagrożeniach związanych z przeciwnikami, a nie na zgodności organizacyjnej.

## OWASP Top 10 for LLM Applications

Źródło: (https://owasp.org/www-project-top-10-for-large-language-model-applications/)[https://owasp.org/www-project-top-10-for-large-language-model-applications/]

Opracowana przez społeczność lista najczęściej występujących luk w zabezpieczeniach aplikacji LLM (np. wstrzyknięcie polecenia, ujawnienie poufnych informacji) wraz z wytycznymi dotyczącymi ich ograniczania.

✅ Zalety:

- Bardzo praktyczne i przyjazne dla programistów skupienie się na konkretnych lukach w zabezpieczeniach.
- Szeroko cytowane przez specjalistów ds. bezpieczeństwa.

❌ Wady:

- Wąski zakres — nie zapewnia holistycznego zarządzania ani zarządzania ryzykiem w całym cyklu życia.
- Musi być połączona z szerszymi ramami (np. NIST) w celu zarządzania ryzykiem związanym ze sztuczną inteligencją w przedsiębiorstwie.

## SAIL Framework

Źródło: (https://www.pillar.security/sail)[https://www.pillar.security/sail]

Ramy zapewnienia bezpieczeństwa dotyczące kontroli bezpieczeństwa w całym cyklu życia i zarządzania wdrożeniami sztucznej inteligencji.

✅ Zalety:

- Kładzie nacisk na praktyki bezpieczeństwa i zapewnienia bezpieczeństwa w całym cyklu życia.

❌ Wady:

- Mniej ugruntowane/znormalizowane w porównaniu z ramami NIST lub CSA.
- Wytyczne dotyczące wdrażania mogą być mniej dojrzałe.

## CAI (Cyber-AI) Framework

Źródło: (https://github.com/aliasrobotics/cai)[https://github.com/aliasrobotics/cai]

Struktura zorientowana na cyberbezpieczeństwo, skupiająca się na zagrożeniach związanych ze sztuczną inteligencją, wektorach zagrożeń i środkach zaradczych — zwłaszcza w przypadku robotyki i systemów autonomicznych.

✅ Zalety:

- Praktyczne skupienie się na rzeczywistych scenariuszach zagrożeń związanych ze sztuczną inteligencją.

❌ Wady:

- Niszowe podejście; nie jest to kompletna struktura zarządzania lub zgodności.
