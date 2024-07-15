---
title: Rückgabe und Rückerstattung von Bestellungen
description: Anweisungen für die Ausgabe vollständiger oder teilweiser Erstattungen für Rückgabeanfragen, die von [!DNL Walmart Marketplace] von [!DNL Channel Manager] für Adobe Commerce und Magento Open Source empfangen wurden.
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# Rückgabe und Rückerstattung von Bestellungen

Wenn ein Käufer eine Rückgabe für über [!DNL Walmart Marketplace] erworbene Bestellartikel anfordert, erstellt Walmart eine Rückgabeanforderung. [!DNL Channel Manager] überwacht den Marketplace-Kanal für diese Anfragen und synchronisiert die Informationen zur Rückgabeanforderung automatisch mit dem Kanal-Manager.

Auf Commerce-Seite initiiert die Rückgabeanforderung den folgenden Workflow:

1. Der Kanal-Manager erstellt eine entsprechende Rückgabeanforderung mit dem Empfangsstatus und fügt die Rückgabe-ID-Nummer ([!UICONTROL RMA #]) zum Dashboard [!UICONTROL Returns] hinzu. Im Dashboard [!DNL Orders] werden die Statusdetails für die mit der Rückgabe verknüpfte Bestellung aktualisiert und enthalten einen [!UICONTROL Return requested] -Link, um die Rückgabe anzuzeigen und zu verarbeiten.

1. Händler verarbeiten die Rückerstattung im Zusammenhang mit der Rückgabe, indem sie ein Credit Memo erstellen, das dem Workflow [Adobe Commerce-Rückerstattung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html) folgt. Alle Erstattungen werden nach der Offline-Methode verarbeitet.

1. [!DNL Channel Manager] sendet ein Update der Rückerstattung an den Walmart Marketplace, damit der Rückkehrstatus aktualisiert werden kann, um die von Adobe Commerce zurückgegebene Rückerstattung widerzuspiegeln.

In der Storefront-Admin können Sie die Rückgaben vom Kanal-Manager anzeigen und verarbeiten, indem Sie den Verkaufskanalspeicher öffnen und **[!UICONTROL Returns]** auswählen.

![Kanal-Manager Gibt das Dashboard zurück, um Erstattungen für von [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png){width="600" zoomable="yes"} empfangene Rückgabeanforderungen zu verarbeiten

>[!NOTE]
>
>Sie können nur Rückerstattungen für versandte Bestellungen verarbeiten. In [!DNL Channel Manager] muss der Bestellstatus [!UICONTROL Shipped] sein. In [!DNL Walmart Marketplace] Verkäuferkonto muss die Bestellung [!UICONTROL Delivered] sein.

## Gibt Steuerelemente und Spaltenbeschreibungen aus

In den folgenden Tabellen werden die für [!DNL Channel Manager] verfügbaren Steuerelemente und Spalten beschrieben.

**Steuerelemente für[!UICONTROL Returns]**

<table>
<tr>
<td><strong>Kontrolle</strong></td>
<td><strong>Beschreibung</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>Filtern Sie die Ansicht, indem Sie eine der [!UICONTROL Return Status] Karten auswählen.</td>
</tr>
<tr>
<td>Statusdetails</td>
<td>Für Rücksendungen mit dem Status [!UICONTROL Received] oder [!UICONTROL Refunded] können Sie das Kreditmemo für die Rückerstattung erstellen oder anzeigen, indem Sie den verknüpften Text in der Spalte Statusdetails auswählen.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Um Bestelldetails anzuzeigen, wählen Sie die [!DNL Commerce] Bestellnummer in der Tabelle [!UICONTROL Order] aus, um die Commerce-Bestellung zu öffnen.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Um die Kanalkonfiguration zu ändern, wählen Sie die Anmeldeinformationen für die Walmart-Verbindung, zugeordnete Attribute oder Versandkennungen aus. Wählen Sie in den Einstellungen die Nummer [!DNL Commerce] der Reihenfolge in der Tabelle [!UICONTROL Order] aus. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten.</td>
</tr>
</table>

**Spaltenbeschreibungen**

<table>
<tr>
<td><strong>Feld</strong></td>
<td><strong>Beschreibung</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>Die Rückgabe-Merchandise-Autorisierungsnummer, die mit der von [!DNL Walmart Marketplace] erhaltenen Rückgabeanforderung verknüpft ist. Diese Zahl wird von Walmart Marketplace [!UICONTROL Returns] generiert, wenn der Rückgabeprozess initiiert wird.</td>
</tr>
<tr>
<td>[!DNL Commerce] Bestellnummer</td>
<td>Die [!DNL Commerce] Bestellnummer, die den Artikeln zugeordnet ist, die in der Rückgabeanforderung von Walmart Marketplace enthalten sind. Zeigen Sie die Bestelldetails an, indem Sie die Bestellnummer auswählen.</td>
</tr>
<tr>
<td>Angefordert</td>
<td>Das Datum, an dem die Rückgabe am [!DNL Walmart Marketplace] angefordert wurde
in lokale Zeit konvertiert wurde.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>Das Datum, ab dem die Rückgabe zurückgezahlt werden muss, um die in Ortszeit umgerechnete [!DNL Walmart Marketplace] [Anforderungen](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f) zu erfüllen.</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>Listet die SKU und die Menge für jedes Element auf, das im Rückgabewert aufgelistet ist.</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>Der Gesamtwert, der für die zurückgegebenen Artikel zurückzuzahlen ist.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Gibt den aktuellen Rückgabestatus im [!DNL Commerce] Rückgabe-Workflow -<i>Erhalten</i>, <i>Erstattet</i> oder <i>Fehler</i> an.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Für entgegengenommene und rückerstattete Rücksendungen bieten die Statusdetails einen Link zum Zugriff auf das Kreditmemo zur Rückerstattungsverarbeitung. Tritt während des Synchronisierungsprozesses [!DNL Channel Manager] zwischen Adobe Commerce und [!DNL Walmart marketplace] ein Fehler auf, wird in diesem Feld die Fehlerbeschreibung angezeigt.</td>
</tr>
</table>

## Rückkehrstatus

[!UICONTROL Return Status] liefert Informationen zum aktuellen Status von [!DNL Walmart Marketplace] von Adobe Commerce oder Magento Open Source verwalteten Rückgabeanforderungen.

Aktualisierungen des Rückkehrstatus treten auf, wenn [!DNL Channel Manager] eine Rückgabeanforderung von der [!DNL Walmart Marketplace] erhält oder wenn das [!DNL Commerce] Kreditmemo erstellt wird, um die Rückerstattung für die zurückgegebenen Elemente zu verarbeiten.

Rückgaben können die folgenden Status aufweisen:

* **[!UICONTROL Received]**-Dies ist der Anfangsstatus der vom [!DNL Walmart Marketplace] -Store empfangenen Rückgabeanforderung. Der Händler kann die Rückerstattung für die Rückgabe verarbeiten, indem er in der [!UICONTROL Status details] die Option **[!UICONTROL Create credit memo]** auswählt.

* **[!UICONTROL Refunded]** - Gibt an, dass ein Kreditmemo erstellt wurde, um eine Rückerstattung für die zurückgegebenen Elemente auszugeben. Händler können Rückerstattungsinformationen anzeigen, indem sie im Feld [!UICONTROL Status details] die Option **[!UICONTROL View credit memo]** auswählen.

* **[!UICONTROL Error]**—Gibt Anfragen zurück, die Fehler aufweisen. Fehler können auftreten, wenn die Rückgabeanforderung von Walmart fehlende oder falsche Daten enthält. Oder wenn [!DNL Channel Manager] die Aktualisierungsmeldung nicht an Walmart senden kann.

## Rückkehrszenarien

In den folgenden Szenarien wird beschrieben, wie Sie Erstattungen für verschiedene Arten von Rückkehranfragen von [!DNL Channel Manager] vornehmen.

* **Vollständige Rückgabe**: Wenn die Rückgabe-Anfrage von Walmart Marketplace für alle Artikel in der Bestellung gilt, aktualisieren Sie die Menge des Guthabens, um alle Artikel zurückzuerstatten.

* **Teilweise Rückgabe** - Wenn die Rückgabeanforderung von Walmart Marketplace nur für einige Bestellartikel gilt, aktualisieren Sie die Kreditkartenmenge nur für die zurückzuerstattenden Artikel.

* **Rückgabe bereits über den Walmart Marketplace zurückerstattet**-In einigen Fällen wird eine Rückerstattung am [!DNL Walmart Marketplace] verarbeitet, bevor Sie die Rückgabe im Kanal-Manager verarbeiten. Wenn beispielsweise eine Commerce-Bestellung nicht innerhalb des von Walmart geforderten 48-Stunden-Rückerstattungsfensters zurückerstattet wird, erstattet Walmart die Bestellung automatisch. In diesem Fall synchronisiert der Kanal-Manager die Rückgabeanforderung weiterhin mit Adobe Commerce, damit Sie die Rückgabe verarbeiten und das Kreditmemo ausgeben können. Dieser Workflow stellt sicher, dass die Bestelldetails in [!DNL Commerce] mit den Bestellinformationen im Walmart Marketplace übereinstimmen.

>[!NOTE]
>
> Es kann bis zu fünf Minuten dauern, bis Aktualisierungen zur Rückerstattung mit [!DNL Walmart Marketplace] synchronisiert werden. Sie können den aktuellen Rückkehrstatus im Dashboard [!DNL Channel Manager] [!UICONTROL Returns] überprüfen.

## Erstattungsantrag verarbeiten

1. Öffnen Sie das Dashboard [!UICONTROL Returns] für Ihren Vertriebskanalspeicher.

   * Wählen Sie im Admin **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** aus.

   * Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

   * Sie können die Rückgaben überprüfen, indem Sie die Registerkarte **[!UICONTROL Returns]** auswählen.

     Sie können auch über die Seite [!UICONTROL Orders] auf Rückkehrinformationen zugreifen. Suchen Sie nach [!UICONTROL Shipped] Bestellungen mit einer Rückgabeanforderung. Wählen Sie dann den Link `Return requested` in der Spalte [!UICONTROL Status Details] aus, um die Anfrage anzuzeigen und zu verarbeiten.

1. Suchen Sie in der Tabelle &quot;Rückgaben&quot;eine Rückgabe mit dem Status &quot;*[!UICONTROL Received]*&quot;.

1. Überprüfen Sie in der Artikelspalte die Liste der Bestellartikel und der Menge, die rückerstattet werden sollen.

1. Verarbeiten Sie die Erstattung durch Ausstellung eines Kreditmemo.

   * Wählen Sie in der Spalte [!UICONTROL Status Details] die Option **[!UICONTROL Create credit memo]** aus, um die Detailseite &quot;Reihenfolge&quot;in [!DNL Commerce] zu öffnen.

     Wenn die Bestellung nicht in Rechnung gestellt wurde, wird auf der Seite Bestelldetails eine Fehlermeldung angezeigt, in der Sie aufgefordert werden, eine zu erstellen. Wählen Sie **[!UICONTROL Create invoice]** aus. Erstellen und speichern Sie dann die Rechnung ](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html).[

   * Wählen Sie auf der Detailseite Reihenfolge die Option **[!UICONTROL Credit Memo]** aus.

   * Aktualisieren Sie im Abschnitt [!UICONTROL Items to Refund] des Abschnitts [!UICONTROL Credit Memo] die Informationen **[!UICONTROL Qty to refund]** und **[!UICONTROL Return to Stock]** für die Elemente, die in der Rückgabeanforderung enthalten sind.

     Stellen Sie sicher, dass nur die in der Rückgabeanforderung aufgelisteten Elemente zurückgegeben werden.

   * Um einen Kommentar hinzuzufügen, geben Sie den Text in das Feld **[!UICONTROL Credit Memo Comments]** ein

   * Wählen Sie **[!UICONTROL Refund Offline]** aus.

Nach Abschluss der Rückerstattung aktualisiert [!DNL Channel Manager] den Rückgabestatus im Dashboard [!UICONTROL Returns] auf [!UICONTROL Refunded] und synchronisiert die Aktualisierung mit Walmart, um den Rückgabestatus im Marketplace zu aktualisieren.


## Anzeigen von Rückerstattungsinformationen für die Rückgabe

Sie können Informationen zu Rückkehranfragen und Erstattungsverarbeitung über das Dashboard [!UICONTROL Returns] anzeigen.

1. Öffnen Sie das Rückgabe-Dashboard für Ihren Verkaufskanalspeicher.

   * Wählen Sie im Admin **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** aus.

   * Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

   * Wählen Sie **[!UICONTROL Returns]** aus.

1. Zeigen Sie erstattete Bestellungen an, indem Sie die Statuskarte **[!UICONTROL Refunded]** auswählen.

1. Zeigen Sie Details zur Rückgabe an, indem Sie **[!UICONTROL View credit memo]** auswählen.

   ![Kreditvermerk zur Rückerstattung zurückgegebener Artikel für eine [!DNL Walmart Marketplace] Bestellung](assets/refund-credit-memo-for-marketplace-order.png){width="600" zoomable="yes"}

>[!NOTE]
>
>Nach Rückerstattung einer Bestellung zeigt das Dashboard [!UICONTROL Orders] keine Rückgabeinformationen an. Um Rückkehrinformationen anzuzeigen, verwenden Sie das Dashboard [!DNL Channel Manager] Rückgabe . Ausführlichere Informationen zu Rückgabe und Rückerstattung finden Sie auch auf der Seite Bestelldetails .

## Fehlerbehebung bei Rückgabefehlern

Fehler können auftreten, wenn die Rückgabeinformationen von [!DNL Walmart Marketplace] empfangen werden oder [!DNL Channel Manager] Statusaktualisierungen von [!DNL Commerce] zu [!DNL Walmart Marketplace] synchronisiert.

Wenn der Synchronisierungsvorgang für eine Rückgabe-Aktualisierung fehlschlägt, zeigt das Dashboard [!DNL Channel Manager] den Status *[!UICONTROL Error]* für den Rückgabeeintrag an. Um sicherzustellen, dass die Rückgabe- und Rückerstattungsinformationen im Walmart Marketplace-Konto korrekt widergespiegelt werden, müssen Sie die Bestellung in Ihrem [!DNL Walmart Marketplace] -Store manuell aktualisieren.
