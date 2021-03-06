---
layout: default
title: De technologie
section: technisch
---
<h3>De technologie achter Limesco</h3>
<p>
Er zijn bij Limesco twee vormen waarin telefoonverkeer kan plaatsvinden:
<em>Out-of-the-Box</em> en <em>Do-It-Yourself</em>. Beide vormen hebben hun
eigen voor- en nadelen, zoals hieronder te vinden is. De technische afhandeling
van gesprekken, sms en mobiel internet wordt door <a
href="http://speakup.nl">SpeakUp</a> geleverd.
</p>

<h3>Out-of-the-Box</h3>
<p>In deze vorm is er praktisch geen verschil met
standaardabonnementen bij andere providers. Je kan bellen en gebeld worden zoals
je dat normaal ook zou kunnen. Hetzelfde geldt voor SMS en data. Out-of-the-box
is daarmee de simpelste en meest toegankelijke abonnementsvorm om te bellen via
Limesco.</p>

<h3>Do-It-Yourself</h3>
<p>Deze vorm houdt in dat je het telefoonverkeer (vooralsnog alleen spraak) zelf
regelt. In deze vorm worden alle inkomende gesprekken op een door jou gekozen
server afgeleverd en moet je zelf bedenken hoe je dit verder <em>routeert</em>.
De andere kant op moet je ook zelf regelen: als jij uitgaand belt komt het
gesprek op jouw server uit en is het aan jou om te zorgen dat het gesprek bij
de juiste persoon terechtkomt.</p>

<h4>SIP</h4>
<p>De techniek die hierachter zit is gebaseerd op het <em>Session Initiation
Protocol</em> (SIP). Er zijn twee richtingen die beide gebruikt worden bij
Do-It-Yourself: <em>inkomend</em> en <em>uitgaand</em>. Bij het bellen naar een
mobiel nummer op DIY wordt de term <em>inkomend</em> gebruikt. Bij het bellen
met de mobiele telefoon wordt er gesproken over <em>uitgaande</em> gesprekken.</p>

<p>Om telefoongesprekken af te leveren op jouw <em>Private Branch Exchange</em>
(PBX) wordt er een <dfn>SIP INVITE</dfn> naar jouw PBX verstuurd zodat er een sessie
opgebouwd kan worden tussen SpeakUp en jouw PBX. Hierdoor weet SpeakUp bij
welke machine het inkomende gesprek moeten worden afgeleverd.</p>

<p>De uitgaande gesprekken gaan ongeveer hetzelfde, maar er zit een subtiel
verschil in. Bij het opzetten van het gesprek moet er eerst een <dfn>SIP
INVITE</dfn> worden gestuurd vanaf SpeakUp naar de PBX van de klant. Daarna moet
de PBX het verder afhandelen. Er is een mogelijkheid om het gesprek weer terug
te sturen naar SpeakUp, alwaar zij het verder afhandelen. Dan stuurt de PBX een
<dfn>SIP INVITE</dfn> terug naar SpeakUp zodat het gesprek vanaf SpeakUp verder
kan oppakken en routeren</p>

<h4>Meer informatie</h4>
Op de <a href="https://secure.limesco.nl/wiki/Getting_started">wiki</a> kan je
voorbeeldconfiguraties vinden voor <a
href="https://secure.limesco.nl/wiki/Asterisk/Instellen">Asterisk</a> en <a
href="https://secure.limesco.nl/wiki/FreeSWITCH/Instellen">FreeSWITCH</a>.
