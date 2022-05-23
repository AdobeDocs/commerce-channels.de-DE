---
title: Info [!DNL Channel Manager]
description: Erfahren Sie, wie Sie installieren und verwenden [!DNL Channel Manager] , um Adobe Commerce- und Magento Open Source-Stores mit Drittanbieter-Marktplätzen zu integrieren und einen Vertriebskanal zu erstellen, um Marketplace-Listen, -Preise, -Bestands- und -verkäufe nahtlos über Ihren Commerce-Administrator zu verwalten.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: ef4c1362424285d4969fe173a0790809fccff80b
workflow-type: tm+mt
source-wordcount: '772'
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

## Walmart-Voraussetzungen

Sie benötigen die folgenden Informationen von Walmart, um Commerce in den Walmart Marketplace zu integrieren:

* Genehmigung zum Verkauf auf Walmart und Anmeldedaten für die Anmeldung beim registrierten Vertriebskonto für Marketplace

* API-Schlüssel zur Verbindung von Adobe Commerce oder Magento Open Source mit Walmart Marketplace

   Der Walmart Marketplace-API-Schlüssel ermöglicht die Integration zwischen dem Channel Manager für Adobe Commerce oder Magento Open Source und dem Walmart Marketplace. Richten Sie den API-Schlüssel in Seller Central ein, bevor Sie den Onboarding-Prozess für den Kanal-Manager starten.

### Einrichten eines Marketplace-Verkäuferkontos

1. [Senden Sie Ihre Walmart Seller-Anwendung](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
2. nach Genehmigung durch Walmart, [Einrichten Ihres Walmart Seller-Kontos](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

### Erstellen eines Walmart Marketplace-API-Schlüssels

1. Gehen Sie zu Walmart Marketplace , um eine [API-Schlüssel für die Produktion von Lösungsanbietern für die Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Erstellen Sie den Schlüssel und konfigurieren Sie Berechtigungen:

   * Wählen Sie Adobe als Lösungsanbieter aus.

   * Legen Sie die Berechtigungen wie in der folgenden Tabelle gezeigt fest. Weitere Informationen finden Sie unter [API-Anmeldeinformationen](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) im *[!DNL Walmart Marketplace]Hilfe zum Verkäufer*.

   **Adobe API-Schlüsselkonfiguration für Walmart**

   | **Berechtigung** | **Einstellung** |
   |----------------|-------------|
   | Inhalt | Vollständiger Zugriff |
   | Feeds abrufen | Nur anzeigen |
   | Bestand | Vollständiger Zugriff |
   | Elemente | Vollständiger Zugriff |
   | Startzeit | Vollständiger Zugriff |
   | Bestellung | Vollständiger Zugriff |
   | Preis | Vollständiger Zugriff |
   | Berichte | Nur anzeigen |
   | Rückgabe | Vollständiger Zugriff |
   | Regeln | Vollständiger Zugriff |
   | Versand | Vollständiger Zugriff |

## Walmart Marketplace Store-Status

Wenn Sie Produkte im Walmart Marketplace veröffentlichen, hängt die Verfügbarkeit der Liste vom Status Ihrer Walmart Marketplace-Stores ab:

* Bei Live Stores werden Ihre Produktangebote aufgelistet und stehen zum Verkauf zur Verfügung, wenn der Match-Vorgang abgeschlossen ist.

* Bei Geschäften, die nicht live sind, werden Ihre Produktangebote gestaffelt und für Kunden nicht sichtbar. Wenn der Store live geschaltet wird, werden Staging-Listen automatisch an den Live Store gesendet.


![[!DNL Walmart Seller Central] Staging-Produkte](assets/walmart-seller-central-staged.png)
