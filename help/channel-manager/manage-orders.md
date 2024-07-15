---
title: "Anzeigen und Verwalten von Bestellungen von  [!DNL Channel Manager]"
description: '"Anzeigen und Verwalten von [!DNL Walmart Marketplace] Bestellungen mit [!DNL Channel Manager] für Adobe Commerce und Magento Open Source".'
feature: Sales Channels, Orders
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

# Anzeigen und Verfolgen von Bestellungen über [!DNL Channel Manager]

[!DNL Walmart Marketplace] Bestelldaten für [!DNL Commerce] Produkte werden automatisch auf [!DNL Channel Manager] synchronisiert, nachdem [!DNL Walmart] die Bestellung verarbeitet hat.

Auf der Seite [!DNL Commerce] werden bei erfolgreicher Synchronisation die folgenden Trigger ausgeführt:

- [!DNL Channel Manager] sendet eine Auftragsbestätigung an Walmart.

- Eine entsprechende [!DNL Commerce] -Reihenfolge wird aus der Walmart-Reihenfolge erstellt.

- Die aktualisierten Bestellinformationen werden im Dashboard [!DNL Channel Manager] Bestellungen angezeigt.

In der Storefront-Admin können Sie Bestelldaten aus [!DNL Channel Manager] anzeigen, indem Sie den Verkaufskanalspeicher öffnen und **[!UICONTROL Orders]** auswählen.

