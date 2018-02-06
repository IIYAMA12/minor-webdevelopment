# Single-page vs multiple-page application (MPA)


## Voor en nadelen single-page applicatie (SPA)

### Voordelen
* Een single-page is heel snel. Na het downloaden van alle website code (HTML, CSS, Javascript), hoeft alleen de data/content heen en weer.
* De server hoeft niet meer de pagina te renderen, na dat deze gedownload is. Dat doet clientside nu. Jorik: `Wat waarschijnlijk inhoud dat er minder serverbelasting is op dat gebied.`
* Makkelijker te debuggen. Alle data is clientside, hierdoor kan je makkelijk data vergelijken met de elementen op het scherm. (Jorik: `Er hoeft dus minder gekeken te worden naar sessies op serverside.`)
* Deze applicatie slaat alles op in het geheugen van de client, dat de mogelijkheid bied om na de download de website offline te laten werken.

### Nadelen
* Het is moeilijk om deze voor de zoekmachine te optimaliseren. De zoekmachine van Google indexeert elke beschikbare pagina op het web. Maar zal moeite hebben met AJAX (Asynchronous Javascript en XML), omdat Google niet standaard weet wanneer de website geladen is en of het überhaupt dit zou kunnen downloaden/lezen.
* Bij het downloaden van de pagina wordt gelijk de hele website met frameworks gedownload. Dit is een relatieve grote download in vergelijking met maar één pagina te downloaden.
* Javascript is ten alle tijden benodigd. Mocht deze uitstaan dan kan de website niet geladen worden op de juiste wijzen.
* De applicatie is minder veilig. Omdat er veel data via voornamelijk AJAX gecommuniceerd wordt tussen client en server. Je moet dus meer ingangen dichtmaken. (In het gevonden artikel wordt ook het volgende gezegd: “it enables attackers to inject client-side scripts into web application by other users”. Hoe dit zou gebeuren wordt niet duidelijk uitgelegd.)
* Gevoeliger voor geheugen lekken van Javascript.

## Voor en nadelen multiple-page applicatie

### Voordelen
* Je houdt beter overzicht over de website.
* Goed en makkelijk voor zoekmachines om te doorgronden.

### Nadelen
* Frontend en backend zijn sterk van elkaar afhankelijk.
* Het uitvoeren van de website wordt complexer omdat de bouwer het framework clientside of serverside moet gaan gebruiken. Het kan daarom langer duren voordat de website klaar is.

[Bron: Single-page vs multiple-page application](https://medium.com/@NeotericEU/single-page-application-vs-multiple-page-application-2591588efe58)
