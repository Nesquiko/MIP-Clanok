# [Why Don't Software Developers Use Static Analysis Tools to Find Bugs?](https://ieeexplore.ieee.org/abstract/document/6606613)

## 3 vyskumne otazky:
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
Skratky:
- NST = nastroje statickej analyzy
- ST = staticka analyza
