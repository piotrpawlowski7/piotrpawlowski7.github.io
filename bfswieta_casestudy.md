## Case Study projektu pocztówki internetowej
**Opis projektu:** Celem projektu było zdigitalizowanie pocztówki świątecznej, którą firma dotychczas wysyłała na święta do swoich klientów.

**Wykorzystane technologie:** HTML, CSS, JavaScript
<br>

**Wykorzystane dodatkowe oprogramowanie:** Adobe Illustrator, Adobe Xd

**[Gotowa strona](https://piotrpawlowski7.github.io/bfswieta/), [kod strony](https://github.com/piotrpawlowski7/bfswieta/)**

### 1. Założenia projektu



- Przygotowanie prostej strony internetowej z przygotowanej pocztówki
- zakup i konfiguracja domeny
- deployment strony na serwerze
- po otwarciu strona ma być czerwona (jak na rewersie projektu), wraz z logotypem i akcentami świątecznymi
- wykorzystanie efektu parallaxy do przygotowanych grafik
- zapewnienie responsywności strony (Desktop+mobile)

Całość projektu wyglądała następująco:
<img class="lazyload" src="images/casestudy/kartka.png?raw=true"/>


### 2. Wyzwania
- Projekt graficzny nie był projektowany na potrzeby strony internetowej (niemożliwość zastosowania opływania wokół grafik, obszerność tekstów)
- Przygotowane grafki odbiegają od standardów projektowania webowego

Zakodzona pocztówka w tym formacie wyglądała następująco: [Wersja 1](https://piotrpawlowski7.github.io/bfswieta_v1/),
a jej kod jest dostępny [tutaj](https://github.com/piotrpawlowski7/bfswieta_v1). Został podjęte decyzji o częściowym redesignie.

### 3. Nowy projekt
- Na etapie ustaleń doszliśmy do kolejnych założeń: finalny efekt powinien być czysty, nowoczesny, przejrzysty; Konieczne było zerwanie z projektem graficznym pocztówki i zaprojektowanie całego rozwiązania na nowo.
- Czas. Nie było możliwości całkowitej zmiany przygotowanych grafik. Nowy projekt musiał mieć tę samą bazę, ale całkowicie nową otoczkę.
- Odejście od One Page Site na rzecz wdrożenia rozwiązania typu fullpage (z niewidzialnym scrollem), dzięki czemu dana sekcja zajmuje całą stronę i mamy większą kontrolę nad contentem. Wykorzystany został skrypt fullpage.js
- W związku z tym powstało poważne wyzwanie -> wykorzystany skrypt renderuje całą stronę po pierwszym wczytaniu,a kolejne strony są tylko odpytywane. Stanowi to wyzwanie na dalszym etapie dodawania animacji na stronie (animacje ładują się na etapie wczytywania, czyli kończą zanim "zjedziesz na dół")
- Koncepcja dalej utrzymana jest w tonie listu - pocztówki, przedstawione rozwiązania pasują do formatu i gotowych materiałów.

Dla należytej kolejności pracy wykonałem szkic w Adobe Xd, który wyglądał następująco i zawierał dodatkowe elementy:
- wykorzystanie grafiki z kieliszkami z projektu pocztówki (do zaanimowania na dalszym etapie)
- dalszy redesign treści - została podzielona na więcej akapitów; wyróżniono też nagłównki dla lepszego efektu wizualnego i lepszego przyswojenia dużej ilości treści

<img class="lazyload" src="images/casestudy/sketch_xd_2.png?raw=true"/>


### 4. Gotowa strona

Gotowa strona jeszcze bardziej wyeulowała w trakcie kodowania: 
- tekst podzielono na więcej bloków; więcej nagłówków zamiast samych paragrafów
- grafiki zajmują pełny oddzielny slajd (odejście od pierwotnego planu i koncepcji)
- wykorzystano gotowe animacje (animate.css) oraz napisano własne skrypty (css/js): zaanimowano otwarcie strony oraz zderzanie się w stanie ciągłym kieliszków, co podkreśla wyskakujące "Zdrówko!"; animację otrzymały pojawiające się grafiki.
- Do podkreślenia koncepcji listu wykorzystano animacje typu "typewriter" - efekt pisania. Dzięki temu strona stała się przyjemniejsza wizualnie. Ilość treści mniej przytłacza.

<img class="lazyload" src="images/casestudy/bf3.gif?raw=true"/>
<img class="lazyload" src="images/casestudy/bf_6.gif?raw=true"/>
<img class="lazyload" src="images/casestudy/bf_4.gif?raw=true"/>

**Wyzwania w projekcie:**
- przygotowanie plików graficznych do animacji (svg)
- zmiana koncepcji w trakcie realizacji oraz jednoczesna praca nad designem+kodem w wąskim przedziale czasu (dowiezienie przed świętami)
- wykorzystanie JavaScriptu do triggerowania animacji po pokazaniu slajdu na ekranie (domyślnie animacje były triggerowane po wpisaniu adresu)
- nienajlepsze wyświetlanie grafik na mobile'u (docelowo powinny zostać zakodowane oddzielnie)

**Całą stronę można obejrzeć [tutaj](https://piotrpawlowski7.github.io/bfswieta/),
a jej kod jest dostępny [tutaj](https://github.com/piotrpawlowski7/bfswieta/)**

<script src="lazysizes.min.js" async=""></script>
