---
title: '"Einführung in [!DNL Channel Manager]"'
description: Erfahren Sie, wie Sie installieren und verwenden [!DNL Channel Manager] , um Adobe Commerce- und Magento Open Source-Stores mit Drittanbieter-Marktplätzen zu integrieren und einen Vertriebskanal zu erstellen, um Marktplatzierungen, -preise, -inventare und -verkäufe nahtlos über Ihren Commerce-Administrator zu verwalten.
role: User
level: Intermediate
source-git-commit: ff87f31fec7a689385a93b8cab260fd93ff15f90
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---


# Übersicht

Der Kanalmanager für Adobe Commerce und Magento Open Source bietet einen praktischen Arbeitsbereich in der Admin-Konsole, um Kanalverkäufe auf Drittanbieter-Marktplätzen wie Walmart, Amazon und eBay zu verwalten. Steigern Sie den Umsatz und expandieren Sie auf neue Märkte, während Sie gleichzeitig den Betrieb Ihrer Vertriebskanäle nahtlos von Ihrem Commerce-Administrator aus verwalten.

![[!DNL Channel Manager] Admin-Ansicht der Erweiterung](assets/channel-manager-admin-entry-page.png)

## Beta-Version - Übersicht

Die Beta-Version von Channel Manager unterstützt Adobe Commerce- oder Magento Open Source-Verkäufer, die Produkte im Walmart Marketplace anbieten möchten.

Diese Version unterstützt die folgenden Funktionen zur Verwaltung von Vertriebskanalvorgängen:

* API-Verbindung zwischen Adobe Commerce oder Magento Open Source und Walmart Marketplace herstellen

* Veröffentlichen von Produkten aus dem Kanal-Manager in Walmart mithilfe der Produktzuordnung

* Anzeigen des Produktlistenstatus im Kanal-Manager, z. B. *Entwurf*, *Verarbeitung*, *passend*, *error*.

* Lagerbestandsmengen für übereinstimmende Produkte von Commerce nach Walmart synchronisieren

* Synchronisieren der Katalogpreise für passende Produkte von Commerce nach Walmart

* Bestellungen von Walmart Marketplace empfangen und im [!DNL Commerce] Dashboard für Bestellungen

### Erwartete Latenz für den Kanal-Manager-Betrieb

Die Datensynchronisation zwischen [!DNL Channel Manager] und [!DNL Walmart Marketplace] -Store benötigt etwas Zeit, um abzuschließen. Überprüfen Sie die erwartete Verarbeitungszeit für [!DNL Channel Manager] Operationen, die die Planung des Betriebs von Vertriebskanälen erleichtern.

**Geschätzte Latenz bei Vorgängen im Kanalmanager**
| **Vorgang**                              | **Beschreibung**                                                                                                                               | **Erwartete Verzögerung**                                                                                                        | |—|—|—| | Hinzufügen von Produkten zum Kanal-Manager | Wählen Sie Produkte aus dem Commerce-Produktkatalog aus und importieren Sie sie in den Channel Manager.                                                       | **Bis zu 5 Minuten**-Wenn Sie viele Produkte auswählen, z. B. einen gesamten Produktkatalog, dauert der Importvorgang länger. | | Übereinstimmung mit Produkten auf dem Walmart Marketplace | Wählen Sie Produktlisten im Kanal-Manager aus und senden Sie sie zur Übereinstimmung an Walmart.                                                                  | **Bis zu 30 Minuten**-Wenn Sie viele Produkte auswählen, dauert der passende Prozess je nach ausgewählter Menge länger.   | | Bestandsaktualisierungen | Wenn sich die Lagerbestandsmenge in Commerce ändert. Channel Manager synchronisiert Aktualisierung mit Walmart.                                                         | **Bis zu 10 Minuten**                                                                                                      | | Preisaktualisierungen | Wenn sich ein Produktpreis ändert, synchronisiert der Channel Manager das Update mit Walmart.                                                                    | **Bis zu 5 Minuten**                                                                                                       | | Auftragssynchronisierungen von Walmart zu Commerce | Der Kunde bestellt ein Commerce-Produkt auf dem Walmart Marketplace. Walmart sendet die Bestellung an den Kanal-Manager. Die Reihenfolge wird im Bestell-Dashboard angezeigt. | **Bis zu 30 Minuten**                                                                                                      | | Bestellung in der Commerce Order Management erstellt | Der Kanal-Manager erstellt die Commerce-Bestellung über die Walmart-Bestellung und aktualisiert das Bestell-Dashboard, sodass es die Commerce-Bestellnummer enthält.       | **Bis zu 5 Minuten**                                                                                                       |

## Walmart-Voraussetzungen

Sie benötigen die folgenden Informationen von Walmart, um Commerce in den Walmart Marketplace zu integrieren:

* Genehmigung zum Verkauf auf Walmart und Anmeldedaten für die Anmeldung beim registrierten Vertriebskonto für Marketplace

* API-Schlüssel zur Verbindung von Adobe Commerce oder Magento Open Source mit Walmart Marketplace

   Der Walmart Marketplace-API-Schlüssel ermöglicht die Integration zwischen dem Channel Manager für Adobe Commerce oder Magento Open Source und dem Walmart Marketplace. Richten Sie den API-Schlüssel in Seller Central ein, bevor Sie den Onboarding-Prozess für den Kanal-Manager starten.

### Einrichten eines Marketplace-Verkäuferkontos

1. [Senden Sie Ihre Walmart Seller-Anwendung](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)
2. nach Genehmigung durch Walmart, [Einrichten Ihres Walmart Seller-Kontos](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

### Erstellen eines Walmart Marketplace-API-Schlüssels

1. Gehen Sie zu Walmart Marketplace , um eine [API-Schlüssel für die Produktion von Lösungsanbietern für die Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Erstellen Sie den Schlüssel und konfigurieren Sie Berechtigungen:

   * Wählen Sie Adobe als Lösungsanbieter aus.

   * Legen Sie die Berechtigungen wie in der folgenden Tabelle gezeigt fest. Weitere Informationen finden Sie unter [API-Anmeldeinformationen](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) im _Walmart Marketplace Seller-Hilfe_.

|    **Adobe API-Schlüsselkonfiguration für Walmart**
| **Berechtigung** | **Einstellung** | |—|—| | Inhalt | Vollständiger Zugriff | | Feeds abrufen | Nur Ansicht | | Bestand | Vollständiger Zugriff | | Artikel | Vollständiger Zugriff | | Launch Time | Vollständiger Zugriff | | Bestellung | Vollständiger Zugriff | | Preis | Vollständiger Zugriff | | Berichte | Nur Ansicht | | Rückgabe | Vollständiger Zugriff | | Regeln | Vollständiger Zugriff | | Versand | Vollständiger Zugriff |

## Walmart Marketplace Store-Status

Wenn Sie Produkte im Walmart Marketplace veröffentlichen, hängt die Verfügbarkeit der Liste vom Status Ihrer Walmart Marketplace-Stores ab:

* Bei Live Stores werden Ihre Produktangebote aufgelistet und stehen zum Verkauf zur Verfügung, sobald der Match-Vorgang abgeschlossen ist.

* Bei Geschäften, die nicht live sind, werden Ihre Produktangebote gestaffelt und für Kunden nicht sichtbar. Sobald der Store live geschaltet wird, werden Staging-Listen automatisch an den Live Store gesendet.


![[!DNL Walmart Seller Central] Staging-Produkte](assets/walmart-seller-central-staged.png)
