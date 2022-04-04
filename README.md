# VideoCloud

<h1 id="top">------------------------ PORTOFOLIO --------------------------</h2>
 

# introductie
In dit project wil ik een online platform maken waarin gebruikers media van andere gebruikers kunnen beluisteren en zelf ook media kunnen oploaden. Deze media zal alleen muziek zijn. Het doel is om hiermee aan te tonen dat ik kan laten zien dat ik begrijp hoe een JavaScript front-end werkt, dat ik dit kan combineren met een OO gebaseerde back-end taal en dat de software gedistribueerd is zodat het een grote hoeveelheid aan gebruikers tevreden kan stellen. Om dit proces voor de gebruiker zo snel en efficiënt mogelijk te maken zal er gebruik worden gemaakt van asynchrone communicatie om te voorkomen dat een gebruiker lang moet wachten. In combinatie van een intuïtieve UX moet dit ervoor zorgen dat de gebruikservaring van de website zo optimaal mogelijk is. De data van de gebruiker zal opgeslagen worden in een relationele database. Aangezien dit gevoelige informatie is zal er gekeken moeten worden naar verschillende beveiligingsopties om de data van de gebruiker te kunnen beschermen.


<h2 id="top">Inhoudsopgave ReadMe VideoCloud-documentatie</h2>
1: Onderzoek 1: XSS

<h2 id="top">1. Onderzoek 1: XSS</h2>

<h3 id="top">Introductie</h3>
<h4> Wat is Cross Site Scripting? </h4>
Cross Side Scripting is de naam van een fout in de beveiliging van een webapplicatie. Het probleem wordt veroorzaakt doordat de invoer die de webapplicatie ontvangt (zoals cookie, url, request parameters) niet juist wordt verwerkt en hierdoor in de uitvoer terechtkomt naar de eindgebruiker. Via deze bug in de website kan er kwaadaardige code (JavaScript, VBScript, ActiveX, HTML, Flash etc.) geïnjecteerd worden. Hiermee kunnen onder meer sessiecookies worden bekeken, sessie van een gebruiker worden overgenomen, functionaliteit van een website worden verrijkt of onbedoelde acties voor een gebruiker worden uitgevoerd. https://nl.wikipedia.org/wiki/Cross-site_scripting

Met een XSS aanval kan je kleine aanvallen doen, zoals de kleur van je website achtergrond aanpassen of een javascript alert creëren, alleen kan je ook met XSS aanvallen iemand zijn database platleggen doormiddel van 1 query in een tekstveld. Dat maakt het super belangrijk om hier beveiligd voor te zijn. En daaruit komt de vraag: 
Hoe kan ik mijn website beveiligen tegenover XSS aanvallen? 
<h3 id="top">Soorten XSS</h3>
 
 Als je over XSS spreekt, spreek je niet gelijk over een algemeen onderwerp. We spreken van 3 verschillende soorten XSS aanvallen;
 
<li>   Reflected XSS Attack:
Stored XSS also known as persistent XSS occurs when user input is stored on the target server such as database/message forum/comment field etc. Then the victim is able to retrieve the stored data from the web application.</ul>
<li>  Stored XSS Attack:
 Stored XSS also known as persistent XSS occurs when user input is stored on the target server such as database/message forum/comment field etc. Then the victim is able to retrieve the stored data from the web application. </ul>

<li> DOM Based XSS Attack: 
DOM Based XSS is a form of XSS when the source of the data is in the DOM, the sink is also in the DOM, and the data flow never leaves the browser.
</li>
<h4> 
 Wat kan ik tegen een XSS Doen?
</h4>
Gelukkig is Cross side scripting makkelijk te beveiligen. Populaire webframeworks zoals Laravel heeft ingebouwde beveiliging tegenover XSS aanvallen. 
-  Alle niet vertrouwde gegevens op basis van de HTML-Context, attribuut, Javascript, CSS of URL waarin de gegevens zijn geplaatst moeten uitgefilterd worden
 
 
<h3 id="top">Conclusie</h3>
Een XSS aanval wordt weinig aandacht aan gegeven bij beginnende ontwikkelaars terwijl  die aanvallen cruciaal kunnen zijn voor hun webapplicaties.

__________________________________________________________________
<h3>Conceptueel model(in the work)</h3>
(https://user-images.githubusercontent.com/73832880/161519346-5d78ed71-e2a0-4846-9ac1-61ec9b08a6d5.jpg)

<h3>Entity Relationship Diagram(in the work)</h3>
(https://user-images.githubusercontent.com/73832880/161521255-ef5687e2-7d00-4704-b8e7-6e8aa3bb0a70.JPG)

