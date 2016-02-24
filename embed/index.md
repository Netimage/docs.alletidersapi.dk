---
title: iFrame Embed documentation
layout: default
---

# Embed iFrame


For at få resultatet af flere temaer, tilføj hvert ønsket tema i iFrame src URLen.

	http://yourdomain.dk/embed/gallery?theme[]=1&theme[]=2&theme[]=3

	eller

	http://yourdomain.dk/embed/gallery/theme/1/theme/2/theme/3

Der kan stadig puttes andre parametre i URL'en sammen med flere temaer

	http://yourdomain.dk/embed/gallery/?theme[]=1&theme[]=2&limit=3&language=da-DK osv.

Og det er også muligt kunj at have et enkelt tema

	http://yourdomain.dk/embed/gallery/?theme=1

Mulige parametre:

	term		=[fritekst søgning]
	city		=[id på område]
	theme		=[id for tema]
	start-date	=[start dato i formatet dd/mm/yyyy]
	end-date	=[slut dato i formatet dd/mm/yyyy]
	limit		=[antal resultater der skal vises]
	language	=[sprog kode f.eks da-DK]

Eksempel på url med alle parametre:

	http://yourdomain.dk/embed/gallery/?term=weekend&city=432&theme[]=1&theme[]=2&start-date=28/02/2016&end-date=28/02/2016&limit=3&language=da-DK