---
title: Info [!DNL Channel Manager]
description: Erfahren Sie, wie Sie installieren und verwenden [!DNL Channel Manager] , um Adobe Commerce- und Magento Open Source-Stores mit Drittanbieter-Marktplätzen zu integrieren und einen Vertriebskanal zu erstellen, um Marketplace-Listen, -Preise, -Bestands- und -verkäufe nahtlos über Ihren Commerce-Administrator zu verwalten.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 9ccd205ccd4f4b3f4e6b9fed2c4d16893f4b0da8
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---


# Info [!DNL Channel Manager]

[!DNL Channel Manager] hilft Ihnen, den Umsatz zu steigern und neue Kunden zu erreichen, indem Sie Ihren Adobe Commerce- oder Magento Open Source-Produktkatalog in die [!DNL Walmart US Marketplace].

![[!DNL Channel Manager] Admin-Ansicht der Erweiterung](assets/channel-manager-home.png)

Der Channel Manager unterstützt Adobe Commerce- oder Magento Open Source-Verkäufer, die auf dem Walmart Marketplace verkaufen möchten.

Nach der Installation und Konfiguration [!DNL Channel Manager], die [!DNL Commerce] Admin wird erweitert, damit Sie [!DNL Walmart Marketplace] Absatzvorgänge nahtlos aus Ihrer Commerce-Umgebung heraus.

* **Listenverwaltung**-Veröffentlichen Sie einfach Produktlisten, indem Sie Produkte aus Ihrem Commerce-Katalog mit vorhandenen Walmart Marketplace-Listen abgleichen.

* **Inventory management**-Elemente im Marketplace-Händlerkonto des Händlers werden automatisch synchronisiert und aus dem Handel aktualisiert, um eine präzise Bestandsaufnahme zu gewährleisten.

* **Preisaktualisierungen**- Erhalten Sie genaue Preise für Marktplatzierungen mit automatischer Preissynchronisierung. Wenn sich ein Preis in Adobe Commerce ändert, werden die Änderungen innerhalb von 10 Minuten auf dem Markt übernommen.

* **Auftragsverwaltung**-Wenn neue Bestellungen auf einem Marketplace erstellt werden, synchronisiert der Channel Manager Bestellungen mit Adobe Commerce und sendet Bestellbestätigungen an den Marketplace, um sicherzustellen, dass der Bestand für jede Bestellung reserviert ist.

* **Versandmanagement**-Wenn Bestellungen als in Adobe Commerce versandt gekennzeichnet sind, wird die Versandaktualisierung an die [!DNL Walmart Marketplace]. Diese Benachrichtigung stellt sicher, dass die Verkäufer ihre SLA-Anforderungen erfüllen und dass Kunden Versandaktualisierungen für ihre aktuellen Bestellungen erhalten.

* **Stornierungen**-Wenn Bestellungen in Adobe Commerce storniert werden, sendet der Channel Manager aktualisierte Bestellinformationen an den Marketplace, um die Aktion für die entsprechende Marketplace-Bestellung zu replizieren.

## Erwartete Latenz für den Kanal-Manager-Betrieb

Die Datensynchronisation zwischen [!DNL Channel Manager] und [!DNL Walmart Marketplace] -Store benötigt etwas Zeit, um abzuschließen. Überprüfen Sie die erwartete Verarbeitungszeit für [!DNL Channel Manager] Operationen, die die Planung des Betriebs von Vertriebskanälen erleichtern.

**Geschätzte Latenz bei Vorgängen im Kanalmanager**

| **Vorgang** | **Beschreibung** | **Erwartete Verzögerung** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Hinzufügen von Produkten zum Kanal-Manager | Wählen Sie Produkte aus dem Commerce-Produktkatalog aus und importieren Sie sie in den Kanal-Manager. | **Bis zu fünf Minuten**-Wenn Sie viele Produkte auswählen, z. B. einen gesamten Produktkatalog, dauert der Importvorgang länger. |
| Produkte auf dem Walmart Marketplace abgleichen | Wählen Sie Produktlisten im Kanal-Manager aus und senden Sie sie zur Übereinstimmung an Walmart. | **Bis zu 30 Minuten**-Wenn Sie viele Produkte auswählen, dauert der passende Prozess je nach ausgewählter Menge länger. |
| Inventaraktualisierungen | Wenn sich die Lagerbestandsmenge in Commerce ändert, [!DNL Channel Manager] synchronisiert die Aktualisierung mit Walmart. | **Bis zu 10 Minuten** |
| Preisaktualisierungen | Wenn sich ein Produktpreis ändert, synchronisiert der Channel Manager das Update mit Walmart. | **Bis zu fünf Minuten** |
| Synchronisierungen von Walmart an Commerce bestellen | Der Kunde bestellt ein Commerce-Produkt auf dem Walmart Marketplace. Walmart sendet die Bestellung an den Kanal-Manager. Die Reihenfolge wird im Bestell-Dashboard angezeigt. | **Bis zu 30 Minuten** |
| In der Commerce Order Management erstellte Bestellungen | Der Kanal-Manager erstellt die Commerce-Bestellung über die Walmart-Bestellung und aktualisiert das Bestell-Dashboard, sodass es die Commerce-Bestellnummer enthält. | **Bis zu fünf Minuten** |