![Ansicht &quot;Channel Manager Bestellungen&quot;, um [!DNL Walmart Marketplace] Bestellungen zu verwalten](assets/orders-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>Es kann bis zu 35 Minuten dauern, bis eine [!DNL Walmart Marketplace]-Bestellung in der Liste der [!DNL Channel Manager] Bestellungen angezeigt wird. [!DNL Walmart] benötigt ca. 30 Minuten, um eingehende Bestellungen zu verarbeiten und an [!DNL Channel Manager] zu senden. Nachdem der Kanal-Manager die Bestellung erhalten hat, dauert es etwa fünf Minuten, bis die Bestellung in Adobe Commerce oder Magento Open Source erstellt und angezeigt wird.

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
<td>Sortieren Sie die Ansicht, indem Sie eine der [!UICONTROL Order Status] Karten auswählen.</td>
</tr>
<tr>
<td>Statusdetails</td>
<td>Enthält Informationen zu Bestellfehlern und Rückgabeanfragen. Um Rückgabe- und Rückerstattungsstatus für eine Bestellung anzuzeigen, wählen Sie den Text <strong>[!UICONTROL Return requested]</strong> aus, um das Dashboard [!UICONTROL Returns] zu öffnen.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Um Bestelldetails anzuzeigen, wählen Sie die [!DNL Commerce] Bestellnummer in der Tabelle [!UICONTROL Order] aus. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Um die Kanalkonfiguration zu ändern, wählen Sie die Anmeldeinformationen für die Walmart-Verbindung, zugeordnete Attribute oder Versandkennungen aus. Wählen Sie in den Einstellungen die Nummer [!DNL Commerce] der Reihenfolge in der Tabelle [!UICONTROL Order] aus. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten.</td>
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
<td>Die der Bestellung in der [!DNL Walmart Marketplace] zugewiesene Bestellnummer. Beim erstmaligen Import einer Bestellung in [!DNL Channel Manager] wird nur die Bestellnummer [!DNL Walmart] angezeigt. Wenn die [!DNL Commerce] -Bestellung erstellt wird, wird die [!DNL Walmart] -Bestellnummer im Produktattribut [!UICONTROL External ID] gespeichert.</td>
</tr>
<tr>
<td>[!DNL Commerce] Bestellnummer</td>
<td>Die Zahl, die der mit der [!DNL Walmart Marketplace] -Reihenfolge erstellten [!DNL Commerce]-Reihenfolge zugewiesen wurde.</td>
</tr>
<tr>
<td>Elemente</td>
<td>Anzahl der bestellten Artikel bei [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>Gesamtkosten der bestellten Artikel.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>Das Datum, an dem die Bestellung an die [!DNL Walmart Marketplace] gesendet wurde, die in die lokale Zeitzone konvertiert wurde.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>Das Datum, an dem die Bestellung versandt werden muss, um die in die lokale Zeitzone konvertierten [!DNL Walmart Marketplace] Anforderungen zu erfüllen.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>Das Datum, an dem die Bestellung an den Kunden geliefert werden muss, um die in die lokale Zeitzone konvertierten [!DNL Walmart Marketplace] Anforderungen zu erfüllen.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>Die für die Bestellung ausgewählte [[!DNL Walmart Marketplace] Versandmethode](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29 .</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>Zeitstempel, der angibt, wann die Bestelldaten zuletzt in [!DNL Channel Manager] in eine lokale Zeitzone konvertiert wurden.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Gibt den aktuellen Bestellstatus im Workflow [!DNL Commerce] Bestellung an. Der Anfangsstatus für eine von [!DNL Walmart Marketplace] importierte Bestellung ist _Open_. Zusätzliche Statusaktualisierungen treten auf, wenn [!DNL Commerce] Bestellungen verarbeitet werden und [!DNL Channel Manager] Sendungen, Teillieferungen und Stornierungsaktualisierungen erfolgreich mit dem [!DNL Walmart Marketplace] synchronisiert.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Enthält detailliertere Informationen zu Bestellungen mit Fehlern oder Erstattungsanfragen.</td>
</tr>
</table>

## Bestellstatus

[!UICONTROL Order Status] liefert Informationen zum aktuellen Status von [!DNL Walmart Marketplace] Bestellungen, die von Adobe Commerce oder Magento Open Source verwaltet werden. Aktualisierungen des Bestellstatus treten auf, wenn [!DNL Channel Manager] aktualisierte Bestellinformationen entweder vom [!DNL Walmart Marketplace]- oder vom [!DNL Commerce] Bestellsystem erhält. Bestellungen können den folgenden Status aufweisen:

- **[!UICONTROL Shipped]**—Bestellungen, die aus dem [!DNL Commerce]-Store versandt wurden. Wenn die Bestellung ausgeht, sendet [!DNL Channel Manager] eine Aktualisierung an [!DNL Walmart Marketplace], um den Versandstatus bei Walmart zu aktualisieren und die Bestellnummer für die Sendung anzugeben. Nach dem Versand einer Bestellung können Bestellungen teilweise oder vollständig zurückerstattet werden, wenn Walmart ein Formular für die Rückgabe-Merchandise-Autorisierung ausgibt. Siehe [Rückgaben und Rückerstattungen](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]**—Bestellungen, bei denen einige als versandt markierte Artikel und andere warten, versandt zu werden. Wenn Artikel im Bestellschiff, sendet [!DNL Channel Manager] eine Aktualisierung an [!DNL Walmart Marketplace], um den Versandstatus auf _[!DNL Partially Shipped]_bei Walmart zu aktualisieren und die Bestellverfolgungsnummer für die Sendung anzugeben.

- **[!UICONTROL Canceled]**—Bestellungen, die aus dem [!DNL Commerce]-Store storniert wurden.

  Nach Abschluss der Stornierung wird die Lagermenge von [!DNL Commerce] aktualisiert, um die zurückgegebenen Elemente widerzuspiegeln. Dann synchronisiert [!DNL Channel Manager] die Aktualisierung mit dem [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]**: Wenn der Walmart Marketplace eine Rückgabe für versandte Bestellelemente anfordert, wird in der Spalte [!UICONTROL Status details] ein `Return requested` -Link angezeigt. Wenn Sie den Link auswählen, wird das Dashboard [!UICONTROL Returns] geöffnet, um die Rückgabe anzuzeigen und den Rückerstattungsprozess zu verwalten.

- **[!UICONTROL Error]**—Bestellungen mit Fehlern. Fehler können auftreten, wenn ein Bestellaktualisierungsvorgang fehlschlägt. Beispielsweise treten Fehler auf, wenn [!DNL Channel Manager] keine neue Bestellung von Walmart erhalten kann. Sie können auch auftreten, wenn [!DNL Channel Manager] keine Auftragsversand- oder -stornierungsaktualisierung an die [!DNL Walmart Marketplace] senden kann. Wenn ein Vorgang fehlschlägt, zeigt die Seite &quot;Bestellungen&quot;den Status _Fehler_ für die Bestellung an. Weitere Informationen finden Sie unter [Bestellfehler beheben](process-orders.md#fix-shipping-and-cancel-errors).

- **[!UICONTROL Status details]**-Bietet weitere Informationen zu Bestellfehlern, die aufgrund von Problemen auftreten, wie fehlende Informationen oder ungültige Werte, falsche Versanddetails oder eine fehlgeschlagene Auftragsstornierung. Anhand der Beschreibung kann festgestellt werden, ob ein Fehler in der [!DNL Commerce] -Instanz oder in der [!DNL Walmart Marketplace] aufgetreten ist.

>[!NOTE]
>
>Wenn Bestellartikel in mehreren Sendungen gesendet werden, spiegelt der Bestellstatus in [!DNL Channel Manager] den letzten verfügbaren Bestellstatus wider. Wenn beispielsweise das erste Element ausgeliefert wird und keine Fehler zurückgegeben werden, wenn Bestellaktualisierungen mit [!DNL Channel Manager] und [!DNL Walmart Marketplace] synchronisiert werden, lautet der Auftragsstatus [!DNL Channel Manager] _[!UICONTROL Partially Shipped]_. Wenn ein zweites Element ausgeliefert wird und [!DNL Channel Manager] einen Fehler zurückgibt, wird der Auftragsstatus auf_[!UICONTROL Error]_ aktualisiert.

## Bestellungen überprüfen

1. Wählen Sie im Admin **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** aus, um die Seite [!UICONTROL Channel Manager Marketplace Stores] zu öffnen.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol in einer Store-Einstiegszeile auswählen.

1. Um Bestellinformationen anzuzeigen, wählen Sie *[!UICONTROL *Orders]**.

1. Rufen Sie Informationen zur Reihenfolge ab und bestimmen Sie die nächsten Schritte, indem Sie die Spalte **[Status](#order-status)** überprüfen.

## Details zur Bestellung überprüfen

Nachdem eine Bestellung vom Marketplace empfangen und in Ihren Vertriebskanalspeicher importiert wurde, verwenden Sie die [!DNL Commerce] Bestell-ID , um die Bestelldetails in Adobe Commerce anzuzeigen.

Wählen Sie unter &quot;**[!UICONTROL Orders]**&quot;den Wert &quot;**[!UICONTROL Commerce Order Number]**&quot;aus, um die [!DNL Commerce] Bestelldetails zu öffnen.

![Commerce Bestelldetailansicht für eine [!DNL Walmart Marketplace] Bestellung](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

Im Commerce-Storefront enthalten die Bestelldaten die folgenden zusätzlichen Informationen zu aus [!DNL Walmart Marketplace] importierten Bestellungen:

- **Zahlungsinformationen und Versandmethode**-Aus Walmart importierte Bestellungen enthalten folgende Werte für Zahlungs- und Versandfelder:

   - **[!UICONTROL Offline Channel Payment]**—Gibt an, dass die Bestellungszahlung offline von [!DNL Walmart Marketplace] verarbeitet wird.

   - **[!UICONTROL External Order Number]** - Zeigt die [!DNL Walmart Marketplace] Bestellnummer an.

   - **[!UICONTROL Channel Shipping - Value]**-Gibt an, dass Versandgebühren über [!DNL Walmart Marketplace] verarbeitet werden.

   - **[!UICONTROL Cancellation Reason]** - Dieses Feld wird nur angezeigt, wenn eine aus [!DNL Walmart Marketplace] importierte Bestellung abgebrochen wurde. Zu den Abbruchsgründen gehören:

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **Bestellte Artikel** - In diesem Abschnitt werden die Bestellelemente für alle Commerce-Bestellungen aufgelistet. Die Spalte [!UICONTROL Qty] enthält den Statusverlauf für Bestellelemente. Wenn beispielsweise eine Bestellung fakturiert, versandt und rückerstattet wurde, können Sie die Statusübergänge sehen.

  ![Bestelldetails Bestellstatus-Verlauf [!DNL Walmart Marketplace] Bestellungen](assets/order-detail-status-history.png){width="600" zoomable="yes"}

Zeigen Sie Details zur Artikelrechnung und -rückerstattung an, indem Sie die Optionen [!UICONTROL Invoice] und [!UICONTROL Credit Memo] im Navigationsmenü auswählen. Sie können auch direkt über das Dashboard [[!UICONTROL Returns]](return-refund-orders.md) in Ihrem Vertriebskanalspeicher auf das Credit Memo zugreifen.
