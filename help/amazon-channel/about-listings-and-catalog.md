---
title: Über Amazon und den Commerce-Katalog
description: Der Amazon-Vertriebskanal importiert Ihre Amazon-Auflistungen in Ihr Commerce-Backend und synchronisiert sie kontinuierlich mit Produkten und Verkäufen.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 5d30a5282ede2db0d9619eb2263b733328d26426
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Über Amazon und die [!DNL Commerce] Katalog

Ihr Adobe Commerce- oder Magento Open Source-Backend enthält einen Katalog mit allen Produkten und zugehörigen Einstellungen und Informationen (Bilder, Optionen, Preise und mehr) sowie Konfigurationen für Bestellung und Versand. Ihre [!DNL Amazon Seller Central] -Konto verfügt auch über Katalog- und Bestellkonfigurationen, mit denen Sie Ihre Verkäufe durch [!DNL Amazon Marketplace].

Um Ihren Produktkatalog und Ihre Verkaufszahlen an einem Ort besser zu verwalten und zu überprüfen, importiert der Amazon-Vertriebskanal Ihre Amazon-Auflistungen in Ihre [!DNL Commerce] Backend, synchron mit Produkten und Verkäufen und meldet Probleme und Trends. Es unterstützt Integrationen mit mehreren [!DNL Amazon Seller Central] -Konten, die alle Daten über die zentrale Oberfläche für mehrere Storefronts verfolgen.

## Produktattribute

Adobe Commerce und Magento Open Source verwalten Katalogsynchronisierungen mit der Verwendung von Produkten [attributes](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} zur Definition von Produkteinstellungen und Daten. Amazon verwendet auch Attribute, die über das Onboarding zugeordnet werden. Während [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md) Für den Amazon-Vertriebskanal definieren Sie bei Bedarf zusätzliche Amazon-Attribute, um beim Import Ihrer Amazon-Auflistungen in Ihre [!DNL Commerce] Katalog. Zu diesen Attributen gehören UPC, EAN, ISBN und ASIN ([!DNL Amazon Standard Identification Number]). Beim Onboarding werden Produkte zwischen Amazon und synchronisiert. [!DNL Commerce] Kataloge mit Ihren Attributen. Ordnungsgemäße Zuordnung Ihrer [!DNL Commerce] und Amazon-Produkte gewährleisten eine kontinuierliche Synchronisierung von Produktinformationen, Bestellungen und Beständen.

Wenn Sie diese Attribute nicht für Ihren Katalog erstellt oder konfiguriert haben, sollten Sie eine [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} und Werte zu Ihren Produkten vor dem Onboarding angeben. Wenn ein Amazon-Attribut importiert wird, kann es für Suche, Navigation, Preisregeln und vieles mehr verwendet werden. Siehe [Was bedeuten ASIN, UPC, EAN, ISBN, SKU und andere Barcodes?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target=&quot;_blank&quot;}

Nach dem Onboarding können Sie Ihre Produktattribute und Amazon-Zuordnungen jederzeit verwalten und aktualisieren.

## Produktlisten

Eine Amazon-Auflistung ist eine Produktseite für jedes Produkt, das Sie über [!DNL Amazon Marketplace], mit Produktbeschreibungen, Preisen, Bildern und mehr, die über Attribute zugeordnet sind. Während des Onboarding können Sie Ihre [!DNL Commerce] Produkte können automatisch in Amazon-Listen veröffentlicht werden. Sie können Ihre vorhandenen Amazon-Listen auch importieren, indem Sie sie Ihren [!DNL Commerce] Produkte.

Wenn Sie eine Liste erstellt haben [!DNL Commerce] Produkte, werden sie zur Genehmigung an Amazon übermittelt. Die meisten erfolgreichen Listen werden innerhalb weniger Stunden genehmigt. Wenn Ihre Liste genehmigt wurde, wird sie im [!DNL Amazon Marketplace] für sofortige Bestellungen von Kunden. Die [!DNL Amazon Sales Channel] -Erweiterung bietet eine Reihe von Registerkarten zum Überprüfen von Amazon-Listen. Je nach Problem oder den erforderlichen Daten sollten Sie Ihre [!DNL Amazon Seller Central] für spezifische Details zu diesen Auflistungen.

- [Aktiv](./active-listings.md): Listet genehmigte Produktlisten auf, die über den Marketplace verfügbar sind.

- [Listenbereit](./ready-to-list.md): Listet Produkte auf, die die Anforderungen an Regeln erfüllen und für die Veröffentlichung in Amazon bereit sind.

- [Inaktiv](./inactive-listings.md): Listet Produkte auf, die aufgrund der Blockierung aus einem bestimmten Grund (z. B. Branding-Problem), der Schließung und Anforderung von Zuverlässigkeit usw. nicht auf dem Markt verfügbar sind.

- [Nicht förderfähig](./ineligible-listings.md): Aufgrund der Listening-Regeln werden Produkte aufgelistet, die nicht aktiv auf dem Marketplace aufgeführt werden können (z. B. `0` Verkaufsdaten).

- [Unvollständig](./incomplete-listings.md): Listet Produkte auf, denen erforderliche Informationen fehlen. Aktualisieren Sie die Produktdaten für eine weitere Überprüfung.

- [Beendet](./ended-listings.md): Listet Produktlisten auf, die für eine Auflistung infrage kommen, aber manuell aus Amazon entfernt werden können. Sie können diese Produkte neu auflisten.

## Synchronisieren von Daten

Adobe Commerce und Magento Open Source kommunizieren Produkt- und Bestelldaten zwischen Ihren [!DNL Amazon Seller Central] und [!DNL Commerce] Backend. Die kontinuierlichen Aktualisierungen bieten eine einzige Quelle über [!DNL Commerce] die Verwaltung und Pflege Ihrer Lagerbestände, die Erfüllung von Bestellungen, die Rückverfolgung von Verkäufen sowie die Reduzierung von Aufwand und Doppelarbeit. Die Berichterstellung erfasst die neuesten Daten zur Verfolgung von Trends und zur Lösung von Kommunikationsproblemen, die zwischen den beiden Systemen auftreten.

Die gesamte Synchronisierung wird von einer [Cron-Auftrag](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}, so eingestellt, dass sie alle fünf Minuten in Ihrer [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md).
