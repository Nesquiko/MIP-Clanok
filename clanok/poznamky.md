# Poznamky

## [Why Don't Software Developers Use Static Analysis Tools to Find Bugs?](https://ieeexplore.ieee.org/abstract/document/6606613)

## 3 vyskumne otazky

### 1. Ake dovody maju na vyuzivanie/nevyuzivanie nastrojov statickej analyzy?

#### Vyuzivanie

- manualna kontrola je zdlhava a namahava, 5 z 20 ucastnikov si mysli ze NST sa oplati pouzivat, lebo automaticky hladaju chyby
  - "Hoci co co zautomatizuje vsednu/nudnu pracu je skvele."
- NST su uz predpripravene vo vyvojovom prostredi, 3 z 20
- udrzanie vyvojovych tymovych praktik, 7 z 20
  - zvysenie povedomia o moznych problemoch, chybach z nepozornosti, skor vo vyvojovom cycle
  - komunukacia a presadzovanie standardov a stylov kodu
- nastavitelnost pre hladanie chyb

#### Nevyuzivanie

- zle zobrazenie vystupu, 14 z 20
  - falosne pozityva prevazia pradive pozitiva
  - vo velkych projektoch, pocet chyb a varovani je vysoky a neprehladny, napravene lepsou prezentaciuo a citatelnostou
- zla podpora pre tymovu kolaboraciu, 9 z 20
  - manualne zdielanie nastaveni
- nastavitelnost nie je trivialna, alebo nie je podporavana vo forme aku by developer chcel, 17 z 20
  - vypnutie typu varovani na urcity cas
- nejasny vystup, 19 z 20
  - podrobnejsie vysvetlenia
  - navrhy rychlych oprav (Quick fix)

Tabluka na strane 6 Fig.1 je zhrnutie

### 2. Ako dobre tieto nastroje zapadaju do ich pracovneho preostredia a priebehu prace?

- NST beziace v pozadi, vystup poskytnuty hned v case vytvarania kodu
- integracia s kompilerom
- zastavenie prace a prekliknutie sa do NST narusuje developerove sustredenie
- pomale na vacsich projektoch, nutne zastavenie prace

### 3. Ake vylepsenia by chceli vidiet na tychto nastrojoch?

- navrh rychlych oprav, 10 z 20
  - zobrazenie pred a po uprave
  - moznosti aplikovania opravy - aplikovat cely navrh, iba cast, vobec
- zobrazeni chyb a varovani, 20 z 20
  - co najrychlejsie, bez rozrusenia priebehu prace, v pozadi s okamzitymou spatnou vazbou, pocas kompilovania
  - ulozenie sprav na neskor, zdialanie s inymi developermi
- grafy a diagramy namiesto listov chyb

#### chyby prace: maly data set (20 developerov), developeri co uz pracovali s NST, neznamy kod pre developerov pocas interaktivnej casti interview

## [Why Do Software Developers Use Static Analysis Tools? A User-Centered Study of Developer Needs and Motivations](https://ieeexplore.ieee.org/abstract/document/9124719)

Studia s 87 developermi firmy Software AG.

## 4 vyskumne otazky

### 1. Ako su NST integrovane do vyvojoveho prostredia?

- najcastejsie pouzivane NST su specializovane a IDE nastroje a upozornenia + graf Figure 2
- rozne formy vystupu, ale preferovana moznost je mat vsetko na jednom mieste + graf Figure 3
- stylove nedostatky maju nizsiu prioritu oproti vykonnosti, pamati a chybam subeznosti + tabulka Table 1 a graf Figure 4

### 2. V akych kontextoch vyuzivaju devekloperi NST a s akymi cielmi?

- developeri vyuzivaju NST behom volna (cas medzi stretnutiami, volne casove okno,...) + tabulka Table 2
- oprava chyb a varovani je najcastejsie realizovana v kratsich pracovnych sedeniach + tabulka Table 3
- developeri otvaraju NST s cielom opravenia vsetkych chyb/varovani a s cielom opravenia chyb/varovani v danom casovom useku + tabulka Table 4
- cas je hlavny dovod preco developeri zatvaraju NST a to aj ovlyvnuje ake chyby/varovanie opravia + tabulka Table 5

### 3. Ake strategie developeri aplikuju pri praci s NST?

- developeri prevazne opravuju to co vedia opravit, maju na to znalosti o celkovom projekte, skusenost s danym NST
- varovania su vyberane podla znalosti a skusenosti z danym NST
- UI NST by malo podporit spravne spravanie, ako napr. kolaboracia, ziskavanie znalosti o danom projekte

### 4. Ake funkcie by mali NST poskytovat developerom?

- developeri najcastejsie pri otvarani NST pozeraju na hlavnu stranku so vseobecnym prehladom o projekte
- pri zatvarani pozeraju najcastejsie na list chyb/varovani
- UI funkcionality tykajuce sa opravi chyb su najpopularnejsie

### Zaver

1. Casove obmedznia su primarny problem developerov pri praci s NST. Dlzka praconej casti s NST by mala byt zobrana do uvahy pri dizajnovani pracovneho prostredia/priebehu.
2. Dlhy proces analyzy alebo nejasne UI. Tieto prvky by maki byt minimalizovane na znizenie cakacieho casu.
3. Moznost pridat vlastne pravidlo na zaklade firemneho alebo projektoveho predpisu.
4. Niektore pravidla mozu naopak sposobit skodu. Zlepsenim vysvetlitelnosti varovani by bol efekt tychto pravidiel minimalizovany.
5. Rozvoj znalosti by mal integrovany cez prisposobene varovania k developerovim znalostiam, casu a schopnosti.
6. Taktiez znalosti by mali byt volne dostupne vsetkym cez nastavenia v NST.
7. NST by mali byt dizajnovane aby podporovali spravne spravanie v situaciach ked su uzivatelia zaseknuty.
8. Viacero typov NST by malo byt pouzitych sucasne (zamerannych na vykonnost, pamat, ...)
9. Pri pouzivani viacerych NST, vystupy by mali byt na jednom centralnom mieste. Toto by prinieslo lahsie porozumenie varovaniam, centralne miesto pre znalosti, kolaboracie a aj na statisticke ucely
10. Uspech NST priamo zavisi na firemnych predpisoch, rozsireni znalosti o vyhodach NST a ucelovych treningoch na ich implementaciu

#### chyby prace: data set iba z jednej firmy, zle porozumenie otazkam

## [A few billion lines of code later: using static analysis to find bugs in the real world](https://dl.acm.org/doi/10.1145/1646353.1646374)

Porovnanie potrieb ST v akademickom prostredi a v komercnom.

## [Using Static Analysis to Find Bugs](https://ieeexplore.ieee.org/document/4602670?denied=)

Skratky:

- NST = nastroje statickej analyzy
- ST = staticka analyza
