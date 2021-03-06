---
title: '''[!DNL Walmart] Voraussetzungen'
description: '"Vergewissern Sie sich, dass Sie über die erforderlichen [!DNL Walmart Marketplace]Informationen und Ressourcen zur Integration mit dem Kanal-Manager."'
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 4f0c40d7bcd05f7c8708d0d339cc29d920d646d5
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# [!DNL Walmart] Anforderungen

[!DNL Channel Manager] erfordert die folgenden Ressourcen und Informationen zum Konfigurieren eines [!DNL Commerce] Vertriebskanal für [!DNL Walmart Marketplace.]

* Genehmigung zum Verkauf [!DNL Walmart] und Anmeldedaten für die Anmeldung beim registrierten Marketplace Seller-Konto

* API-Schlüssel zum Verbinden von Adobe Commerce oder Magento Open Source mit [!DNL Walmart Marketplace]

   Die [!DNL Walmart Marketplace] API-Schlüssel ermöglicht die Integration zwischen [!DNL Channel Manager] für Adobe [!DNL Commerce] oder Magento Open Source und dem Walmart Marketplace. Richten Sie den API-Schlüssel in Seller Central ein, bevor Sie den Onboarding-Prozess für den Kanal-Manager starten.

## Richten Sie eine [!DNL Walmart Seller] account

1. [Senden Sie Ihre Walmart Seller-Anwendung](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
1. Nach Erteilung der Genehmigung durch [!DNL Walmart], [Einrichten Ihres Walmart Seller-Kontos](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

## Generieren Sie eine [!DNL Walmart Marketplace] Produktions-API-Schlüssel

1. Navigieren Sie zu [!DNL Walmart Marketplace] , um [API-Schlüssel für die Produktion von Lösungsanbietern für die Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Erstellen Sie den Schlüssel und konfigurieren Sie Berechtigungen:

   * Wählen Sie Adobe als Lösungsanbieter aus.

   * Legen Sie die Berechtigungen wie in der folgenden Tabelle gezeigt fest. Weitere Informationen finden Sie unter [API-Anmeldeinformationen](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) im _Walmart Marketplace Seller-Hilfe_.

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

## [!DNL Walmart Marketplace] Speicherstatus

Wenn Sie Produkte mit dem Marketplace verbinden, hängt die Verfügbarkeit der Liste vom Status Ihrer [!DNL Walmart Marketplace] Stores:

* Bei Live Stores werden Ihre Produktangebote aufgelistet und stehen zum Verkauf zur Verfügung, wenn der Match-Vorgang abgeschlossen ist.

* Bei Geschäften, die nicht live sind, werden Ihre Produktangebote gestaffelt und für Kunden nicht sichtbar. Wenn die [!DNL Walmart Marketplace] Store wird live geschaltet, gestaffelte Listen werden automatisch an den Live Store gesendet.

![[!DNL Walmart Seller Central] Staging-Produkte](assets/walmart-seller-central-staged.png)

>[!IMPORTANT]
>
>Nachher [!DNL Channel Manager] installiert und konfiguriert ist, werden alle Inventar-, Preis- und Bestellaktualisierungen automatisch synchronisiert. Keine Verbindung herstellen [!DNL Channel Manager] in einen Live-Walmart Marketplace-Speicher wechseln, bis Sie alle anderen Integrationen deaktiviert haben, die die Produkt- und Bestelldaten aktualisieren. Wenn Sie andere Integrationen konfiguriert haben, überprüfen Sie, ob die Artikelmenge und die Preise in [!DNL Commerce] entspricht den Mengen in [!DNL Walmart Marketplace] vor dem Herstellen einer Verbindung zu einem Live Store.

