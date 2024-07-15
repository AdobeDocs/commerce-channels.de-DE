---
title: '[!DNL Walmart] Anforderungen'
description: "Stellen Sie sicher, dass Sie über die erforderlichen [!DNL Walmart Marketplace]Informationen und Ressourcen zur Integration mit dem Kanal-Manager verfügen."
role: Leader, Admin, Developer
feature: Sales Channels, Install, User Account, Tools and External Services
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# [!DNL Walmart] Voraussetzungen

[!DNL Channel Manager] erfordert die folgenden Ressourcen und Informationen, um einen [!DNL Commerce] -Verkaufskanal für [!DNL Walmart Marketplace.] zu konfigurieren

* Ein [!DNL Walmart] Verkäuferkonto

* API-Schlüssel zum Verbinden von Adobe Commerce oder Magento Open Source mit [!DNL Walmart Marketplace]

  Der API-Schlüssel [!DNL Walmart Marketplace] ermöglicht die Integration zwischen [!DNL Channel Manager] für Adobe [!DNL Commerce] oder Magento Open Source und dem Walmart Marketplace. Richten Sie den API-Schlüssel in Seller Central ein, bevor Sie den Onboarding-Prozess für den Kanal-Manager starten.

## Einrichten eines [!DNL Walmart Seller]-Kontos

Navigieren Sie zu &quot;[!DNL Walmart Seller Center]&quot;, um Ihr [Walmart Seller-Konto](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp) einzurichten.

## Generieren eines [!DNL Walmart Marketplace] Produktions-API-Schlüssels

1. Wechseln Sie zu [!DNL Walmart Marketplace] , um einen [API-Schlüssel für die Produktion des Lösungsanbieters für Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey) zu generieren.

1. Erstellen Sie den Schlüssel und konfigurieren Sie Berechtigungen:

   * Wählen Sie Adobe als Lösungsanbieter aus.

   * Legen Sie die Berechtigungen wie in der folgenden Tabelle gezeigt fest. Weitere Informationen finden Sie unter [API-Anmeldeinformationen](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) in der _Walmart Marketplace-Verkäuferhilfe_.

   **Adobe-API-Schlüsselkonfiguration für Walmart**

   | **Permission** | **Einstellen** |
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

## [!DNL Walmart Marketplace] Speicherstatus

Wenn Sie Produkte mit dem Marketplace verbinden, hängt die Verfügbarkeit der Liste vom Status Ihrer [!DNL Walmart Marketplace] Stores ab:

* Bei Live Stores werden Ihre Produktangebote aufgelistet und stehen zum Verkauf zur Verfügung, wenn der Match-Vorgang abgeschlossen ist.

* Bei Geschäften, die nicht live sind, werden Ihre Produktangebote gestaffelt und für Kunden nicht sichtbar. Wenn der [!DNL Walmart Marketplace] -Store live geschaltet wird, werden Staging-Listen automatisch an den Live Store gesendet.

![[!DNL Walmart Seller Central] Staged Products](assets/walmart-seller-central-staged.png){width="600" zoomable="yes"}

>[!IMPORTANT]
>
>Nachdem [!DNL Channel Manager] installiert und konfiguriert wurde, werden alle Bestands-, Preis- und Bestellaktualisierungen automatisch synchronisiert. Verbinden Sie [!DNL Channel Manager] erst dann mit einem Live-Walmart Marketplace-Store, wenn Sie andere Integrationen deaktiviert haben, die das Produkt und die Bestelldaten aktualisieren. Wenn Sie andere Integrationen konfiguriert haben, überprüfen Sie, ob die Artikelmenge und die Preise in [!DNL Commerce] mit den in [!DNL Walmart Marketplace] angegebenen Mengen übereinstimmen, bevor Sie eine Verbindung zu einem Live Store herstellen.

