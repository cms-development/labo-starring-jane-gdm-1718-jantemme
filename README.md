# Starring Jane Gastles
## Starring Jane
Starring Jane is een Digital Web Agency in Gent die zich focust op PHP, .NET en Javascript. Ze bestaan uit onder andere 2 grote dev-teams.

## Case
mijnherinneringaanjou.be, een web app voor kinderen om de dood van vrienden en familie beter te kunnen verwerken.
### Klant
- Dela (Uitvaartverzekeringen)
### Waarom dit een interessante opdracht was
- Breed doelpubliek: Zowel volwassenen als kinderen
- Moest zeer kwalitatief zijn (Marketing voor Dela)
- Persoonlijk en veilig, deleting all data on account deletion
- Dela released de website met een persbericht
### Taakverdeling
Voor deze opdracht werkte Starring Jane samen met Studio Monk (Designbureau) en een kindertherapeut.

- Starring Jane: UX UI, Development, GDPR
- Studio Monk: Illustraties
- Therapeut: Copywriting

### Requirements
- Zowel mobile als desktop
- Performant voor de launch
- Gedeeltelijk offline: PWA

### Sprints
Starring Jane werkte voor deze opdracht met sprints, in korte tijdsperioden werkte ze naar een bepaald doel (deliverable) om dan feedback bij de klant te vragen. Na deze feedback stond het voorbije deel vast en gingen ze door naar de volgende sprint.

### Development
#### Backend: 
De backend was een Laravel api. Deze bevatte tests om te verzekeren dat elk deel werkte naar behoren.

#### Frontend: 
- Voor de frontend maakten ze gebruik van Vue.js. Dit doen ze om verschillende redenen, de grootste daarvan: de lage learning curve. Verder bevat Vue observables, variabelen waar je aan kan vanuit elk component. Dit gebeurt doormiddel van een store waarin deze variabelen zitten, deze kan je dan opvragen doormiddel van Getters (methoden die de variabele returnen). Dit zit ingebakken in Vue in tegenstelling tot alternatieven zoals React, waarbij je hiervoor een aparte library moet gebruiken.

- Wat ook herkenbaar is bij Vue is het opdelen van de app in components. Elk klein deeltje wordt een component, die we dan kunnen gebruiken in een groter component, bv: een button, die dan in een model wordt gebruikt, die dan weer in de omgeving wordt gebruikt. Deze components kunnen we hergebruiken doormiddel van props (properties), dit zijn variabelen die we vanuit de parent kunnen doorgeven aan een component. Bv: een button waar tekst in komt en iets moet gebeuren wanneer je erop klikt, als prop geven we dan mee welke tekst in de button moet komen en wat er moet gebeuren bij het click-event.

- Vue bevat ook pre-defined actions: Created, Mounted, destroy, etc. Deze zijn handig om code te runnen die zo snel mogelijk moet gebeuren bij het inladen van de app (Created), bv: api's fetchen. Wanneer we naar een andere pagina gaan kunnen we ook de Destroy-method gebruiken om op de vorige pagina een "cleanup" te doen, bv: alle listeners verwijderen omdat deze anders later voor problemen kunnen zorgen.

- Ook de "Watch" method is zeer handig. Hiermee kan je een variabele "watchen" op verandering waarbij deze method een callback triggered.

- Op hun webapp was er ook een ballon die je kon besturen op desktop (pijltjes) en op mobile (gyroscoop). Dit is meer werk dan je denkt, zeker omdat het multiplatform is.

### Tips van Starring Jane
- Promises: Js in asynchroon dus wanneer we moeten wachten op iets loopt het mis, bv: api fetch. We kunnen in deze gevallen een promise gebruiken: een promise voert een stuk code uit en wacht tot dit lukt om dan verder te gaan. Ook wanneer dit misloopt kan de promise het opvangen.

- Op voorhand samen met het backend-team een database structuur afspreken zodat de api hierop kan worden afgesteld.

- Axios gebruiken voor api calls.

- Vue devtools, in de browser je component structuur zien, de store en vele andere vue related debugging.

## Feedback op de gastles
Ik vond deze gastles zeer goed gegeven en interessant. Dit komt waarschijnlijk ook door mijn bredere basis tegenover vorig jaar en het feit dat ik van te voren al geïnteresseerd was. Naar het einde toe werd het iets moeilijker om de aandacht erbij te houden maar dit lag niet aan de inhoud van de gastles op dat moment. Ik begrijp nu ook beter waarom Vue een goed alternatief is, zeker wanneer je met niet-frontenders samen werkt. Verder heb ik over Vue zelf veel bijgeleerd en weet nu beter wanneer ik het in de toekomst zelf kan gebruiken.