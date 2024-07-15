---
title: "Einführung in [!DNL Channel Manager]"
description: "Erfahren Sie, wie Sie [!DNL Channel Manager] installieren und verwenden, um Adobe Commerce- und Magento Open Source-Stores in den Walmart Marketplace zu integrieren und einen Vertriebskanal zu erstellen, über den Sie von Ihrem Commerce-Administrator aus nahtlos Marktplatzierungen, Preise, Lagerbestände und Verkäufe verwalten können."
role: Leader, Admin, User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 850aece134084e108b324a964d7d834042c7ddfd
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---


# Einführung in [!DNL Channel Manager]

[!DNL Channel Manager] hilft Händlern, den Umsatz zu steigern, neue Kunden zu erreichen, die Verkaufsvorgänge zu optimieren und Zeit zu sparen, indem ein Adobe Commerce- oder Magento Open Source-Produktkatalog in den [!DNL Walmart Marketplace] integriert wird.

![[!DNL Channel Manager] Erweiterung Admin view](assets/channel-manager-home.png){width="700" zoomable="yes"}

[!DNL Channel Manager] unterstützt Adobe Commerce- oder Magento Open Source-Händler, die mit [!DNL Walmart Marketplace] verkaufen möchten, indem sie den [!DNL Commerce] -Admin erweitern. Wenn [!DNL Channel Manager] installiert ist, können Store-Administratoren und -Betriebskräfte [!DNL Walmart Marketplace] -Umsätze, -Bestände und -Produktpreise nahtlos in der Commerce-Umgebung verwalten.

Der erweiterte Admin optimiert Vorgänge, da Händler dieselben Workflows und Prozesse verwenden können, um Verkäufe sowohl aus den [!DNL Commerce] Storefronts als auch aus dem Walmart Marketplace zu verwalten.

Nachdem Sie [!DNL Channel Manager] installiert und konfiguriert haben, können Sie die folgenden Funktionen verwenden, um Walmart Marketplace-Verkaufsaufträge zu verwalten:

* **Listing Management** - Stellen Sie einfach Produktlisten durch die Zuordnung von Produkten aus Ihrem [!DNL Commerce] -Katalog zu vorhandenen [!DNL Walmart Marketplace]-Listen zusammen.

* **Inventory management**-Elemente im Marktplatzierungskonto des Händlers werden automatisch synchronisiert und von [!DNL Commerce] aktualisiert, um eine genaue Bestandsaufnahme sicherzustellen.

* **Preisaktualisierungen** - Erhalten Sie genaue Preise für Marktplatzierungen mit automatischer Preissynchronisierung. Wenn sich ein Preis in Adobe Commerce ändert, werden die Änderungen auf dem Markt übernommen.

* **Auftragsverwaltung**: Wenn neue Bestellungen auf dem Markt erstellt werden, synchronisiert [!DNL Channel Manager] Bestellungen mit Adobe Commerce und sendet Bestellbestätigungen an den Marketplace. Diese Bestätigung stellt sicher, dass der Bestand für jede Bestellung reserviert ist. Der letzte Schritt besteht darin, die entsprechenden Bestellungen im System [!DNL Commerce] Order Management zur Verarbeitung zu erstellen.

* **Versandverwaltung**: Wenn Bestellungen in Adobe Commerce als versandt gekennzeichnet sind, wird die Versandaktualisierung an die [!DNL Walmart Marketplace] gesendet. Diese Benachrichtigung stellt sicher, dass die Verkäufer ihre SLA-Anforderungen erfüllen und dass Kunden Versandaktualisierungen für ihre aktuellen Bestellungen erhalten.

* **Stornierungen**: Wenn Bestellungen in Adobe Commerce storniert werden, sendet [!DNL Channel Manager] aktualisierte Bestellinformationen an den Marketplace, um die Aktion für die entsprechende Marketplace-Bestellung zu replizieren. Nach Abschluss der Auftragsstornierung wird die [!DNL Commerce] Lagermenge aktualisiert, um die zurückgegebenen Elemente und Bestandsaktualisierungen automatisch auf [!DNL Walmart Marketplace] zu synchronisieren.

