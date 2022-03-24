---
title: Walmart-Voraussetzungen
description: Stellen Sie sicher, dass Sie über die erforderlichen Informationen und Ressourcen für den Walmart Marketplace verfügen, um sie in den Kanal-Manager zu integrieren.
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# Walmart-Voraussetzungen

Der Kanal-Manager benötigt die folgenden Ressourcen und Informationen, um einen Commerce-Vertriebskanal für Walmart Marketplace zu konfigurieren.

* Genehmigung zum Verkauf auf Walmart und Anmeldedaten für die Anmeldung beim registrierten Vertriebskonto für Marketplace

* API-Schlüssel zur Verbindung von Adobe Commerce oder Magento Open Source mit Walmart Marketplace

   Der Walmart Marketplace-API-Schlüssel ermöglicht die Integration zwischen dem Channel Manager für Adobe Commerce oder Magento Open Source und dem Walmart Marketplace. Richten Sie den API-Schlüssel in Seller Central ein, bevor Sie den Onboarding-Prozess für den Kanal-Manager starten.

## Einrichten eines Marketplace-Verkäuferkontos

1. [Senden Sie Ihre Walmart Seller-Anwendung](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)
1. nach Genehmigung durch Walmart, [Einrichten Ihres Walmart Seller-Kontos](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

## Erstellen eines Walmart Marketplace-API-Schlüssels

1. Gehen Sie zu Walmart Marketplace , um eine [API-Schlüssel für die Produktion von Lösungsanbietern für die Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Erstellen Sie den Schlüssel und konfigurieren Sie Berechtigungen:

   * Wählen Sie Adobe als Lösungsanbieter aus.

   * Legen Sie die Berechtigungen wie in der folgenden Tabelle gezeigt fest. Weitere Informationen finden Sie unter [API-Anmeldeinformationen](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) im _Walmart Marketplace Seller-Hilfe_.

|    **Adobe API-Schlüsselkonfiguration für Walmart**
| **Berechtigung** | **Einstellung** | |—|—| | Inhalt | Vollständiger Zugriff | | Feeds abrufen | Nur Ansicht | | Bestand | Vollständiger Zugriff | | Artikel | Vollständiger Zugriff | | Launch Time | Vollständiger Zugriff | | Bestellung | Vollständiger Zugriff | | Preis | Vollständiger Zugriff | | Berichte | Nur Ansicht | | Rückgabe | Vollständiger Zugriff | | Regeln | Vollständiger Zugriff | | Versand | Vollständiger Zugriff |

## Walmart Marketplace Store-Status

Wenn Sie Produkte im Walmart Marketplace veröffentlichen, hängt die Verfügbarkeit der Liste vom Status Ihrer Walmart Marketplace-Stores ab:

* Bei Live Stores werden Ihre Produktangebote aufgelistet und stehen zum Verkauf zur Verfügung, wenn der Match-Vorgang abgeschlossen ist.

* Bei Geschäften, die nicht live sind, werden Ihre Produktangebote gestaffelt und für Kunden nicht sichtbar. Wenn der Store live geschaltet wird, werden Staging-Listen automatisch an den Live Store gesendet.

![[!DNL Walmart Seller Central] Staging-Produkte](assets/walmart-seller-central-staged.png)
