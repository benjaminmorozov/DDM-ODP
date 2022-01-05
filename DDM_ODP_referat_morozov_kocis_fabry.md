# Typografia webových stránok

**Autori**: Benjamín Morozov, Filip Kočiš, Ľubomír Fábry II.A

[@benjaminmorozov](https://github.com/benjaminmorozov), [@fifo260](https://github.com/fifo260), [@lubomirfabry](https://github.com/lubomirfabry)

**Predmet**: DDM-ODP

**Vypracované**: 14. 12. 2021

Na vypracovanie dokumentu boli použité nástroje **Visual Studio Code**, **Adobe Acrobat DC** a **doxygen** (1.9.2).

# Obsah

- **[Typy písma a texty](#typy-písma-a-texty)** - 2-3
  - Bezpätkové - 2
  - Pätkové - 2
  - Proporciálnosť písiem - 2
  - Koľko fontov by som mal použiť na jednej stránke? - 3
  - Dlhé vs krátke texty - 3
  - Maximálna úroveň nadpisov - 3
  - Pravidlá na písma - 3
- **[Rozloženie a prvky stránky](#rozloženie-a-prvky-stránky)** - 4-6
  - Z-pattern vs F-pattern - 4
  - Single page application - 4
  - E-shopy vs portfóliá - 4
  - Zlatý rez - 5
  - Malo by byť logo stránky klikateľné? - 6
  - Slider vs banner - 6
- **[Typografia webu vs tlačovín](#typografia-webu-vs-tlačovín)** - 6-7
- **[Responzívny web dizajn](#responzívny-web-dizajn)** - 7-8
  - Existujú nejaké pravidlá, ktoré by sme mali dodržiavať?  - 7
  - Ako by sa stránka mala meniť podľa typu média - 7-8
  - Zobrazenie podstatných sekcií - 8
- **[Optimalizácia obrázkov](#optimalizácia-obrázkov)** - 8-9
  - Rozlíšenie - 8
  - Veľkosť - 8
  - Použitie CDN v praxi - 8
- **[Farby a štýly](#farby-a-štýly)** - 9-10
  - UX vs UI - 9
  - Konzistentnosť štýlov a farieb - 9
- **[Základné pojmy](#základné-pojmy)** - 10-12
- **[Použitie frameworkov](#použitie-frameworkov)** - 13-14
  - Najobľúbenejšie PHP frameworky medzi vývojármi - 13-14
- **[Zdroje](#zdroje)** - 15

# Typy písma a texty

**Bezpätkové písmo**, v angličtine tiež **sans-serif** (sans znamená bez), je písmo **bez pätkov** (serifov). Jedná sa teda o **neokrasné bežné písma**, slúžiace na **kľudný čistý dizajn** bez akýchkoľvek **rušivých elementov**. V typografii sa pre ne používa aj slovo **grotesk**.

![Porovnanie serif a sans-serif](https://newenglandrepro.com/wp-content/uploads/2016/08/BP-Serif-SansSerif-Graphic1-862x518.jpg)

**Pätkové písmo**, v angličtine tiež **serif**, je písmo, ktoré naopak **obsahuje pätky**. Jedná sa o **krásne tradičné písma**, slúžiace na zvýraznenie **estetiky** v texte. Používajú sa zväčša na **citáty**, na text, používaný v **právnom zmysle**, a na **nadpisy**. Sú veľmi podobné tradičnému **ručne-písanému štýlu textu**.

**Proporciálnosť písiem** je jedna zo **základných vlastností** typografie. Hovorí o tom, že každé písmeno by malo mať svoje **vlastné proporcie**, teda šírku. V praxi ju je možné vysvetliť tak, že sa do každého riadku vmestí **iný počet** rôznych písmen.

mmmmmmmm - 8 písmen

llllllll - 8 písmen

**Poznáme teda:**
 - **neproporciálne písma** - každé písmeno má vyhradený rovnaký priestor, všetky znaky majú rovnakú šírku.
 - **proporciálne písma** - každé písmeno má rozdielnú šírku a voľný priestor. Takéto písma sa nám môžu zdať ľahšie čitateľné.

> “If there’s one thing you learn by working on a lot of different web sites, it’s that almost any design idea – no matter how appallingly bad – can be made usable in the right circumstances, with enough effort.” - Steve Krug

![Proporciálnosť písiem](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c5/Propvsmono.svg/220px-Propvsmono.svg.png)

Pri **dizajne webov** a iných grafických médií vzniká vždy u jeho autora otázka - **môžem použiť viac ako tri písma**? Kedy sa z textu stáva nekonzistentná obluda?
Neexistuje **žiadne pevne dané pravidlo**, ktoré by odpovedalo na túto otázku. V jednom texte by sme však **nemali prepínať medzi rôznymi písmami** a mali by sme byť konzistentní. Ak má jeden nadpis sans-serif font, tak aj ostatné nadpisy budú mať rovnaký font.
V praxi sa teda typicky využívajú **maximálne 3 fonty** za účelom zachovania **vernosti jednotného dizajnu**.

Autor by sa mal taktiež snažiť zachovať čo **najkratší text**, aby sa v ňom čitateľ nestratil. Je taktiež dôležité udržiavať **vety vždy čo najkratšie**, ako je možné, aby si čitateľ vetu **nemusel čítať 3krát**, len aby ju pochopil.

Dôležité je taktiež **zachovať čitateľnosť** aj na tých **najmenších zariadeniach**. Je teda dôležité **nevnucovať na malé obrazovky obrovské písma**, ktoré sa nebudú dobre škálovať.

Dôležité je na webových stránkach taktiež **používať veľkosti písiem**, ktoré budú ich **dôležitosť dostatočne reprezentovať**. Pre **nadpisy** sa väčšinou používa **najväčšie písmo**, pričom pre **texty**, poprípade **disclaimery**, sa používajú často tie **najmenšie písma**, s potrebou toho, zaistiť, aby bolo dané písmo stále čitateľné.

**Neexistujú žiadne pravidlá** na písma. Môžeme si dokonca urobiť **úplne vlastné**, no je dôležité na ne **odkázať**, aby ich bolo prehliadačom **možné stiahnúť**. Je **hlúpe** hovoriť, ako by font nemal obsahovať **takéto a takéto grafické prvky**, ako by nemal byť **takto a takto vysoký**, nakoľko je všetko práve na **autorovi grafického média**. Typografia je v podstate **druh elektronického umenia**.

![Typografia je v podstate druh elektronického umenia](https://www.shillingtoneducation.com/content-blog/uploads/2019/09/Typography_Anatomy.jpg)

# Rozloženie a prvky stránky

Jednou z **najväčších zaujímavostí** vo webovom dizajne je práve forma alebo spôsob, **ako si stránku čítame** a pozorujeme ju. Na stránkach, ktoré sú **plné informácií a obrázkov**, ktoré nás majú niečo naučiť a niečim zaujať, sa používa práve tzv. **F-pattern**, kedy čítame **riadok po riadku**, s tým, že sa vraciame na **rovnakú vertikálnu čiaru**, aby sme pokračovali v odstavci.

Existuje však aj tzv. **Z-pattern** spôsob čítania, ktorý sa používa na stránkach, ktoré majú čitateľa **zaujať skôr ich grafickým dizajnom**, ich prvkami a ich obrázkami. Čítame teda hlavne nadpisy, obrázky ale aj slidery a bočné panely. Na rovnakom princípe fungujú aj **sociálne siete**.

![F-pattern](https://99designs-blog.imgix.net/blog/wp-content/uploads/2016/07/heatmap-eye-tracking.jpg?auto=format&q=60&fit=max&w=930)

Medzi formu webových stránok a ich prijímania patrí aj tzv. **SAP**, teda single page application. Jedná sa o stránku, ktorá **nikdy nemení svoju URL adresu** a pracujeme v podstate s vždy rovnakým rozložením. Jej obsah je však **dynamicky tvorený** rôznymi server-side skriptmi. Príkladom je **Facebook,** ktorý na svoju hlavnú stránku **po obnovení vždy umiestni iné obrázky** a príspevky aj napriek tomu, že ich tam nikto ručne nevpísal.

Práve takéto **server-side skripty** sa používajú na **e-shopoch**, na ktorých aj hovoria o tom, ku ktorému **košíku** priradiť **aký tovar**, a k akému zákazníkovi priradiť akú **objednávku**. Takéto skripty **nie sú veľmi potrebné** na **osobných a personálnych portfóliách**, ktoré by mali byť **statické** a ich obsah by sa nemal na základe žiadneho používateľského vstupu nijako meniť.

Rozdielom medzi **e-shopmi** a **osobnými portfóliami** je taktiež použitie **rozdielnych sekcií**, ako je napríklad **použitie okrasných písiem** a **väčšia pravdepodobnosť** použitia **ikoniek a linkov** pre **sociálne siete** na **osobných portfóliach**, kdežto na webových stránkach typu **e-shop** je pravidelnejšie **použitie sekcií na vyhľadávanie** a **pop-upov**, ktoré informujú o **novinkách** v katalógu.

![Facebook](https://cdn.vox-cdn.com/thumbor/IdBI4T4fH6vebzkYAz7JqkdSylE=/1400x1050/filters:format(jpeg)/cdn.vox-cdn.com/uploads/chorus_asset/file/19954379/NRP_the_new_facebook.com_final_1.jpg)

**Zlatý rez** nám hovorí o nejakom **myslenom vedomí dôležitosti prvkov na základe ich rozmiestnenia a veľkosti**. **Najdôležitejšie prvky** by mali byť na stránke rozmiestnené čo **najbližšie používateľovi** s tým, že akékoľvek ďalšie a **nepodstatné informácie** by mali byť vzhľadovo **menšie** a menej-prepracované ako ta hlavná.

![Zlatý rez](https://blueweb.bwcdn.net/media/2021/08/1/4/7.png)

Jedným zo **základov webového dizajnu** je aj **user experience**. Používateľovi by **malo byť na pohľad jasné**, čo aké tlačidlo robí **bez toho**, aby ho musel **najprv vyskúšať**. Pre čitateľa je teda samozrejmé, že ak klikne na **logo stránky**,** tak by ho malo **zaviesť na nejakú centrálu**, teda hlavnú stránku, zameranú práve na danú značku.

Na internete v posledných rokoch vzniká zaujímavá senzácia menom **slider**. Jedná sa o **typ banneru** (statická časť webu, ktorá zobrazuje najdôležitejšie informácie na jednom mieste), ktorý je **spracovaný formou galérie**. Dokáže teda zobraziť oveľa viacej informácií ako jeho náprotivok.

# Typografia webu vs tlačovín

Zaujímavosťou je práve **podobnosť medzi papierovým a elektronickým médiom**. Obe formy **predávajú informácie** rovnakým spôsobom - **čítaním** (ak nepočítame videá a audionahrávky). Problém však vzniká v ďalšej interakcii. **Tlačoviny** sú tzv. **dvojdimenzionálne médium**. To čo máme proste máme a aj keby sme papier otáčali a otvárali koľkokrát by sme len chceli, nič by sa na ňom nezmenilo. Naopak, u **webových/elektronických médií** je možné **jediným klikom prejsť** z noviniek o športe na vtipné videá psov. **Navigácia** je taktiež oveľa jednoduchšia, nakoľko nám **stačí stlačiť jedinú skratku** - <span style="background-color: #333; color: white">⠀Ctrl+F⠀</span> - a môžeme sa **dostať priamo k informácii**, ktorú hľadáme, kdežto ak si kúpime encyklopédiu o zvieratách len za účelom toho, aby sme si prečítali o tom, koľko nôh má žirafa, tak by sme si pravdepodobne **museli knihu prečítať celú**.

![Ctrl+F](https://community-assets.home-assistant.io/original/3X/7/0/707984acd98a5c848bb2cbbeb1b26767c5273dbe.png)

Problém však vzniká v tom, že **nikdy nevieme**, **ako** môže používateľ **prijímať** danú web-stránku. Nech ju prijíma **na smartfóne**, na počítači alebo na bankomate, stránku **musíme prispôsobiť** na úplne **každú možnú veľkosť** a médium, aké len ide. Dizajnéri a programátori tak dostávajú **zbytočne prácu navyše**, nakoľko musia vymýšľat zaujímavé spôsoby, ako na hodinky vtiesniť všetok text, ktorý je potrebný. Naopak, **u papierového média** stačí text **navrhnúť raz** a vždy bude vytlačený **rovnakým spôsobom**.

![Tlačený dizajn](https://wenceslau-nd.com/wp-content/uploads/2020/09/Domani_Print_09_Wenceslau_News_Design-1.gif)

Vzniká tu taktiež problém toho, že **nie každý používateľ má rovnaký internet** a **nemôžeme** mu na stránku dať **32MB obrázok**, ktorý by sme **my**, ako vývojári **stiahli za menej ako sekundu**, kdežto **niekto z východného Slovenska** by ho sťahoval **aj vyše 15 sekúnd**. Weby je veľmi dôležité optimalizovať tak, aby boli dostupné úplne všade. Je taktiež **dôležité kód zbytočne nepredlžovať**, nakoľko nám to môže pridať na náročnosti stránky a **na lacnejších a slabších zariadeniach** sa môže dokonca **zasekávať**. Je taktiež zbytočné na stránky vkladať **8K obrázky**, keď bude obrázok tvoriť **menej ako 30% obrazovky**.

# Responzívny web dizajn

Je veľmi dôležité, aby sme **nezabúdali** na to, že by sa **na obrazovke nemalo nachádzať príliš veľa elementov** naraz. Pri **mobilnej verzii** stránky by sa nám totiž **text mohol stať priam nečitateľným**, nakoľko by ho veľa elementov zakrývalo.
Musíme myslieť aj na to, že **aj napriek tomu, že sa nachádzame na takom malom médiu**, mali by sme zachovať rovnaké, ba aj **väčšie medzery medzi samotnými odstavcami**, ikonkami a tlačidlami.

Na **mobilnej verzii stránky** by sa malo taktiež **zmeniť navigačné menu** z pozdlhovastého na stlačené, poprípade na malú tzv. "hamburger" ikonu, ktorá zobrazí ďalšie možnosti.

Tiež by sa mali **odstrániť**, poprípade zmenšiť, **rušiace prvky**. Potvrdenia o cookies by sa mali zmeniť z full-screen potvrdenia na malé tlačidlo na dolnej časti obrazovky.

> “A designer knows he has achieved perfection not when there is nothing left to add, but when there is nothing left to take away.” - Antoine de Saint-Exupéry

Najhlavnejšie je **prispôsobiť user experience pre dotyk**. Slidery by mali fungovať pomocou **tlačidiel**, pomocou **preťahovania prstom** ale aj **klávesnicou naraz**. Nikdy totiž **nevieme**, či čitateľ pozná zariadenie, ktoré používa, poprípade pozná práve **tie gestá**, ktoré chceme **použiť**.

Na **mobilných zariadeniach** by mali byť **odstránené sekcie**, ktoré sa tam veľmi **nehodia**, teda bočné panely, widgety a floating-tlačítka.

![Responzívny dizajn](https://assets.awwwards.com/awards/images/2015/07/awwwards-responsive-big.png)

# Optimalizácia obrázkov

Ako sme už spomínali vyššie, je **veľmi dôležité nevkladať na web obrázky s príliš vysokým rozlíšením**, hlavne, keď sa dané rozlišenie nevyužije naplno. Stránka sa nám na pomalých sieťach bude **načítavať príliš pomaly**. Naopak do článkov, v ktorých väčšinou chceme **vyzdvihnúť určitú časť obrázku**, napríklad budovu alebo osobu, je nutné vkladať **minimálne Full HD obrázky**, teda s rozlíšením 1920x1080px. V **opačnom prípade** môže totiž dôjsť k tomu, že obrázky budú príliš **rozpixelované**, poprípade rozmazané a článok tak bude rozprávať o niečom, čo ani nevidíme.

Je taktiež veľmi **dôležité**, aby **obrázok nezastával na obrazovke viac ako 50%** priestoru na výšku. Stránka by sa tak stala veľmi neintuitívnou a príliš náročnou na čítanie. Na **mobilných zariadeniach** by obrázky mali byť **ešte menšie**, nakoľko môže nastať situácia, kedy na obrazovke uvidíme veľmi minimálne množstvo textu. V **najlepšom prípade** by sme mali aj **odstrániť akékoľvek bannerové reklamy**, ak je to možné.

Nakoľko nie je možné, aby malé weby, blogy a e-shopy mali servery po celom svete, stáva sa, že ich **načítanie z opačnej strany sveta** je oveľa **pomalšie** ako o mesto vedľa. Práve preto sa **používajú** tzv. **CDN**. Jedná sa o **centralizované servery**, ktoré nám **poskytujú stiahnutie zdrojov** zo **serverov po celom svete**. Nemusíme teda čakať 5 sekúnd na to, aby sa nám stiahol jeden .css súbor, ktorý je hostovaný na veľmi pomalom serveri.

![CDN](https://res.cloudinary.com/lwgatsby/f_auto/www/uploads/2020/09/2-how-does-a-cdn-work-1.jpg)

# Farby a štýly

V grafickom dizajne **existujú dva pojmy** - **user experience** a **user interface**. User experience hovorí o **intuitívnosti dizajnu**, o tom, ako by stránka mala byť **ľahko použiteľná pre všetkých** a ako by všetky ikony mali signalizovať to, čo skutočne robia. Nemala by byť **zbytočne plná nepekných elementov**, ktoré so sebou nijako **nesúvisia** a navzájom si zavadzajú. Na základný návrh user experience sa **väčšinou** používajú prototypy a **wireframy**.

Naopak, **user interface hovorí** o tom, **ako stránka**, poprípade aplikácia **vyzerá**. Hovorí o tom, či **je dizajnovo moderná** a či **má konzistentný design language**. Na stránke by sa nám **nemali meniť hlavné farby**, ktoré používame. Tiež by sa nám **nemala drasticky meniť rozloha stránky** bez akéhokoľvek používateľského vstupu.

Považuje sa za **vhodné využívať**, aj keď už často používané, **moderné prvky webového dizajnu**, nakoľko sú **použivatelia** na internete **zvyknutí na fungovanie rôznych tlačidiel** rovnakým spôsobom naprieč viacerými webmi.

**Dôležité** je tiež **zachovávať** na jednom webe **rovnakú farebnú paletu** a štýl. Ak sú nadpisy červenou farbou, rovnakou farbou by mali ostať všade. Ak majú tlačidlá "sklenený dizajn", rovnako by mali vyzerať aj na mobilných zariadeniach.

Ak je **web dizajnovaný s myšlienkou konzistencie** na prvom mieste, jej používatelia sa o nej začnú učiť rôzne veci bez toho, aby nad tým vôbec premýšľali. **Webovú stránku** si môžeme **predstaviť** ako náš **domov**. Jedná sa o miesto, ktorým vieme navigovať stále, bez sústredenia sa na to. Ak k nám príde návšteva, môže byť na určitý čas zmätená z toho, kde sa nachádza toaleta, kde je obývačka a kde je gauč, no časom sa tieto veci naučí. **Úlohou dizajnéra** je tento čas čo najviac skrátiť a **byť čo najviac konzistentný**, aby nedošlo k tomu, že používateľ bude očakávať tlačidlo späť na stránke s chybou 404, keď bolo vždy na každej inej podstránke.

![UX vs UI](https://grafika.sk/wp-content/uploads/2016/07/rozdiel-UX-a-UI.png)

# Základné pojmy

**Frameworks**
> Knižnica podporných programov, radu API, návrhových vzorov, prídavných funkcií a skriptov, s pomocou ktorej sme schopní vytvoriť funkčnú službu. Slúži na uľahčenie tvorby web stránky.

**Front-end**
> Predná časť stránky - tá, ktorú vidíme.

**Back-end**
> Zadná časť stránky - tá, ktorú nevidíme. Jedná sa o všetko, čo sa deje na pozadí.

**Bootstrap**
> Otvorená sada/knižnica Javascriptových, CSS a HTML nástrojov pre tvorbu responzívneho, krásneho webového dizajnu, ktorý v prvom rade myslí na mobilný zážitok.

**404**
> Chybový kód, ktorý hovorí o tom, že súbor alebo služba nebola nájdená.

**Cache**
> Jedná sa o časť dát, ktorá sa z každej webovej stránky ukladá lokálne, do počítača. Vždy, keď navštívime nejakú službu, všetky súbory, o ktoré požiadáme z jej serverov, sa nám stiahnú do cache za účelom zaručenia toho, že ak stránku navštívime niekedy v budúcnosti, dané súbory nebudeme musieť sťahovať už znova. Používajú sa taktiež na zdieľanie informácií naprieč webovými stránkami (napr. aby sme sa nemuseli prihlasovať do každej služby Google po jednom).

**CMS**
> Jedná sa o serverový systém, ktorého úlohou je spravovať, archivovať, vytvárať a prezentovať obsah a dáta používateľovi web stránky. Umožňuje nám vytvárať, upravovať a zobrazovať príspevky napr. na blogu.

**Plugin**
> Rozšírenie akéhokoľvek programu, ktoré pridáva prídavnú funkcionalitu. Môže sa napríklad jednať o pluginy, ktoré pridávajú cookies pop-upy do WordPressu.

**Minifikácia**
> Spôsob optimalizácie akéhokoľvek kódu. Sadou nástrojov a pravidiel kód zredukujeme na najmenšiu veľkosť napríklad odstránením prebytočných medzier, kompilátorom-ignorovaných znakov, komentárov a nepoužívaných funkcií za cieľom toho, aby sa čo najviac zmenšila finálna veľkosť súboru.

**Dribbble**
> Zaujímavá sociálna sieť vytvorená pre digitálnych dizajnérov a kreatívnych ľudí. Môžu tu zdieľať svoje kreácia z mnohých častí grafického dizajnu - webový, papierový, animovaný, vektorový, mobilný, produktový a typografický dizajn.

**Flaticon**
> Užitočná webová databáza, ktorá grafickým dizajnérom ponúka širokú ponuku rôznych ikoniek, slúžiacich na akékoľvek účely.

**Favicon**
> Ikonka web stránky. Dôležitým cieľom grafického dizajnéra je vytvoriť ikonku, ktorá bude v čo-najmenšiom formáte čo-najviac rozoznateľná.

**Lazy loading**
> Načítavania počas scrollovania. Dokým nie je časť stránky viditeľná na obrazovke, nie je načítaná.

**Bounce rate**
> Percento, ktoré určuje počet čitateľov, ktorí opustia náš webu bez akejkoľvek interakcie s danou stránkou.

**Wireframe**
> Základný návrh stránky bez akéhokoľvek zaujímavého vzhľadu. Hovorí o rozlohe webu, kde sa čo bude nachádzať, a ako to bude so sebou spolupracovať. Sú väčšinou tvorené v čiernobielej forme, pričom sú miesto obrázkov používané zástupné preškrtnuté štvrce. Snažia sa nedotýkať vizuálnej stránky webu, no zaujímať sa skôr o jeho organizáciu, obsah a funkcie. Wireframe je možné vytvoriť v programoch Adobe Illustrator, Adobe Xd, Microsoft Visio, atd. Skutočnosťou je však aj to, že wireframe je možné vytvoriť úplne jednoducho na papier, či na bielu tabuľu. Nemusí byť vôbec interaktívny, stačí aby vyvolal odpovede na otázky ohľadom kompozície web stránky.
> ![Wireframe](https://i.ytimg.com/vi/zQ3Cn3EQz3k/maxresdefault.jpg)

**WYSIWYG**
> What You See Is What You Get - forma písania článkov v redakčných systémoch. To, čo ako autor vložíme, bude to, čo na stránke uvidíme ako finálny výsledok. Myšlienkou WYSIWYG editorov je vytvorenie webových stránok v priamom zobrazení dizajnu, pričom program na pozadí napíše HTML a CSS za nás priamo v reálnom čase. Umožňujú nám písať články a iný obsah pre web bez akejkoľvek znalosti HTML a CSS.
> ![WYSIWYG](https://i.postimg.cc/xjHPdYJW/image.png)

# Použitie frameworkov

PHP frameworky nám uľahčujú vývoj webu. Poskytujú nám dobre organizovaný kód, ktorý môžeme v priebehu času ľahko škálovať. Vďaka nim máme k dispozícii už hotové komplexné funkcie a dizajnové elementy, pomocou ktorých môžeme do hodiny vytvoriť hotový blog, redakčný systém ale aj e-shop.

Medzi najobľúbenejšie PHP frameworky patria:
1. **Laravel** - vydaný v roku 2011. Je momentálne najobľúbenejším frameworkom medzi vývojármi. Má obrovský ekosystém s platformou pripravenou k okamžitej tvorbe. Funguje na základe odľahčeného šablonového enginu Blade, má elegantný syntax a podporuje aj autentikácia, relácia, radenie do front, cachovanie a REST.
![Laravel](https://www.consoleinfotech.com/img/laravel-6.0.jpg)

2. **CodeIgniter** - odhľahčený PHP framework, vydaný v roku 2006. Má veľmi jednoduchý inštalačný proces, ktorý vyžaduje minimálnu konfiguráciu. Používa komponenty controllery, modely a views. Rovnako ako Laravel, poskytuje svojim vývojárom značnú voľnosť. Zaujímavosťou je, že na disku zaberie len 2MB.
![CodeIgniter](https://miro.medium.com/max/1031/1*7o6KRu9HrRfqKlpIhFGmpg.png)

3. **Symfony** - framework, ktorého cieľom je vývojárovi čo najviac uľahčiť prácu. Je osekaný do množstva konfiguračných súborov, ktoré sa píšu vo veľmi úspornom jazyku YAML. Obsahuje množstvo pluginov, ktoré majú programátorovi pomôcť v perfektovaní svojho webu.
![Symfony](https://miro.medium.com/max/1024/0*YYimU29xUrOcvh8m.)

4. **CakePHP** - jeden z najstarších frameworkov. Ponúka solídny základ, mnohonásobne lepší výkon v reálnom prostredí, má prepojený systém pluginov a tém, pričom je jeho výhodou aj ľahšia lokalizácia webu pre široké škály používateľov.
![CakePHP](https://miro.medium.com/max/750/1*butnM2l-USwSb7wE_Vj-JA.png)

5. **Laminas Project** - jedná sa o zbierku profesionálnych balíkov PHP, slúžiacich na pokročilý vývoj webových aplikácií a služieb. Je spravovaný Linux Foundation.
![Laminas Project](https://www.galvao.eti.br/wp-content/uploads/2019/04/LaminasHightlight-1280x720.png)

# Zdroje
##### Použité knižné zdroje:
1. [Modern PHP, O'Reilly Media, Inc., 2015, ISBN9781491905012](https://www.oreilly.com/library/view/modern-php/9781491905173)

2. [Laravel: Up & Running, 2nd Edition, O'Reilly Media, Inc., 2019, ISBN9781492041214](https://www.oreilly.com/library/view/laravel-up/9781492041207)

3. [Web Design with HTML and CSS Digital Classroom, (Book and Video Training) 1st Editionn, AGI Creative Team, Jennifer Smith, Jeremy Osborn, 2011, ISBN9780470583609](https://www.oreilly.com/library/view/web-design-with/9781118094280)

4. [The Principles of Beautiful Web Design: Designing Great Web Sites is Not Rocket Science!, Jason Beaird, James George, 2014, ISBN9780470583609](https://www.amazon.com/Principles-Beautiful-Web-Design-Designing/dp/0992279445)