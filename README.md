<details>
  <summary>Web Typography Opdracht, 2022/2023</summary>

Als je doof bent, of als je om een andere reden geen geluid kunt horen, dan mis je veel informatie als je een film kijkt. Knisperende voetstappen, langzaam aanzwellende muziek, nerveus getik op een deur, je hoort het natuurlijk allemaal niet. Nu bestaat er zoiets als *closed caption*, wat een type ondertiteling is waarbij ook dingen als omgevingsgeluiden en de muziek beschreven worden. Hierdoor krijgt een kijker die informatie wel binnen.

Alleen wordt die auditieve informatie nogal neutraal beschreven. Het geluid van huilend persoon zou bijvoorbeeld beschreven kunnen worden als *snikgeluid op de achtergrond*. En iemand die lacht zou geschreven kunnen worden als *iemand lacht.* Heel neutraal, bijna zakelijk, en bovendien allebei in precies hetzelfde neutrale lettertype. Terwijl het toch echt over twee heel verschillende emoties gaat. 

Dat kan visueel sterker. 

En dat gaan jullie doen.
  
  </details>
  <details>

  <summary>Leerdoelen</summary>

- Je kan de kennis over vormgeving die je hebt opgedaan tijdens de minor technisch toepassen met behulp van CSS
- Je kan verborgen nuance uit een audiotrack overtuigend vertalen naar visuele (typografische) beelden
- Je kan je typografische keuzes onderbouwen.
- Je hebt de exclusive design principles gebruikt.

  </details>
  <details>
  
  <summary>Oplevering</summary>

Je levert een werkende versie op, gemaakt met HTML, CSS en JavaScript. Deze staat op Github. In een duidelijke readme documenteer en onderbouw je je ontwerpkeuzes. Je developmentgeschiedenis is terug te vinden op GitHub.

Je levert ook een *screen recording* met audio op van je fragment. Dit is een video van de definitieve versie, gemaakt van jouw browserscherm.

De beoordeling is mondeling en volgt [de rubric uit het beoordelingsformulier](web-typografie-beoordeling.pdf).

  </details>
  <details>
  
  <summary>Typografische restricties</summary>

Je *moet* een van deze twee opties kiezen, en je keuze moet je onderbouwen. In je readme staat een uitleg over je overwegingen om de ene of de andere restrictie te kiezen.

### Optie 1: Systeemfont

De eerste optie is dat je gebruik maakt van het zogenaamde *systeemfont* van degene die naar jouw werk kijkt. Dit font verschilt per operating system, en het verschilt soms zelfs per versie van het operating system. Het is ook aan te passen door de gebruiker zelf. 

Je hebt dus geen controle over welk lettertype er precies gebruikt wordt. Het levert dus een onzeker, en beperkt typografisch palet op. Je hebt geen *light* versies, of *extrabold*. En ook geen serif en sans-serif versie van dezelfde familie. In dit geval heb je alleen de beschikking over normal, **bold** en _italic_. Dit heeft natuurlijk ook zijn voordelen!

### Optie 2: Brenner

