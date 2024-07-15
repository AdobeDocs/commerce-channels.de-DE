---
title: Amazon und Commerce-Katalog
description: Der Amazon-Vertriebskanal importiert Ihre Amazon-Auflistungen in Ihr Commerce-Backend und synchronisiert sie kontinuierlich mit Produkten und Verkäufen.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services, Merchandising, Catalog Management
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Amazon und der [!DNL Commerce]-Katalog

Ihr Adobe Commerce- oder Magento Open Source-Backend enthält einen Katalog mit allen Produkten und zugehörigen Einstellungen und Informationen (Bilder, Optionen, Preise und mehr) sowie Konfigurationen für Bestellung und Versand. Ihr [!DNL Amazon Seller Central] -Konto verfügt außerdem über einen Katalog und eine Bestellkonfiguration, mit denen Sie Ihre Verkäufe über die [!DNL Amazon Marketplace] genau verfolgen können.

Um Ihren Produktkatalog und Ihre Verkaufszahlen an einem Ort besser zu verwalten und zu überprüfen, importiert der Amazon-Vertriebskanal Ihre Amazon-Auflistungen in Ihr [!DNL Commerce]-Backend, synchronisiert kontinuierlich mit Produkten und Verkäufen und meldet Probleme und Trends. Es unterstützt Integrationen mit mehreren [!DNL Amazon Seller Central] -Konten, wobei alle Daten über die einzige Oberfläche für mehrere Storefronts verfolgt werden.

## Produktattribute

Die Katalogverwaltung in Adobe Commerce und Magento Open Source erfolgt mithilfe von [Attributen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) des Produkts zur Definition von Produkteinstellungen und Daten. Amazon verwendet auch Attribute, die über das Onboarding zugeordnet werden. Während der [Aufgaben vor der Einrichtung ](./amazon-pre-setup-tasks.md) für den Amazon-Verkaufskanal definieren Sie (bei Bedarf) zusätzliche Amazon-Attribute, um beim Import Ihrer Amazon-Auflistungen in Ihren [!DNL Commerce] -Katalog korrekte Produktzuordnungen sicherzustellen. Zu diesen Attributen gehören UPC, EAN, ISBN und ASIN ([!DNL Amazon Standard Identification Number]). Beim Onboarding werden Produkte mithilfe Ihrer Attribute zwischen Amazon- und [!DNL Commerce]-Katalogen synchronisiert. Eine ordnungsgemäße Zuordnung Ihrer [!DNL Commerce]- und Amazon-Produkte gewährleistet eine kontinuierliche Synchronisierung von Produktinformationen, Bestellungen und Beständen.

Wenn Sie diese Attribute nicht für Ihren Katalog erstellt oder konfiguriert haben, sollten Sie Ihren Produkten vor dem Onboarding ein [!DNL Commerce] [Produktattribut](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) und Werte hinzufügen. Wenn ein Amazon-Attribut importiert wird, kann es für Suche, Navigation, Preisregeln und vieles mehr verwendet werden. Siehe [Was bedeuten ASIN, UPC, EAN, ISBN, SKU und andere Barcodes?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

Nach dem Onboarding können Sie Ihre Produktattribute und Amazon-Zuordnungen jederzeit verwalten und aktualisieren.

## Produktlisten

Eine Amazon-Auflistung ist eine Produktseite für jedes Produkt, das Sie über die [!DNL Amazon Marketplace] verkaufen, auf der Produktbeschreibungen, Preise, Bilder und mehr angezeigt werden, die über Attribute zugeordnet sind. Beim Onboarding können Sie konfigurieren, dass Ihre [!DNL Commerce] -Produkte automatisch in Amazon-Listen veröffentlicht werden. Sie können Ihre vorhandenen Amazon-Listen auch importieren, indem Sie sie Ihren [!DNL Commerce] -Produkten zuordnen.

Wenn Sie eine Liste mit [!DNL Commerce] Produkten erstellt haben, werden diese zur Genehmigung an Amazon übermittelt. Die meisten erfolgreichen Listen werden innerhalb weniger Stunden genehmigt. Wenn Ihre Liste genehmigt wurde, wird sie im [!DNL Amazon Marketplace] für sofortige Bestellungen durch Kunden angezeigt. Die Erweiterung [!DNL Amazon Sales Channel] enthält eine Reihe von Registerkarten zum Überprüfen von Amazon-Listen. Abhängig vom Problem oder den erforderlichen Daten sollten Sie Ihr [!DNL Amazon Seller Central]-Konto auf bestimmte Details zu diesen Auflistungen hin überprüfen.

- [Aktiv](./active-listings.md): Listet genehmigte Produktlisten auf, die über den Marketplace verfügbar sind.

- [ Bereit zur Liste](./ready-to-list.md): Listet Produkte auf, die die Regelanforderungen erfüllen und für die Veröffentlichung in Amazon bereit sind.

- [Inaktiv](./inactive-listings.md): Listet Produkte auf, die aufgrund der Blockierung aus einem bestimmten Grund (z. B. ein Branding-Problem), der Schließung und der Notwendigkeit einer Zuverlässigkeit usw. auf dem Marketplace nicht verfügbar sind.

- [Nicht zugelassen](./ineligible-listings.md): Führt aufgrund der Listening-Regeln Produkte auf, die nicht aktiv auf dem Markt aufgeführt werden können (z. B. `0` Mengenangaben oder Verkaufsdaten).

- [Uncomplete](./incomplete-listings.md): Listet Produkte auf, denen erforderliche Informationen fehlen. Aktualisieren Sie die Produktdaten für eine weitere Überprüfung.

- [Beendet](./ended-listings.md): Listet Produktlisten auf, die für eine Auflistung infrage kommen, aber manuell aus Amazon entfernt werden können. Sie können diese Produkte neu auflisten.

## Synchronisieren von Daten

Adobe Commerce und Magento Open Source kommunizieren Produkt- und Bestelldaten zwischen Ihrem [!DNL Amazon Seller Central] -Konto und dem [!DNL Commerce] -Backend. Die fortlaufenden Aktualisierungen bieten eine einzige Quelle bis [!DNL Commerce], um Ihre Lagerbestände zu verwalten und zu pflegen, Bestellungen zu erfüllen, Verkäufe zu verfolgen und Overheads und Doppelarbeit zu reduzieren. Die Berichterstellung erfasst die neuesten Daten zur Verfolgung von Trends und zur Lösung von Kommunikationsproblemen, die zwischen den beiden Systemen auftreten.

Die Synchronisierung wird von einem [cron-Auftrag](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) verwaltet, der alle fünf Minuten in Ihren [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md) aktualisiert wird.
