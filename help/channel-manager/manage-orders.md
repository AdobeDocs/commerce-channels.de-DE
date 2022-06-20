---
title: '"Verwalten [!DNL Walmart Marketplace] Bestellungen"'
description: '"Anzeigen und Verwalten [!DNL Walmart Marketplace] Bestellungen mit [!DNL Channel Manager] für Adobe Commerce und Magento Open Source."'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: eb57189ed866fffa064867d1de5ae9db5b32e283
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 0%

---

# Verwalten [!DNL Walmart Marketplace] Bestellungen

[!DNL Walmart Marketplace] Bestelldaten für [!DNL Commerce] Produkte werden automatisch in [!DNL Channel Manager] after [!DNL Walmart] verarbeitet die Reihenfolge.

Auf der Seite &quot;Commerce&quot;werden bei einer erfolgreichen Synchronisation die folgenden Trigger angezeigt:

- [!DNL Channel Manager] sendet eine Auftragsbestätigung an Walmart.

- Eine entsprechende Commerce-Bestellung wird aus der Walmart-Bestellung erstellt.

- Die aktualisierten Bestellinformationen werden auf der Seite [!DNL Channel Manager] Dashboard &quot;Bestellungen&quot;.

In der Storefront-Admin können Sie Bestelldaten aus [!DNL Channel Manager] durch Öffnen des Verkaufskanalspeichers und Auswählen **[!UICONTROL Orders]**.

![Ansicht &quot;Channel Manager Bestellungen&quot;, die verwaltet werden soll [!DNL Walmart Marketplace] Bestellungen](assets/orders-dashboard-view.png)

>[!NOTE]
>
>Es kann bis zu 35 Minuten dauern für eine [!DNL Walmart Marketplace] Reihenfolge der Anzeige im [!DNL Channel Manager] Bestellliste. [!DNL Walmart] benötigt ca. 30 Minuten, um eingehende Bestellungen zu verarbeiten und an [!DNL Channel Manager]. Nachdem der Kanal-Manager die Bestellung erhalten hat, dauert es etwa fünf Minuten, bis die Bestellung in Adobe Commerce oder Magento Open Source erstellt und angezeigt wird.

## Bestellsteuerung und Spaltenbeschreibungen

In den folgenden Tabellen werden die für Bestellungen verfügbaren Steuerelemente und Spalten beschrieben.

**Steuerelemente für[!UICONTROL Orders]**
| **Kontrolle**                    | **Beschreibung**                                                                                                                                                                                                                                                                  | |—|—| | [!UICONTROL Filter orders]     | Sortieren Sie die Ansicht, indem Sie eine der [!UICONTROL Order Status] Karten.                                                                                                                                                                                                           | | Fehlerbeschreibung | Enthält detailliertere Informationen zu Bestellungen mit dem Fehlerstatus.                                                                                                                                                                                                            | | [!UICONTROL View order detail] | Um Bestelldetails anzuzeigen, wählen Sie die [!DNL Commerce] Bestellnummer im [!UICONTROL Order] Tabelle. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten.                                                                                                                    | | [!UICONTROL Channel Settings]  | Um die Kanalkonfiguration zu ändern, wählen Sie die Anmeldeinformationen für die Walmart Connection, zugeordnete Attribute oder Versandkennungen aus. Wählen Sie in den Einstellungen die Option [!DNL Commerce] Bestellnummer im [!UICONTROL Order] Tabelle. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten. |


**Spaltenbeschreibungen**

