---
title: Über Amazon und den Commerce-Katalog
description: Der Amazon-Vertriebskanal importiert Ihre Amazon-Auflistungen in Ihr Commerce-Backend und synchronisiert sie kontinuierlich mit Produkten und Verkäufen.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Über Amazon und den Katalog [!DNL Commerce]

Ihr Adobe Commerce- oder Magento Open Source-Backend enthält einen Katalog mit allen Produkten und zugehörigen Einstellungen und Informationen (Bilder, Optionen, Preise und mehr) sowie Konfigurationen für Bestellung und Versand. Ihr [!DNL Amazon Seller Central] -Konto verfügt auch über einen Katalog und eine Bestellkonfiguration, die Ihre Verkäufe über das [!DNL Amazon Marketplace] genau verfolgen.

Um Produktkatalog und -verkäufe an einem Ort besser zu verwalten und zu überprüfen, importiert der Amazon-Vertriebskanal Ihre Amazon-Auflistungen in Ihr [!DNL Commerce]-Backend, synchronisiert kontinuierlich mit Produkten und Verkäufen und meldet Probleme und Trends. Es unterstützt Integrationen mit mehreren [!DNL Amazon Seller Central]-Konten, die alle Daten über die einzige Oberfläche für mehrere Storefronts verfolgen.

## Produktattribute

Adobe Commerce und Magento Open Source verwalten Katalogsynchronisierungen mit der Verwendung von Produkt [attributes](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}, um Produkteinstellungen und Daten zu definieren. Amazon verwendet auch Attribute, die über das Onboarding zugeordnet werden. Bei [Aufgaben vor dem Setup](./amazon-pre-setup-tasks.md) für den Amazon-Vertriebskanal definieren Sie (bei Bedarf) zusätzliche Amazon-Attribute, um beim Import Ihrer Amazon-Auflistungen in Ihren [!DNL Commerce]-Katalog korrekte Produktzuordnungen sicherzustellen. Zu diesen Attributen gehören UPC, EAN, ISBN und ASIN ([!DNL Amazon Standard Identification Number]). Beim Onboarding werden Produkte mithilfe Ihrer Attribute zwischen Amazon- und [!DNL Commerce]-Katalogen synchronisiert. Eine ordnungsgemäße Zuordnung Ihrer [!DNL Commerce]- und Amazon-Produkte gewährleistet eine kontinuierliche Synchronisierung von Produktinformationen, Bestellungen und Beständen.

Wenn Sie diese Attribute nicht für Ihren Katalog erstellt oder konfiguriert haben, sollten Sie Ihren Produkten vor dem Onboarding einen [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} und Werte hinzufügen. Wenn ein Amazon-Attribut importiert wird, kann es für Suche, Navigation, Preisregeln und vieles mehr verwendet werden. Weitere Informationen zu diesen Attributen finden Sie unter [Amazon: Was sind UPCs, EANs, ISBNs und ASINs?](https://www.amazon.com/gp/seller/asin-upc-isbn-info.html){target=&quot;_blank&quot;}

Nach dem Onboarding können Sie Ihre Produktattribute und Amazon-Zuordnungen jederzeit verwalten und aktualisieren.

## Produktlisten

Eine Amazon-Auflistung ist eine Produktseite für jedes Produkt, das Sie über das [!DNL Amazon Marketplace] verkaufen, auf der Produktbeschreibungen, Preise, Bilder und mehr angezeigt werden, die über Attribute zugeordnet sind. Während des Onboarding können Sie Ihre [!DNL Commerce]-Produkte automatisch in Amazon-Listen veröffentlichen. Sie können Ihre vorhandenen Amazon-Listen auch importieren, indem Sie sie Ihren [!DNL Commerce]-Produkten zuordnen.

Wenn Sie eine Liste mit [!DNL Commerce] Produkten erstellt haben, werden diese zur Genehmigung an Amazon übermittelt. Die meisten erfolgreichen Listen werden innerhalb weniger Stunden genehmigt. Wenn Ihre Liste genehmigt wurde, erscheint sie im [!DNL Amazon Marketplace] für sofortige Bestellungen durch Kunden. Die [!DNL Amazon Sales Channel]-Erweiterung bietet eine Reihe von Registerkarten zum Überprüfen von Amazon-Listen. Abhängig vom Problem oder den erforderlichen Daten sollten Sie Ihr [!DNL Amazon Seller Central]-Konto auf spezifische Details zu diesen Listen überprüfen.

- [Aktiv](./active-listings.md): Listet genehmigte Produktlisten auf, die über den Marketplace verfügbar sind.

- [Bereit zum Auflisten](./ready-to-list.md): Listet Produkte auf, die den Anforderungen an Regeln entsprechen und für die Veröffentlichung in Amazon bereit sind.

- [Inaktiv](./inactive-listings.md): Listet Produkte auf, die aufgrund der Blockierung aus einem bestimmten Grund (z. B. Branding-Problem), der Schließung und Anforderung von Zuverlässigkeit usw. nicht auf dem Markt verfügbar sind.

- [Nicht zugelassen](./ineligible-listings.md): Führt Produkte, die nicht aktiv auf dem Markt aufgeführt werden können (z. B.  `0` Mengen- oder Verkaufsdaten), aufgrund der Listening-Regeln auf.

- [Unvollständig](./incomplete-listings.md): Listet Produkte auf, denen erforderliche Informationen fehlen. Aktualisieren Sie die Produktdaten für eine weitere Überprüfung.

- [Beendet](./ended-listings.md): Listet Produktlisten auf, die für eine Auflistung infrage kommen, aber manuell aus Amazon entfernt werden können. Sie können diese Produkte neu auflisten.

## Synchronisieren von Daten

Adobe Commerce und Magento Open Source kommunizieren Produkt- und Bestelldaten zwischen Ihrem [!DNL Amazon Seller Central]-Konto und dem [!DNL Commerce]-Backend. Die fortlaufenden Updates bieten eine zentrale Quelle bis [!DNL Commerce], um Ihre Lagerbestände zu verwalten und zu pflegen, Bestellungen zu erfüllen, Verkäufe zu verfolgen und Overheads und Doppelarbeit zu reduzieren. Die Berichterstellung erfasst die neuesten Daten zur Verfolgung von Trends und zur Lösung von Kommunikationsproblemen, die zwischen den beiden Systemen auftreten.

Die gesamte Synchronisierung wird von einem [cron-Auftrag](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;} verwaltet, der in [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md) alle fünf Minuten aktualisiert wird.
