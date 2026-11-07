# App-logo’s

Centrale logo’s voor de Onetoshop-appcatalogus. De aangeleverde 69 apps gebruiken 63 verschillende logo’s. De 63 oorspronkelijke bestanden zijn bytegelijk overgenomen; `riverty.svg` is daarnaast hergebruikt uit de bestaande Riverty-assets in deze repository.

De catalogus verwijst naar `https://static.xelshop.com/public/Apps/<bestandsnaam>`. Nieuwe namen gebruiken kleine letters; bestaande bestanden zijn behouden voor compatibiliteit met oudere verwijzingen. Fashion Cloud, DeepL, NE DistriService, Yuki en Exact Online krijgen duidelijkere bestandsnamen.

## Gebruik

1. Merge en publiceer deze assetwijziging voordat het bijgewerkte apps.json wordt geïmporteerd.
2. Gebruik daarna het bijgewerkte apps.json. De JSON blijft een lijst met dezelfde 69 app-ID’s en dezelfde velden.
3. De fijnere functionele indeling staat in `app-groups.json`. Dit is aanvullende catalogusmetadata; de bestaande admin leest deze indeling nog niet automatisch.

## Compatibiliteit

De huidige admin filtert op `apps.type`: 1 betalingen, 2 verzending, 3 marketing, 4 reviews, 5 social media, 6 boekhouding, 7 platformkoppelingen. Het bestaande `group`-veld bevat 0/1 en wordt niet als nieuwe categorie-enumeratie hergebruikt.

ID, type, group, access, function, link, guide, PHP-geserialiseerde fields en bestaande ingevulde slugs blijven ongewijzigd. Zeven lege slugs zijn aangevuld. Bestaande versies van DPD, TransMission, Rabobank en Sisow blijven herkenbaar als afzonderlijke aansluitingen.

## Redactionele correcties

- Betaalproviders en handmatige betaalmethoden krijgen afzonderlijke functionele groepen.
- Vervoerders, verzendplatformen en logistieke software worden onderscheiden.
- Datatrics valt onder marketing & personalisatie.
- bol.com en Marktplaats zijn verkoop-/advertentiekanalen; Fashion Cloud valt onder productdata en DeepL onder content & vertalingen.
- Google+ blijft als beëindigde integratie aanwezig om bestaande verwijzingen te behouden.
- AfterPay wordt weergegeven als Riverty / AfterPay, met Riverty-logo. De technische AfterPay-koppelingen zijn niet gemigreerd of opnieuw geactiveerd.
- De bestaande Twitter- en Multivers-logo’s zijn als oorspronkelijk beeldmateriaal behouden; de catalogusteksten maken de historische aansluiting herkenbaar.

Deze wijziging installeert, activeert of migreert geen providers en wijzigt geen klantinstellingen. Het volledige apps.json met technische formulierdefinities wordt niet gepubliceerd in deze publieke assetrepository.

## Bronnen voor merk- en statuscorrecties

- Aangeleverde apps.json en de bestaande shopintegraties.
- https://www.riverty.com/en/business/newsroom/riverty-starts-operations/
- https://support.google.com/chat/answer/14087009?hl=nl
- https://online.multivers.nl/HomeOld.aspx
- https://mail.quadient.com/nl/ressources/brochure-simplymail
- https://ne.nl/nl/onze-diensten