| Feld | Beschreibung |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Walmart Order Number] | Die Bestellnummer, die der Bestellung in der [!DNL Walmart Marketplace]. Beim erstmaligen Import einer Bestellung in [!DNL Channel Manager], wobei nur die [!DNL Walmart] Bestellnummer angezeigt. Wenn die [!DNL Commerce] -Reihenfolge erstellt wird, wird die [!DNL Walmart] Die Bestellnummer wird im [!UICONTROL External ID] Produktattribut. |
| [!DNL Commerce] Bestellnummer | Die der [!DNL Commerce] aus der [!DNL Walmart Marketplace] bestellen. |
| Elemente | Anzahl der bestellten Artikel [!DNL Walmart Marketplace]. |
| [!UICONTROL Order Value] | Gesamtkosten der bestellten Artikel. |
| [!UICONTROL Date Ordered] | Das Datum, an dem die Bestellung am [!DNL Walmart Marketplace]. |
| [!UICONTROL Ship By Date] | Datum, an dem die Bestellung versandt werden muss, um sie zu erfüllen [!DNL Walmart Marketplace] Anforderungen. |
| [!UICONTROL Deliver By Date] | Datum der Lieferung der Bestellung an den Kunden zur Erfüllung [!DNL Walmart Marketplace] Anforderungen im UTC-Format. |
| [!UICONTROL Ship Method] | Die [[!DNL Walmart Marketplace] Versandmethode](https://sellerhelp.walmart.com/s/guide?article=000007893) für die Bestellung ausgewählt wurde. |
| [!UICONTROL Last Update At] | Zeitstempel, der angibt, wann die Bestelldaten zuletzt in [!DNL Channel Manager] im UTC-Format. |
| [!UICONTROL Status] | Gibt den aktuellen Bestellstatus im [!DNL Commerce] Bestellworkflow. Der Anfangsstatus einer aus importierten Bestellung [!DNL Walmart Marketplace] is _Öffnen_. Zusätzliche Statusaktualisierungen treten auf, wenn Commerce-Bestellungen verarbeitet werden und [!DNL Channel Manager] Synchronisiert erfolgreich Versand-, Teillieferungs- und Löschaktualisierungen der [!DNL Walmart Marketplace]. |
| [!UICONTROL Error Description] | Detailliertere Informationen zu Bestellungen mit einer _[!UICONTROL Error]_Status. |

## Bestellstatus


[!UICONTROL Order Status] liefert Informationen zum aktuellen Status von [!DNL Walmart Marketplace] Bestellungen, die von Adobe Commerce oder Magento Open Source verwaltet werden. Aktualisierungen des Bestellstatus treten auf, wenn [!DNL Channel Manager] erhält aktualisierte Bestellinformationen von entweder [!DNL Walmart Marketplace] oder [!DNL Commerce] Bestellsystem. Bestellungen können den folgenden Status aufweisen:

- **[!UICONTROL Shipped]**-Bestellungen, die von der [!DNL Commerce] speichern. Wenn die Bestellung ausgeht, [!DNL Channel Manager] sendet eine Aktualisierung an [!DNL Walmart Marketplace] um den Versandstatus von Walmart zu aktualisieren und die Bestellnummer für die Sendung anzugeben.

- **[!UICONTROL Partially Shipped]**—Bestellungen, bei denen einige als versandt markierte Artikel und andere auf den Versand warten. Wenn Artikel in der Bestellung versandt werden, [!DNL Channel Manager] sendet eine Aktualisierung an [!DNL Walmart Marketplace] den Versandstatus zu aktualisieren, um ihn teilweise auf Walmart zu liefern, und die Auftragsverfolgungsnummer für die Sendung anzugeben.

- **[!UICONTROL Canceled]**-Bestellungen, die vom [!DNL Commerce] speichern.

   Nach Abschluss der Auftragsstornierung wird die [!DNL Commerce] Bestandsmengenaktualisierungen, um die zurückgegebenen Elemente widerzuspiegeln. Dann [!DNL Channel Manager] synchronisiert die Aktualisierung mit dem [!DNL Walmart Marketplace].

- **[!UICONTROL Error]**- Fehlerhafte Bestellungen. Fehler können auftreten, wenn ein Bestellaktualisierungsvorgang fehlschlägt. Beispielsweise treten Fehler auf, wenn [!DNL Channel Manager] kann keine neue Bestellung von Walmart erhalten. Sie können auch auftreten, wenn [!DNL Channel Manager] kann eine Auftragsversand- oder Löschungsaktualisierung nicht an die [!DNL Walmart Marketplace]. Wenn ein Vorgang fehlschlägt, wird auf der Seite &quot;Bestellungen&quot;eine _Fehler_ Status für die Bestellung. Weitere Informationen finden Sie unter [Bestellfehler beheben](process-orders.md#fix-shipping-and-cancel-errors).

- **[!UICONTROL Error description]**-Enthält detaillierte Informationen zu Bestellfehlern, die aufgrund von Problemen auftreten, wie fehlende Informationen oder ungültige Werte, falsche Versanddetails oder eine fehlgeschlagene Auftragsstornierung. Anhand der Beschreibung kann festgestellt werden, ob ein Fehler auf der [!DNL Commerce] -Instanz oder auf [!DNL Walmart Marketplace].

>[!NOTE]
>
>Wenn Bestellartikel in mehreren Sendungen gesendet werden, wird der Bestellstatus in [!DNL Channel Manager] spiegeln den letzten verfügbaren Bestellstatus wider. Wenn beispielsweise das erste Element ausgeliefert wird und keine Fehler zurückgegeben werden, wenn Bestellaktualisierungen mit [!DNL Channel Manager] und [!DNL Walmart Marketplace], die [!DNL Channel Manager] Bestellstatus: _[!UICONTROL Partially Shipped]_.  Wenn ein zweites Element versandt wird und [!CKanal-Manager] gibt einen Fehler zurück, der Auftragsstatus wird in_[!UICONTROL Error]_.

## Bestellungen überprüfen

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** , um [!UICONTROL Channel Manager Marketplace Stores] Seite.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol in einer Store-Einstiegszeile auswählen.

1. Um Bestellinformationen anzuzeigen, klicken Sie auf *[!UICONTROL *Orders]**.

1. Informationen über die Reihenfolge abrufen und die nächsten Schritte bestimmen, indem Sie die **[Status](#about-order-status)** -Spalte, um Informationen zu den Bestellungen zu erhalten.

## Bestelldetails anzeigen

Nachdem eine Bestellung vom Marktplatz empfangen und in die Adobe Commerce oder Magento Open Source importiert wurde, verwenden Sie die [!DNL Commerce] Bestell-ID zum Anzeigen der Bestellung in Adobe Commerce.

Von **[!UICONTROL Orders]**, wählen Sie die **[!UICONTROL Commerce Order Number]** , um [!DNL Commerce] Bestelldetails.

![Detailansicht einer Commerce-Bestellung für [!DNL Walmart Marketplace] order](assets/order-detail-with-external-order-id.png)

Im Commerce-Store werden aus importierte Bestellungen [!DNL Walmart Marketplace] die folgenden zusätzlichen Informationen in die Bestelldaten einschließen:

- **Zahlungsinformationen und Versandmethode**-Die von Walmart importierten Bestellungen enthalten folgende Werte für die Zahlungs- und Versandfelder:

   - **[!UICONTROL Offline Channel Payment]**—Gibt an, dass die Bestellungszahlung offline von [!DNL Walmart Marketplace].

   - **[!UICONTROL External Order Number]**—Zeigt die [!DNL Walmart Marketplace] Bestellnummer.

   - **[!UICONTROL Channel Shipping - Value]**-Gibt an, dass Versandgebühren über [!DNL Walmart Marketplace].

   - **[!UICONTROL Cancellation Reason]**-Dieses Feld wird nur angezeigt, wenn eine Bestellung aus [!DNL Walmart Marketplace] wird abgebrochen. Zu den Abbruchsgründen gehören:

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