* **Rückgabe und Rückerstattung**: Wenn Walmart Marketplace eine Rückgabe für Artikel anfordert, die über den Adobe Commerce- oder Magento Open Source-Vertriebskanal bestellt wurden, sendet [!DNL Channel Manager] die Rückgabe-Anfrageinformationen an den Commerce-Verkaufskanalspeicher, um die Rückgabeanforderung zu replizieren. Anschließend kann die Rückerstattung mit dem Offline-Workflow [!DNL Commerce] [Rückerstattung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html#refund-workflow) verarbeitet werden. Nachdem die Rückerstattung abgeschlossen ist, synchronisiert [!DNL Channel Manager] die Aktualisierung mit Walmart, sodass der Rückkehrstatus im Marktplatzierungskonto aktualisiert werden kann, um die Rückerstattung widerzuspiegeln.

## Erwartete Latenz für [!DNL Channel Manager]-Vorgänge

Die Datensynchronisierungsprozesse zwischen [!DNL Channel Manager] und einem verknüpften [!DNL Walmart Marketplace]-Store erfordern einige Zeit, um abgeschlossen zu werden. Überprüfen Sie die erwartete Verarbeitungszeit für [!DNL Channel Manager] -Vorgänge, um die Funktionsweise der Vertriebskanalvorgänge zu planen.

**Geschätzte Latenz für [!DNL Channel Manager] Vorgänge**

| **Vorgang** | **Beschreibung** | **Erwartete Verzögerung** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Produkte zu [!DNL Channel Manager] hinzufügen | Wählen Sie Produkte aus dem [!DNL Commerce] -Produktkatalog aus und importieren Sie sie in [!DNL Channel Manager]. | **Bis zu fünf Minuten** - Wenn Sie viele Produkte auswählen, z. B. einen gesamten Produktkatalog, dauert der Importvorgang länger. |
| Übereinstimmung mit Produkten mit [!DNL Walmart Marketplace] | Wählen Sie Produktlisten in [!DNL Channel Manager] aus und senden Sie sie zur Übereinstimmung an Walmart. | **Bis zu 30 Minuten** - Wenn Sie viele Produkte auswählen, dauert der entsprechende Vorgang je nach ausgewählter Menge länger. |
| Inventaraktualisierungen | Wenn sich die Lagerbestandsmenge in Commerce ändert, synchronisiert [!DNL Channel Manager] die Aktualisierung mit Walmart. | **Bis zu 10 Minuten** |
| Preisaktualisierungen | Wenn sich ein Produktpreis ändert, synchronisiert [!DNL Channel Manager] die Aktualisierung mit Walmart. | **Bis zu fünf Minuten** |
| Synchronisierungen von Walmart an [!DNL Commerce] bestellen | Der Kunde bestellt ein [!DNL Commerce] -Produkt auf dem Walmart Marketplace. Walmart sendet den Befehl an [!DNL Channel Manager]. Die Reihenfolge wird im Bestell-Dashboard angezeigt. | **Bis zu 30 Minuten** |
| In [!DNL Commerce] Order Management erstellte Bestellung | [!DNL Channel Manager] erstellt die [!DNL Commerce] -Bestellung aus der Walmart-Reihenfolge und aktualisiert das Bestell-Dashboard, sodass es die [!DNL Commerce] -Bestellnummer enthält. | **Bis zu fünf Minuten** |
| Aktualisierung des Versandstatus in [!DNL Commerce] Order Management | Wenn eine Bestellung aus Commerce versandt wird, aktualisiert [!DNL Channel Manager] den Versandstatus im Bestell-Dashboard und sendet die Aktualisierung an den Walmart Marketplace, damit der Kunde benachrichtigt werden kann. | **Bis zu fünf Minuten** |
| Aktualisierung der Auftragsstornierung in Commerce Order Management | Wenn eine Bestellung aus Commerce storniert wird, aktualisiert [!DNL Channel Manager] den Bestellstatus im Bestell-Dashboard und sendet die Aktualisierung an den Walmart Marketplace, damit der Kunde benachrichtigt werden kann. Nach Abschluss der Stornierung wird die Lagermenge von [!DNL Commerce] aktualisiert, um die zurückgegebenen Elemente widerzuspiegeln. Dann synchronisiert [!DNL Channel Manager] die Aktualisierung mit dem [!DNL Walmart Marketplace]. | **Bis zu fünf Minuten** |


