---
title: Amazon und der Commerce-Katalog
description: Der Amazon-Vertriebskanal importiert Ihre Amazon-Auflistungen in Ihr Commerce-Backend und synchronisiert sie kontinuierlich mit Produkten und Verkäufen.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# Amazon und die [!DNL Commerce] Katalog

Ihr Adobe Commerce- oder Magento Open Source-Backend enthält einen Katalog mit allen Produkten und zugehörigen Einstellungen und Informationen (Bilder, Optionen, Preise und mehr) sowie Konfigurationen für Bestellung und Versand. Ihre [!DNL Amazon Seller Central] -Konto verfügt auch über Katalog- und Bestellkonfigurationen, mit denen Sie Ihre Verkäufe durch [!DNL Amazon Marketplace].

Um Ihren Produktkatalog und Ihre Verkaufszahlen an einem Ort besser zu verwalten und zu überprüfen, importiert der Amazon-Vertriebskanal Ihre Amazon-Auflistungen in Ihre [!DNL Commerce] Backend, synchron mit Produkten und Verkäufen und meldet Probleme und Trends. Es unterstützt Integrationen mit mehreren [!DNL Amazon Seller Central] -Konten, die alle Daten über die zentrale Oberfläche für mehrere Storefronts verfolgen.

## Produktattribute

Adobe Commerce und Magento Open Source verwalten Katalogsynchronisierungen mit der Verwendung von Produkten [attributes](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) , um Produkteinstellungen und Daten zu definieren. Amazon verwendet auch Attribute, die über das Onboarding zugeordnet werden. Während [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md) Für den Amazon-Vertriebskanal definieren Sie bei Bedarf zusätzliche Amazon-Attribute, um beim Import Ihrer Amazon-Auflistungen in Ihre [!DNL Commerce] Katalog. Zu diesen Attributen gehören UPC, EAN, ISBN und ASIN ([!DNL Amazon Standard Identification Number]). Beim Onboarding werden Produkte zwischen Amazon und synchronisiert. [!DNL Commerce] Kataloge mit Ihren Attributen. Ordnungsgemäße Zuordnung Ihrer [!DNL Commerce] und Amazon-Produkte gewährleisten eine kontinuierliche Synchronisierung von Produktinformationen, Bestellungen und Beständen.

Wenn Sie diese Attribute nicht für Ihren Katalog erstellt oder konfiguriert haben, sollten Sie eine [!DNL Commerce] [Produktattribut](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) und -Werten für Ihre Produkte vor dem Onboarding. Wenn ein Amazon-Attribut importiert wird, kann es für Suche, Navigation, Preisregeln und vieles mehr verwendet werden. Siehe [Was bedeuten ASIN, UPC, EAN, ISBN, SKU und andere Barcodes?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

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

Die gesamte Synchronisierung wird von einer [Cron-Auftrag](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html)festgelegt ist, wird in der [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md).
