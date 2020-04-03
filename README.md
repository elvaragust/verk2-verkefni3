# verk2-verkefni3
# 3.1 LCD (5%)
## 1. ↓↓↓
    1. Hver er helsti munurinn á Character LCDs og Graphical LCDs?
    Character LCD er betri til að sýna texta/litlar myndir í 16 (5x7 pixlum) en graphical Lcd er betri til að búa til myndir afþví það er bara eitt stórt grid sem er (128x64 pixlar)

    2. Hvað gerir RS pinninn á LCD?
    Resister Select (RS): ræður hvernig data/mode er sent í lcd skjáinn (instruction mode/character mode)

    3. Afhverju þarf að tengja RW pinna í jörð ef við erum ekki að nota hann?
    Ástæðan er að digital i/o á Arduino pinMode(), digitalRead(), digitalWrite() var ylla hannað og er hægt, sérstaklega AVR,og að nota busy flag er hægara heldur en smart delays.

    4. Hvað er hægt að birta marga stafi í LCD1602?
    hann er með 32 total grid sem er skipt í 16 grid uppi og 16 grid niðri

    5. Ahverju þarf að stýra LCD1602 með nokkrum pinnum (4 eða 8) á sama tíma? útskýrðu!
    Það er ekki víst afhverju en það er helmingi hraðara að nota 8 pinna heldur en 4. 4 bita tekur 7 (1/0 pinna) en 8 bita tekur 11 (1/0)pinna og þu getur gert eiginlega hvað sem er ef maður notar 4 bita

## 2. [link a tinkercad](https://www.tinkercad.com/things/63A8e1V6wB9-epic-uusam/editel)

# 3.2 motor og Transistors (5%)
## 1. ↓↓↓
    1. Hvernig er skrefmótor (e. stepper motor) ólíkur hefðbundnum DC mótor?
    DC motor er þekktur fyrir að hafa járn súlu sem stendur úr honum og hann getur snúið sér eins mikið og hann vill en stepper motor er þekktur fyrir ad hafa plast kassa og hann getur bara farið 360* og svo þarf hann ad fara til baka
    
    2. Hvernig er stýrimótor (e. servo motor) ólíkur hefðbundnum DC mótor?
    Servo motorar eru sérstakir DC mótorar sem eru með innbyggtu control borði sem þarf signal frá micro-controller
    
    3. Hvernig er hægt að stjórna í hvora áttina DC mótor snýst?
    þú stjórnar því með að setja eithvað ákveðið rafmags flow ef það er negative þa fer hann counter-clockwise og ef það er positive þa fer hann clockwise
    
    4. Hvað gerir transistor?
    transistor er electronic component sem tekur lítið rafmagn og gerir það sterkara
    
    5. Hver er munurinn á NPN og PNP transistorum?
    PNP transistors eru með 2 layers af P(positively charged) efni sem eru utan um eitt layer af N (negatively charged) efni og það hveiknar á honum þegar það er ekkert rafmagn að fara í gegnum hann, NPN transistorinn er öfugur og hann er með 2 layer af N (negatively charged) sem er utan um eitt layer af P (positively charged) efni og hann er alltaf að senda rafmagn þangad til að það er ekki nógu mikið rafmagn og hann slekkur á sér.
## 2. [link af tinkercad](https://www.tinkercad.com/things/ay6XRKiXGGd)     
## 3. ↓↓↓
    1. Afhverju þurfum við að nota PWM pinna til að stýra DC mótor?
    Hann stjórnar hversu mikið rafmagn kemur inn a dc motorinn
    2. Afhverju þurfum við að nota viðnám, transistor og diode með DC mótor í Lesson 13. DC Motors
        * viðnámið stýrir hversu mikið rafmagn það á að fara í transistor
        * transistor er til að tryggja að það kemur 5v og til að stilla hraða á motorinum
        * diode er notað til að tryggja að ekkert klikkar þegar þú slekkur á motorinum
## 4. [link af verklega](https://photos.app.goo.gl/bScvanTG5LkXjWF98) 

# 3.3 DC motor og H-Bridge (5%)
## 1. ↓↓↓
    [link af tinkercad](https://www.tinkercad.com/things/81T8Lr4IAEQ)
    
    [link af verklega](https://photos.app.goo.gl/kdWcXXvbtqPcohER7)
## 2. ↓↓↓
    1. Hvað er hægt að gera með L293D
    L293d er helst notað fyrir motora og til að stilla hraða
    2. Hver er munurinn á L293 or L293D
    munurinn á l293 og l293d er að í l293 þá þarf maður að nota auka íhlut
    3. Í lesson 15 er eftirfarandi kóðabútur, útskýrðu hann útfrá H-Bridge
    þetta er til að breyta hraðanum og ef pin1 er í high og pin2 í low þá myndi það snúast í eina átt og það sama og öfugt
    4. L293D er með tvo +V pinna (8 and 16), útskýrðu þá
    pin (8) er notaður fyir power á motor og (16) fyrir kubbin sjálfan
    
## 3. ↓↓↓
    * Brushed DC Motor
        þessir eru notaðir helst í að búa til leikföng sem keyra og viftur
    * Brushless DC motor.
        þessir eru ekki eins hávaðir og brushed og þeir eru helst notaðir fyrir tölvu viftur o.f.l
    * Stepper motor
        þessir motorar eru dýrarstir, hraðastir og bestir þeir eru helst notaðir fyrir klukkur eða vélmenni
    
    








