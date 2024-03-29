---
title: '''[!DNL Walmart] Voraussetzungen'
description: "Vergewissern Sie sich, dass Sie über die erforderlichen [!DNL Walmart Marketplace]Informationen und Ressourcen zur Integration mit dem Kanal-Manager."
role: Leader, Admin, Developer
feature: Sales Channels, Install, User Account, Tools and External Services
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# [!DNL Walmart] Voraussetzungen

[!DNL Channel Manager] erfordert die folgenden Ressourcen und Informationen zum Konfigurieren eines [!DNL Commerce] Vertriebskanal für [!DNL Walmart Marketplace.]

* A [!DNL Walmart] Verkäuferkonto

* API-Schlüssel zum Verbinden von Adobe Commerce oder Magento Open Source mit [!DNL Walmart Marketplace]

  Die [!DNL Walmart Marketplace] API-Schlüssel ermöglicht die Integration zwischen [!DNL Channel Manager] für Adobe [!DNL Commerce] oder Magento Open Source und dem Walmart Marketplace. Richten Sie den API-Schlüssel in Seller Central ein, bevor Sie den Onboarding-Prozess für den Kanal-Manager starten.

## Richten Sie eine [!DNL Walmart Seller] account

Navigieren Sie zu [!DNL Walmart Seller Center] , um [Walmart Seller-Konto](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

## Generieren Sie eine [!DNL Walmart Marketplace] Produktions-API-Schlüssel

1. Navigieren Sie zu [!DNL Walmart Marketplace] , um [API-Schlüssel für die Produktion von Lösungsanbietern für Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Erstellen Sie den Schlüssel und konfigurieren Sie Berechtigungen:

   * Wählen Sie Adobe als Lösungsanbieter aus.

   * Legen Sie die Berechtigungen wie in der folgenden Tabelle gezeigt fest. Weitere Informationen finden Sie unter [API-Anmeldeinformationen](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) im _Walmart Marketplace Seller-Hilfe_.

   **Adobe-API-Schlüsselkonfiguration für Walmart**

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

## [!DNL Walmart Marketplace] Speicherstatus

Wenn Sie Produkte mit dem Marketplace verbinden, hängt die Verfügbarkeit der Liste vom Status Ihrer [!DNL Walmart Marketplace] Stores:

* Bei Live Stores werden Ihre Produktangebote aufgelistet und stehen zum Verkauf zur Verfügung, wenn der Match-Vorgang abgeschlossen ist.

* Bei Geschäften, die nicht live sind, werden Ihre Produktangebote gestaffelt und für Kunden nicht sichtbar. Wenn die Variable [!DNL Walmart Marketplace] Store wird live geschaltet, gestaffelte Listen werden automatisch an den Live Store gesendet.

![[!DNL Walmart Seller Central] Staging-Produkte](assets/walmart-seller-central-staged.png){width="600" zoomable="yes"}

>[!IMPORTANT]
>
>Nachher [!DNL Channel Manager] installiert und konfiguriert ist, werden alle Inventar-, Preis- und Bestellaktualisierungen automatisch synchronisiert. Keine Verbindung herstellen [!DNL Channel Manager] in einen Live-Walmart Marketplace-Speicher wechseln, bis Sie alle anderen Integrationen deaktiviert haben, die die Produkt- und Bestelldaten aktualisieren. Wenn Sie andere Integrationen konfiguriert haben, überprüfen Sie, ob die Artikelmenge und die Preise in [!DNL Commerce] entspricht den Mengen in [!DNL Walmart Marketplace] vor dem Herstellen einer Verbindung zu einem Live Store.

