---
title: Über Amazon und den Commerce-Katalog
description: Der Amazon Sales Kanal importiert Ihre Amazon-Auflistungen in Ihr Commerce-Backend und synchronisiert sie kontinuierlich mit Produkten und Verkäufen.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Über Amazon und [!DNL Commerce] Katalog

Ihr Adobe Commerce- oder Magento Open Source-Backend enthält einen Katalog mit allen Produkteinstellungen und zugehörigen Einstellungen und Informationen (Bilder, Optionen, Preise und mehr) sowie Konfigurationen für Bestellung und Versand. Ihre [!DNL Amazon Seller Central] hat auch einen Katalog und Auftragskonfigurationen, die ausschließlich Ihren Umsatz durch [!DNL Amazon Marketplace].

Um den Produktkatalog und den Vertrieb über einen Standort besser zu verwalten und zu überprüfen, importiert Amazon Sales Kanal Ihre Amazon-Auflistungen in Ihre [!DNL Commerce] Backend, synchron mit Produkten und Verkäufen, meldet Probleme und Trends. Es unterstützt Integrationen mit mehreren [!DNL Amazon Seller Central] -Konten, die alle Daten über die einzige Oberfläche für mehrere Stores verfolgen.

## Produktattribute

Adobe Commerce und Magento Open Source verwalten Katalogsynchronisierungen mit Produktverwendung [Attribute](https://docs.magento.com/user-guide/catalog/product-attributes.html){Zielgruppe=&quot;_blank&quot;} zum Definieren von Produkteinstellungen und -daten. Amazon verwendet auch Attribute, die über das Einsteigen zugeordnet werden können. Während [Aufgaben vor dem Setup](./amazon-pre-setup-tasks.md) für Amazon Sales Kanal definieren Sie zusätzliche Amazon-Attribute (falls erforderlich), um beim Import Ihrer Amazon-Einträge in Ihre [!DNL Commerce] Katalog. Zu diesen Attributen gehören UPC, EAN, ISBN und ASIN ([!DNL Amazon Standard Identification Number]). Durch Einstieg werden die Produkte zwischen Amazon und [!DNL Commerce] Kataloge mit Ihren Attributen. Richtige Zuordnung Ihrer [!DNL Commerce] und Amazon-Produkte sorgen für eine kontinuierliche Synchronisation von Produktinformationen, Bestellungen und Lagerbeständen.

Wenn Sie diese Attribute nicht für Ihren Katalog erstellt oder konfiguriert haben, sollten Sie einen [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){Zielgruppe=&quot;_blank&quot;} und Werte für Ihre Produkte vor dem Einstieg. Wenn ein Amazon-Attribut importiert wird, kann es für die Suche, Navigation, Preisregeln und vieles mehr verwendet werden. Weitere Informationen zu diesen Attributen finden Sie unter [Amazon: Was sind UPCs, EANs, ISBNs und ASINs?](https://www.amazon.com/gp/seller/asin-upc-isbn-info.html){Zielgruppe=&quot;_blank&quot;}

Nach dem Einstieg können Sie Ihre Produktattribute und Amazon-Zuordnungen jederzeit verwalten und aktualisieren.

## Produktlisten

Eine Amazon-Auflistung ist eine Produktseite für jedes Produkt, das Sie über [!DNL Amazon Marketplace], in dem Produktbeschreibungen, Preise, Bilder und vieles mehr angezeigt werden, die über Attribute zugeordnet sind. Während des Boarding können Sie Ihre [!DNL Commerce] Produkte können automatisch in Amazon-Listen veröffentlicht werden. Sie können Ihre vorhandenen Amazon-Listen auch importieren, indem Sie sie Ihren [!DNL Commerce] Produkte.

Wenn Sie eine Auflistung erstellt haben [!DNL Commerce] werden sie Amazon zur Genehmigung vorgelegt. Die meisten erfolgreichen Auflistungen werden innerhalb weniger Stunden genehmigt. Wenn Ihre Liste genehmigt wurde, wird sie im [!DNL Amazon Marketplace] für Sofortbestellungen durch Kunden. Die [!DNL Amazon Sales Channel] -Erweiterung bietet eine Reihe von Registerkarten zur Überprüfung von Amazon-Auflistungen. Je nach Problem oder den erforderlichen Daten sollten Sie Ihre [!DNL Amazon Seller Central] für spezifische Details in diesen Listen.

- [Aktiv](./active-listings.md): Listen genehmigte Produktauflistungen auf dem Markt verfügbar.

- [Bereit für Liste](./ready-to-list.md): Listen von Produkten, die die Anforderungen der Listening-Regeln erfüllen und auf Amazon veröffentlicht werden können.

- [Inaktiv](./inactive-listings.md): Liste von Produkten, die auf dem Markt nicht verfügbar sind, weil sie aus einem bestimmten Grund blockiert wurden (z. B. Markenproblematik), geschlossen sind und eine erneute Überprüfung erfordern usw.

- [Nicht förderfähig](./ineligible-listings.md): Aufgrund der Listungsregeln können Listen Produkte, die nicht aktiv auf dem Markt aufgeführt werden können (z. B. `0` Verkaufsdaten).

- [Unvollständig](./incomplete-listings.md): Listen-Produkte fehlen erforderliche Informationen. Aktualisieren Sie die Produktdaten für eine andere Überprüfung.

- [Beendet](./ended-listings.md): Listen von Produktauflistungen, die für eine Auflistung infrage kommen, aber manuell aus Amazon entfernt wurden. Sie können diese Produkte neu auflisten.

## Daten werden synchronisiert

Adobe Commerce und Magento Open Source kommunizieren Produkt- und Bestelldaten zwischen Ihren [!DNL Amazon Seller Central] und [!DNL Commerce] Backend. Die kontinuierlichen Aktualisierungen bieten eine einzige Quelle durch [!DNL Commerce] Ihre Bestände zu verwalten und zu pflegen, Aufträge zu erfüllen, Verkäufe zu verfolgen und den Aufwand und die Doppelarbeit zu reduzieren. Berichte erfasst die neuesten Daten zur Verfolgung von Trends und zur Behebung von Kommunikationsproblemen, die zwischen den beiden Systemen auftreten.

Alle Synchronisierungen werden von einem [cron job](https://docs.magento.com/user-guide/system/cron.html){Zielgruppe=&quot;_blank&quot;}, eingestellt auf alle fünf Minuten in Ihrem [Aufgaben vor dem Setup](./amazon-pre-setup-tasks.md).
