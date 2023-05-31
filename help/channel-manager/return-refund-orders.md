---
title: Rückgabe und Rückerstattung von Bestellungen
description: Anleitung für die vollständige oder teilweise Erstattung von Rückerstattungsanträgen [!DNL Walmart Marketplace] von [!DNL Channel Manager] für Adobe Commerce und Magento Open Source.
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '1184'
ht-degree: 0%

---

# Rückgabe und Rückerstattung von Bestellungen

Wenn ein Käufer eine Rückgabe für über erworbene Bestellungen anfordert [!DNL Walmart Marketplace], erstellt Walmart eine Rückkehranfrage. [!DNL Channel Manager] überwacht den Marketplace-Kanal für diese Anforderungen und synchronisiert die Informationen zur Rückgabeanforderung automatisch mit dem Kanal-Manager.

Auf der Seite &quot;Commerce&quot;löst die Rückgabeanforderung den folgenden Workflow aus:

1. Der Kanal-Manager erstellt eine entsprechende Rückgabeanforderung mit dem Empfangsstatus und fügt die Rückgabe-ID-Nummer ([!UICONTROL RMA #]) auf [!UICONTROL Returns] Dashboard. Im [!DNL Orders] Dashboard, die Statusdetails für die Bestellung, die mit der Rückgabe verknüpft ist, werden aktualisiert und enthalten eine [!UICONTROL Return requested] -Link, um die Rückgabe anzuzeigen und zu verarbeiten.

1. Die Händler verarbeiten die Rückerstattung im Zusammenhang mit der Rückgabe, indem sie ein Kreditmemo erstellen, das dem [Adobe Commerce-Erstattungs-Workflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html). Alle Erstattungen werden nach der Offline-Methode verarbeitet.

1. [!DNL Channel Manager] sendet eine Rückerstattungsaktualisierung an Walmart Marketplace, damit der Rückkehrstatus aktualisiert werden kann, um die von Adobe Commerce zurückgezahlte Erstattung widerzuspiegeln.

In der Storefront-Admin können Sie die Rückgaben vom Kanal-Manager anzeigen und verarbeiten, indem Sie den Verkaufskanalspeicher öffnen und auswählen **[!UICONTROL Returns]**.

![Kanal-Manager Gibt Dashboard zurück, um Rückerstattungen für Rückgabeanforderungen zu verarbeiten, die von empfangen wurden [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>Sie können nur Rückerstattungen für versandte Bestellungen verarbeiten. In [!DNL Channel Manager], muss der Bestellstatus [!UICONTROL Shipped]. In [!DNL Walmart Marketplace] Verkäuferkonto, muss die Bestellung [!UICONTROL Delivered].

## Gibt Steuerelemente und Spaltenbeschreibungen aus

Die folgenden Tabellen beschreiben die verfügbaren Steuerelemente und Spalten für [!DNL Channel Manager] gibt zurück.

**Steuerelemente für[!UICONTROL Returns]**

<table>
<tr>
<td><strong>Kontrolle</strong></td>
<td><strong>Beschreibung</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>Filtern Sie die Ansicht, indem Sie eine der [!UICONTROL Return Status] Karten.</td>
</tr>
<tr>
<td>Statusdetails</td>
<td>Für Rückgabeeinträge mit der [!UICONTROL Received] oder [!UICONTROL Refunded] Status können Sie das Kreditmemo für die Rückerstattung erstellen oder anzeigen, indem Sie den verknüpften Text in der Spalte Statusdetails auswählen.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Um Bestelldetails anzuzeigen, wählen Sie die [!DNL Commerce] Bestellnummer im [!UICONTROL Order] -Tabelle, um die Commerce-Bestellung zu öffnen.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Um die Kanalkonfiguration zu ändern, wählen Sie die Anmeldeinformationen der Walmart Connection, zugeordnete Attribute oder Versandkennungen aus. Wählen Sie in den Einstellungen die Option [!DNL Commerce] Bestellnummer im [!UICONTROL Order] Tabelle. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten.</td>
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
<td>Die Autorisierungsnummer der rückkehrenden Ware, die mit der von erhaltenen Rückgabeanforderung verknüpft ist [!DNL Walmart Marketplace]. Diese Zahl wird von Walmart Marketplace generiert. [!UICONTROL Returns] wenn der Rückgabeprozess initiiert wird.</td>
</tr>
<tr>
<td>[!DNL Commerce] Bestellnummer</td>
<td>Die [!DNL Commerce] Bestellnummer, die mit den Artikeln verknüpft ist, die in der Rückgabeanforderung von Walmart Marketplace enthalten sind. Zeigen Sie die Bestelldetails an, indem Sie die Bestellnummer auswählen.</td>
</tr>
<tr>
<td>Angefordert</td>
<td>Das Datum, an dem die Rückgabe am [!DNL Walmart Marketplace]
in lokale Zeit konvertiert wurde.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>Das Datum, ab dem die Rückgabe erstattet werden muss, um [!DNL Walmart Marketplace] [requirements](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f), konvertiert in lokale Zeit.</td>
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
<td>Gibt den aktuellen Rückkehrstatus im [!DNL Commerce] return workflow-<i>Erhalten</i>, <i>Erstattet</i>oder <i>Fehler</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Für entgegengenommene und rückerstattete Rücksendungen bieten die Statusdetails einen Link zum Zugriff auf das Kreditmemo zur Rückerstattungsverarbeitung. Wenn während der [!DNL Channel Manager] Synchronisierungsprozess zwischen Adobe Commerce und [!DNL Walmart marketplace]enthält dieses Feld die Fehlerbeschreibung.</td>
</tr>
</table>

## Rückkehrstatus

[!UICONTROL Return Status] liefert Informationen zum aktuellen Status von [!DNL Walmart Marketplace] von Adobe Commerce oder Magento Open Source verwaltete Rückgabeanforderungen zurückgeben.

Statusaktualisierungen werden zurückgegeben, wenn [!DNL Channel Manager] empfängt eine Rückgabeanfrage von der [!DNL Walmart Marketplace] oder wenn die [!DNL Commerce] Credit Memo wird erstellt, um die Rückerstattung für die zurückgegebenen Artikel zu verarbeiten.

Rückgaben können die folgenden Status aufweisen:

* **[!UICONTROL Received]**- Dies ist der Anfangsstatus der vom [!DNL Walmart Marketplace] speichern. Der Händler kann die Rückerstattung für die Rückgabe verarbeiten, indem er **[!UICONTROL Create credit memo]** im [!UICONTROL Status details].

* **[!UICONTROL Refunded]**—Gibt an, dass ein Kreditmemo erstellt wurde, um eine Rückerstattung für die zurückgegebenen Artikel zu verlangen. Händler können Erstattungsinformationen durch Auswahl von anzeigen **[!UICONTROL View credit memo]** im [!UICONTROL Status details].

* **[!UICONTROL Error]**—Gibt Anfragen zurück, die Fehler aufweisen. Fehler können auftreten, wenn die Rückgabeanforderung von Walmart fehlende oder falsche Daten enthält. Oder wenn [!DNL Channel Manager] kann die Update-Benachrichtigung nicht an Walmart senden.

## Rückkehrszenarien

In den folgenden Szenarien wird beschrieben, wie Erstattungen für verschiedene Arten von Rückkehranfragen von [!DNL Channel Manager].

* **Vollständige Rückgabe**—Wenn die Rückgabe-Anfrage von Walmart Marketplace für alle Artikel in der Bestellung gilt, aktualisieren Sie die Kreditkartenmenge, um alle Artikel zurückzuerstatten.

* **Teilweise Rückgabe**-Wenn die Rückgabe-Anfrage von Walmart Marketplace nur für einige Bestellartikel gilt, aktualisieren Sie die Kreditkartenmenge nur für die zurückzuerstattenden Artikel.

* **Rückgabe bereits über den Walmart Marketplace rückerstattet**-In einigen Fällen wird eine Erstattung verarbeitet am [!DNL Walmart Marketplace] bevor Sie die Rückgabe im Kanal-Manager verarbeiten. Wenn beispielsweise eine Commerce-Bestellung nicht innerhalb des von Walmart geforderten 48-Stunden-Rückerstattungsfensters zurückerstattet wird, erstattet Walmart die Bestellung automatisch. In diesem Fall synchronisiert der Kanal-Manager die Rückgabeanforderung weiterhin mit Adobe Commerce, damit Sie die Rückgabe verarbeiten und das Kreditmemo ausgeben können. Dieser Workflow stellt sicher, dass die Bestelldetails in [!DNL Commerce] entspricht den Bestellinformationen in Walmart Marketplace.

>[!NOTE]
>
> Es kann bis zu fünf Minuten dauern, bis die Aktualisierung der Rückerstattung mit synchronisiert wird. [!DNL Walmart Marketplace]. Sie können den aktuellen Rückkehrstatus im [!DNL Channel Manager] [!UICONTROL Returns] Dashboard.

## Erstattungsantrag verarbeiten

1. Öffnen Sie die [!UICONTROL Returns] Dashboard für Ihren Verkaufskanalspeicher.

   * Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

   * Sie können die Ergebnisse überprüfen, indem Sie die **[!UICONTROL Returns]** Registerkarte.

      Sie können auch über die [!UICONTROL Orders] Seite. Suchen nach [!UICONTROL Shipped] Bestellungen mit einer Rückgabeanforderung. Wählen Sie anschließend die `Return requested` im [!UICONTROL Status Details] -Spalte, um die Anfrage anzuzeigen und zu verarbeiten.

1. Suchen Sie in der Tabelle &quot;Rückgaben&quot;nach einer Rückgabe mit der Variablen *[!UICONTROL Received]* Status.

1. Überprüfen Sie in der Artikelspalte die Liste der Bestellartikel und der Menge, die rückerstattet werden sollen.

1. Verarbeiten Sie die Erstattung durch Ausstellung eines Kreditmemo.

   * Aus dem [!UICONTROL Status Details] Spalte auswählen **[!UICONTROL Create credit memo]** , um die Detailseite &quot;Bestellung&quot;in [!DNL Commerce].

      Wenn die Bestellung nicht in Rechnung gestellt wurde, wird auf der Seite Bestelldetails eine Fehlermeldung angezeigt, in der Sie aufgefordert werden, eine zu erstellen. Auswählen **[!UICONTROL Create invoice]**. Dann [Rechnung erstellen und speichern](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html).

   * Wählen Sie auf der Detailseite Sortierung die Option **[!UICONTROL Credit Memo]**.

   * In [!UICONTROL Items to Refund] Abschnitt [!UICONTROL Credit Memo], aktualisieren Sie die **[!UICONTROL Qty to refund]** und **[!UICONTROL Return to Stock]** Informationen für die Elemente, die in der Rückgabeanforderung enthalten sind.

      Stellen Sie sicher, dass nur die in der Rückgabeanforderung aufgelisteten Elemente zurückgegeben werden.

   * Um einen Kommentar hinzuzufügen, geben Sie den Text im **[!UICONTROL Credit Memo Comments]**

   * Auswählen **[!UICONTROL Refund Offline]**.

Nach Abschluss der Erstattung [!DNL Channel Manager] Aktualisiert den Rückkehrstatus im [!UICONTROL Returns] Dashboard zu [!UICONTROL Refunded] und synchronisiert die Aktualisierung mit Walmart, um den Rückgabestatus im Marketplace zu aktualisieren.


## Anzeigen von Rückerstattungsinformationen für die Rückgabe

Sie können Informationen zu Rückkehranfragen und Erstattungsverarbeitung über die [!UICONTROL Returns] Dashboard.

1. Öffnen Sie das Rückgabe-Dashboard für Ihren Verkaufskanalspeicher.

   * Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

   * Auswählen **[!UICONTROL Returns]**.

1. Zeigen Sie erstattete Bestellungen an, indem Sie **[!UICONTROL Refunded]** Statuskarte.

1. Anzeigen von Rückerstattungsdetails für eine Rückkehr durch Auswahl von **[!UICONTROL View credit memo]**.

   ![Kreditvermerk zur Rückerstattung zurückgegebener Artikel für einen [!DNL Walmart Marketplace] order](assets/refund-credit-memo-for-marketplace-order.png){width="600" zoomable="yes"}

>[!NOTE]
>
>Nach Rückerstattung einer Bestellung wird die [!UICONTROL Orders] im Dashboard werden keine Rückkehrinformationen angezeigt. Um Rückkehrinformationen anzuzeigen, verwenden Sie die [!DNL Channel Manager] Gibt Dashboard zurück. Ausführlichere Informationen zu Rückgabe und Rückerstattung finden Sie auch auf der Seite Bestelldetails .

## Fehlerbehebung bei Rückgabefehlern

Fehler können auftreten, wenn die Rückkehrinformationen von empfangen werden [!DNL Walmart Marketplace]oder wenn [!DNL Channel Manager] Synchronisiert Statusaktualisierungen von [!DNL Commerce] nach [!DNL Walmart Marketplace].

Wenn der Synchronisierungsvorgang für eine Rückgabe-Aktualisierung fehlschlägt, wird die [!DNL Channel Manager] Das Rückgabe-Dashboard zeigt eine *[!UICONTROL Error]* -Status für den Rückkehreintrag. Um sicherzustellen, dass die Rückgabe- und Rückerstattungsinformationen im Walmart Marketplace-Konto korrekt widergespiegelt werden, müssen Sie die Bestellung manuell in Ihrem [!DNL Walmart Marketplace] speichern.
