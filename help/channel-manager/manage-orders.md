---
title: '"Anzeigen und Verwalten von Bestellungen aus [!DNL Channel Manager]'''
description: "Anzeigen und Verwalten [!DNL Walmart Marketplace] Bestellungen mit [!DNL Channel Manager] für Adobe Commerce und Magento Open Source."
feature: Sales Channels, Orders
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Anzeigen und Verfolgen von Bestellungen von [!DNL Channel Manager]

[!DNL Walmart Marketplace] Bestelldaten für [!DNL Commerce] Produkte werden automatisch in [!DNL Channel Manager] after [!DNL Walmart] verarbeitet die Reihenfolge.

Im [!DNL Commerce] bei erfolgreicher Synchronisierung werden die folgenden Trigger ausgeführt:

- [!DNL Channel Manager] sendet eine Auftragsbestätigung an Walmart.

- Eine entsprechende [!DNL Commerce] -Bestellung wird aus der Walmart-Bestellung erstellt.

- Die aktualisierten Bestellinformationen werden auf der Seite [!DNL Channel Manager] Dashboard &quot;Bestellungen&quot;.

In der Storefront-Admin können Sie Bestelldaten aus [!DNL Channel Manager] durch Öffnen des Verkaufskanalspeichers und Auswählen **[!UICONTROL Orders]**.