Je kan er ook voor kiezen om gebruik te maken van de complete Brenner familie. Dit is een zeer uitgebreid en uiterst flexibel font. [Hier kan je je verdiepen in dit font](https://www.typotheque.com/blog/brenner_an_unusual_typeface_family_with_distinct_voices). Als je kiest voor dit font dan heb je de beschikking over een *sans serif*, een *condensed*, een *serif*, een *monotype*, een *slab*, een *display* en een *script* versie. En veel van deze versies hebben varianten van *light* tot *bold*, en allemaal zowel *bold* als *italic*.

Met Brenner zijn er natuurlijk veel en veel meer mogelijkheden dan met systeemfonts. Dat kan zowel een voordeel als een nadeel zijn. 

Voor een overzicht, zie [de brenner.pdf](brenner.pdf).

  </details>
  <details>
  <summary>Het fragment</summary>

Ik heb een fragment voorbereid. Het gaat om twee scenes uit *Blade Runner 2049*. De captions staan in de HTML, en ze verschijnen in sync met de video. [Kijk maar](closed-captions/index.html).

  </details>
  <details>
  
  <summary>De captions</summary>

De captions staan in de html, in het bestand index.html. Je kan aan elke paragraaf eventueel een of meer classes toevoegen. Bijvoorbeeld `voice1` of `voice2 soft`. Classes voeg je handmatig toe in de html.

Met JavaScript worden er een paar dingen extra gedaan: 

- er wordt aan elke paragraaf een unieke class toegevoegd (`p0`, `p1`, etc)
- Elk woord wordt in een aparte `span` gezet. Hierdoor kan je elk woord apart stylen, en eventueel ook [na elkaar laten verschijnen](https://github.com/cmda-minor-vid/web-typography-18-19/blob/master/closed-captions/css.css#L41).

  </details>
  <details>
  <summary>Tijdens het afspelen</summary>

Tijdens het afspeelen wordt er een class `on` op de caption gezet als hij moet verschijnen, en een class `off` als hij klaar is. *Zowel class `on` als class `off` blijft op de caption staan!*

De timimg van de captions kan je aanpassen in [closed-captions/captions.js](closed-captions/captions.js).

Er verschijnen ook classes op de body op momenten dat er geluiden worden afgespeeld, zoals `sound1` en `sound2`. Je kan geluiden toevoegen in [closed-captions/sounds.js](closed-captions/sounds.js).

*let op,* de geluiden zijn niet compleet, dit zal je zelf moeten aanvullen.
  
  </details>
  <details>

  <summary>Een eigen fragment (afgeraden, uitgebreide onderbouwing is nodig)</summary>

Je kan er ook voor kiezen om een eigen, *beter* fragment te gebruiken. Dit wordt afgeraden. De tijd die je besteedt aan het zoeken naar dat fragment kan je beter besteden aan het werken aan de opdracht. Bovendien blijkt dat er vaak fragmenten worden gekozen die niet goed voldoen aan de opdracht. Als je een ander fragment kiest dan *moet* je dit goed onderbouwd voorleggen aan je docent. De deadline hiervoor is vrijdagochtend in de eerste week.

### Waar moet je op letten bij het kiezen van een eigen fragment.
Lees de opdracht nog eens goed door. Waar gaat het ook al weer precies om? 

Voor een goede onderbouwing van je keuze voor een ander fragment moet je deze vragen in elk geval beantwoorden:

- Welke informatie zit er in de audio die echt niet zichtbaar is?
- Welke rol speelt de audio in het fragment?
- Werkt de scene nog zonder geluid?
- Waarom is dit fragment beter dan het aangeboden fragment?

Je kan dan de nodige HTML en JavaScript genereren door gebruik te maken van [caption generator](https://cmda-minor-vid.github.io/web-typography-18-19/generator/) (in Google Chrome). 

Als je de closed captions wil bewerken dan kan je een tool zoals [Amber Script](https://www.amberscript.com/en) gebruiken. Daar kan je exporteren als `.srt`, en die kan je weer door de generator halen.

</details>

### MIJN PROCES:

Mijn eerste stappen waren om bij elke sound een animatie toe te voegen. Ik ben erg extreem begonnen, met wilde animaties en extreme kleuren, puur om te kijken wat mogelijk is. 

Dit was de eerste feedback van Annika:

<img width="536" alt="peerfeedback_merelW" src="https://github.com/merelwiersmaa/webtypografie/assets/83574654/51ae4b73-e917-43a5-bda2-ea4c4e068cd5">

Hierna heb ik al een paar 'extreme' kleuren eruit gehaald en aangepast. Ook heb ik de 'visuele hoofdpijn' van de piep nog meer aangepast, zodat deze geleidelijk opbouwt bij het harder worden van de piep.

Na de tweede feedback in de klas met Vasilis, kreeg ik positieve reacties op mijn experimenten met de bewegingen en kleuren. Als tip kreeg ik om het te fine-tunen naar een mooie tussenweg, waarin het nog wel 'extreem' is maar niet afwijkt van de sfeer van het fragment. Ook het piep-geluid mag nog meer opgebouwd worden, want in het begin is die nog amper te horen, terwijl mijn animatie al begint. 

Ook het contrast met achtergrond en tekst moet ik goed in de gaten houden zodat het leesbaar blijft.

UPDATE:

Ik ben nu de animaties aan het aanpassen dat ze alleen tijdens het geluid veranderen, en niet veranderd blijven ná het geluid. Het is nu een eenmalige animatie, net zoals het geluid ook eenmalig is.

Ook heb ik in de animaties een bepaald kleurenpalet aangehouden, die passen bij de sfeer:

Rood/maroon, wit, zwart, teal. Deze heb ik in de diverse animaties gebruikt, zodat het 1 geheel blijft.

Voor de agent/computer stem heb ik Brenner Mono Italic gebruikt, omdat dat de feeling van die computerstem goed weergeeft.

Voor KD6-3.7 heb ik Branner Slab gebruikt. Hij ziet er een beetje 'bad-ass' uit, en heb hem daarom dit stoere font gegeven.

Sommige woorden heb ik met een witte of 'teal' kleur aangepast om te benadrukken. Bijvoorbeeld de 'fuck-off skin-job' heeft een zwaar font en een andere kleur, waardoor je ziet dat het agressief bedoeld is en eenmalig in beeld komt, omdat het dus qua vormgeving afwijkt.

Ook het laatste woord van de computer 'constant K, you can pick up your bonus' heb ik laten afwijken van de normale vormgeving, omdat dit voor het eerst 'aardig' overkomt als een beloning, en geen kruisverhoor.

Verder heb ik niet veel met de tekst gedaan. De animaties van het beeld zijn al vrij druk en extreem, waardoor het in mijn ogen TEveel wordt als ik ook nog van alles doe met de tekst. 

Het laatste gedeelte met de piep heb ik ook aangepast. eerst deed ik de achtergrond om en om met complementaire kleuren om die visuele hoofdpijn te creeren, maar die kleuren paste niet bij de sfeer van de clip. daarom heb ik hiervoor andere kleuren gebruikt (maroon en teal, complementair maar dan 'duister') en heb ik de animatie zodanig uitgesteld dat het pas 'erg' wordt wanneer de piep toeneemt.

een nadeel is dat het hoofdpijn effect niet meer supersterk is, maar alsnog wel irritant om naar te kijken. Om dit te versterken heb ik op een gegeven moment het beeld op en neer laten bouncen, wat de trilling van de piep weergeeft.


