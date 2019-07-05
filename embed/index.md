---
title: iFrame Embed documentation
layout: default
---

# Embed iFrame

Alletiders API stiller nogle specielle sider tilgængelig som er målrettet efter iframe embedding. 
I det følgende er der beskrevet hvilke muligheder man har hvis man ønsker at bruge iframe embedding af sin salgkanal. 

I eksemplerne forneden er der som URL anvendt http://yourdomain.dk/embed - dette skal ændres til den rette salgskanal URL, som man ønsker vist i iframen. 
Alletiders API's standard url for en salgskanal embed er som følgende, hvor X erstattes med salgskanal id'en:
    
    https://channel-X.pebc.combineservices.dk/embed  

## iFrame HTML
For at kunne vise en salgskanal via en iframe skal der indsættes en html kode ind på hjemmesiden - dér hvor man ønsker at få vist salgkanal indholdet. 

En simpel iframe kode kunne se således ud:

    <iframe src="https://yourdomain.dk/embed" height="400" width="600"></iframe>
    
Denne kode vil vise en iframe med en højde på 400px og bredde på 600px. 

Ønskes der yderligere tilpasninger af iframen i form af andre parametre, findes der rigtig mange eksempler på internettet.

## Search

	https://yourdomain.dk/embed/search

Giver muligheden for at vise et søgefelt som vil søge efter produkter på det angivne domæne.

## List

	https://yourdomain.dk/embed/list
	
Giver muligheden for at vise en liste over produkter.

Mulige parametre:

	city		=[id på område]
	theme		=[id for tema]
	limit		=[antal resultater der skal vises]
	distanceLimit	=[afgrænsning af udsøgningsområde i km]
	excludeTheme    =[id for temaer, som man ikke ønsker resultater fra]
	
Eksempel på url med parametre:

	https://yourdomain.dk/embed/gallery/?city=432&theme[]=1&limit=3&distanceLimit=50

For at få resultatet af flere temaer, tilføj hvert ønsket tema i iFrame src URLen.

	https://yourdomain.dk/embed/gallery?theme[]=1&theme[]=2&theme[]=3

	eller

	https://yourdomain.dk/embed/gallery/theme/1/theme/2/theme/3

Der kan stadig puttes andre parametre i URL'en sammen med flere temaer

	https://yourdomain.dk/embed/gallery/?theme[]=1&theme[]=2&limit=3&language=da-DK osv.

Og det er også muligt kun at have et enkelt tema

	https://yourdomain.dk/embed/gallery/?theme=1
	
Ønsker man derimod at vise resultater fra alle temaer pånær nogle enkelte, kan parameteren `excludeTheme` med fordel benyttes.
    
    https://yourdomain.dk/embed/gallery/?city=432&excludeTheme[]=1&limit=3&distanceLimit=50

## Gallery

	https://yourdomain.dk/embed/gallery

Giver muligheden for at vise produktmoduler med billeder. Der kan i gallery anvendes de samme parametre, som nævnt under liste visningen.