![Ansicht &quot;Channel Manager Bestellungen&quot;, die verwaltet werden soll [!DNL Walmart Marketplace] Bestellungen](assets/orders-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>Es kann bis zu 35 Minuten dauern für eine [!DNL Walmart Marketplace] Reihenfolge der Anzeige im [!DNL Channel Manager] Bestellliste. [!DNL Walmart] benötigt ca. 30 Minuten, um eingehende Bestellungen zu verarbeiten und an [!DNL Channel Manager]. Nachdem der Kanal-Manager die Bestellung erhalten hat, dauert es etwa fünf Minuten, bis die Bestellung in Adobe Commerce oder Magento Open Source erstellt und angezeigt wird.

## Bestellsteuerung und Spaltenbeschreibungen

In den folgenden Tabellen werden die für Bestellungen verfügbaren Steuerelemente und Spalten beschrieben.

**Steuerelemente für[!UICONTROL Orders]**

<table>
<tr>
<td><strong>Kontrolle</strong></td>
<td><strong>Beschreibung</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>Sortieren Sie die Ansicht, indem Sie eine der [!UICONTROL Order Status] Karten.</td>
</tr>
<tr>
<td>Statusdetails</td>
<td>Enthält Informationen zu Bestellfehlern und Rückgabeanfragen. Um Rückkehrinformationen und den Rückerstattungsstatus für eine Bestellung anzuzeigen, wählen Sie die <strong>[!UICONTROL Return requested]</strong> Text zum Öffnen [!UICONTROL Returns] Dashboard.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Um Bestelldetails anzuzeigen, wählen Sie die [!DNL Commerce] Bestellnummer im [!UICONTROL Order] Tabelle. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Um die Kanalkonfiguration zu ändern, wählen Sie die Anmeldeinformationen der Walmart Connection, zugeordnete Attribute oder Versandkennungen aus. Wählen Sie in den Einstellungen die Option [!DNL Commerce] Bestellnummer im [!UICONTROL Order] Tabelle. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten.</td>
</tr>
</table>


**Spaltenbeschreibungen**

<table>
<tr>
<td>Feld</td>
<td>Beschreibung</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>Die Bestellnummer, die der Bestellung in der [!DNL Walmart Marketplace]. Beim erstmaligen Import einer Bestellung in [!DNL Channel Manager], wobei nur die [!DNL Walmart] Bestellnummer angezeigt. Wenn die [!DNL Commerce] -Reihenfolge erstellt wird, wird die [!DNL Walmart] Die Bestellnummer wird im [!UICONTROL External ID] Produktattribut.</td>
</tr>
<tr>
<td>[!DNL Commerce] Bestellnummer</td>
<td>Die der [!DNL Commerce] aus der [!DNL Walmart Marketplace] bestellen.</td>
</tr>
<tr>
<td>Elemente</td>
<td>Anzahl der bestellten Artikel [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>Gesamtkosten der bestellten Artikel.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>Das Datum, an dem die Bestellung eingereicht wurde [!DNL Walmart Marketplace] in die lokale Zeitzone konvertiert wurde.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>Das Datum, an dem die Bestellung versandt werden muss, um die Anforderungen zu erfüllen [!DNL Walmart Marketplace] Anforderungen, die in die lokale Zeitzone konvertiert wurden.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>Das Datum, an dem die Bestellung an den Kunden geliefert werden muss, um erfüllt zu werden [!DNL Walmart Marketplace] Anforderungen, die in die lokale Zeitzone konvertiert wurden.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>Die [[!DNL Walmart Marketplace] Versandmethode](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29 für die Bestellung ausgewählt.</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>Zeitstempel, der angibt, wann die Bestelldaten zuletzt in [!DNL Channel Manager] in die lokale Zeitzone konvertiert wurde.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Gibt den aktuellen Bestellstatus im [!DNL Commerce] Bestellworkflow. Der Anfangsstatus einer aus importierten Bestellung [!DNL Walmart Marketplace] ist _Open_. Zusätzliche Statusaktualisierungen treten auf, wenn [!DNL Commerce] Bestellungen werden verarbeitet und [!DNL Channel Manager] Synchronisiert erfolgreich Versand-, Teillieferungs- und Löschaktualisierungen der [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Enthält detailliertere Informationen zu Bestellungen mit Fehlern oder Erstattungsanfragen.</td>
</tr>
</table>

## Bestellstatus

[!UICONTROL Order Status] liefert Informationen zum aktuellen Status von [!DNL Walmart Marketplace] Bestellungen, die von Adobe Commerce oder Magento Open Source verwaltet werden. Aktualisierungen des Bestellstatus treten auf, wenn [!DNL Channel Manager] erhält aktualisierte Bestellinformationen von entweder [!DNL Walmart Marketplace] oder [!DNL Commerce] Bestellsystem. Bestellungen können den folgenden Status aufweisen:

- **[!UICONTROL Shipped]**—Bestellungen, die von der [!DNL Commerce] speichern. Wenn die Bestellung ausgeht, [!DNL Channel Manager] sendet eine Aktualisierung an [!DNL Walmart Marketplace] um den Versandstatus von Walmart zu aktualisieren und die Bestellnummer für die Sendung anzugeben. Nach dem Versand einer Bestellung können Bestellungen teilweise oder vollständig zurückerstattet werden, wenn Walmart ein Formular zur Genehmigung der Rücksendung ausstellt. Siehe [Rückgaben und Erstattungen](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]**—Bestellungen, bei denen einige als versandt markierte Artikel und andere auf den Versand warten. Wenn Artikel in der Bestellung versandt werden, [!DNL Channel Manager] sendet eine Aktualisierung an [!DNL Walmart Marketplace] , um den Versandstatus auf _[!DNL Partially Shipped]_auf Walmart und geben Sie die Bestellnummer für die Sendung an.

- **[!UICONTROL Canceled]**—Bestellungen, die vom [!DNL Commerce] speichern.

  Nach Abschluss der Auftragsstornierung wird die [!DNL Commerce] Bestandsmengenaktualisierungen, um die zurückgegebenen Elemente widerzuspiegeln. Dann [!DNL Channel Manager] synchronisiert die Aktualisierung mit dem [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]**—Wenn Walmart Marketplace eine Rückgabe für die gelieferten Bestellartikel anfordert, wird ein `Return requested` Der Link wird in [!UICONTROL Status details] Spalte. Wenn Sie den Link auswählen, wird der [!UICONTROL Returns] Dashboard, um die Rückgabe anzuzeigen und den Rückerstattungsprozess zu verwalten.

- **[!UICONTROL Error]**—Bestellungen mit Fehlern. Fehler können auftreten, wenn ein Bestellaktualisierungsvorgang fehlschlägt. Beispielsweise treten Fehler auf, wenn [!DNL Channel Manager] kann keine neue Bestellung von Walmart erhalten. Sie können auch auftreten, wenn [!DNL Channel Manager] kann eine Auftragsversand- oder Löschungsaktualisierung nicht an die [!DNL Walmart Marketplace]. Wenn ein Vorgang fehlschlägt, wird auf der Seite &quot;Bestellungen&quot;eine _Fehler_ Status für die Bestellung. Weitere Informationen finden Sie unter [Bestellfehler beheben](process-orders.md#fix-shipping-and-cancel-errors).

- **[!UICONTROL Status details]**-Bietet weitere Informationen zu Bestellfehlern, die aufgrund von Problemen auftreten, wie fehlende Informationen oder ungültige Werte, falsche Versanddetails oder eine fehlgeschlagene Auftragsstornierung. Anhand der Beschreibung kann festgestellt werden, ob ein Fehler auf der [!DNL Commerce] -Instanz oder auf [!DNL Walmart Marketplace].

>[!NOTE]
>
>Wenn Bestellartikel in mehreren Sendungen gesendet werden, wird der Bestellstatus in [!DNL Channel Manager] spiegelt den letzten verfügbaren Bestellstatus wider. Wenn beispielsweise das erste Element ausgeliefert wird und keine Fehler zurückgegeben werden, wenn Bestellaktualisierungen mit [!DNL Channel Manager] und [!DNL Walmart Marketplace], die [!DNL Channel Manager] Bestellstatus: _[!UICONTROL Partially Shipped]_. Wenn ein zweites Element versandt wird und [!DNL Channel Manager] gibt einen Fehler zurück, der Auftragsstatus wird in_[!UICONTROL Error]_.

## Bestellungen überprüfen

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** , um [!UICONTROL Channel Manager Marketplace Stores] Seite.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol in einer Store-Einstiegszeile auswählen.

1. Um Bestellinformationen anzuzeigen, klicken Sie auf *[!UICONTROL *Orders]**.

1. Informationen über die Reihenfolge abrufen und die nächsten Schritte bestimmen, indem Sie die **[Status](#order-status)** Spalte.

## Details zur Bestellung überprüfen

Nachdem eine Bestellung vom Marketplace empfangen und in Ihren Vertriebskanalspeicher importiert wurde, verwenden Sie die [!DNL Commerce] Bestell-ID zum Anzeigen der Auftragsdetails in Adobe Commerce.

Von **[!UICONTROL Orders]**, wählen Sie die **[!UICONTROL Commerce Order Number]** , um [!DNL Commerce] Bestelldetails.

![Detailansicht einer Commerce-Bestellung für [!DNL Walmart Marketplace] order](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

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

- **Bestellte Artikel**—In diesem Abschnitt werden die Bestellinformationen aller Commerce-Bestellungen aufgelistet. Die [!UICONTROL Qty] gibt den Statusverlauf für Bestellelemente an. Wenn beispielsweise eine Bestellung fakturiert, versandt und rückerstattet wurde, können Sie die Statusübergänge sehen.

  ![Auftragsdetails zum Status des geordneten Elements [!DNL Walmart Marketplace] Bestellungen](assets/order-detail-status-history.png){width="600" zoomable="yes"}

Zeigen Sie Artikelrechnungen und Erstattungsdetails an, indem Sie [!UICONTROL Invoice] und [!UICONTROL Credit Memo] Optionen aus dem Navigationsmenü. Sie können auch direkt über das [[!UICONTROL Returns]](return-refund-orders.md) Dashboard in Ihrem Verkaufskanalspeicher.
