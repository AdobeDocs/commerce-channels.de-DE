---
title: Amazon-Bestelleinstellungen
description: Verwenden Sie die Bestelleinstellungen, um zu bestimmen, wie Amazon-Bestellungen in Ihren Commerce-Store importiert und dort verarbeitet werden.
feature: Sales Channels, Orders, Inventory, Configuration
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: a93ba31a95f32cc6ea285aed2399255021985693
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 0%

---

# Amazon-Bestelleinstellungen

Mit den Bestelleinstellungen wird definiert, ob und wie Amazon-Bestellungen in importiert und verarbeitet werden. [!DNL Commerce] und kann über die [Store-Dashboard](./amazon-store-dashboard.md).

Die Einstellungen für den Bestellimport sind auf `Enabled` Standardmäßig bedeutet dies, dass Ihre Amazon-Bestellungen im Store-Dashboard angezeigt werden und die entsprechenden [!DNL Commerce] Bestellungen. Importierte Bestellungen können im [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) Arbeitsablauf.

>[!NOTE]
>
>Unabhängig von Ihren Bestelleinstellungen werden Amazon-Bestellungen, die vor Ihrer Store-Integration existierten, nicht importiert.

Nachher [Store-Integration](./store-integration.md) abgeschlossen ist, können Sie Ihre Bestelleinstellungen ändern. Wenn Sie Ihre Bestelleinstellungen auf `Disabled`, werden Amazon-Bestellungen im Store-Dashboard angezeigt, müssen jedoch in Ihrem [!DNL Amazon Seller Central] -Konto.

Wenn eine Bestellung in Amazon erstellt wird, wird sie nicht sofort in importiert [!DNL Commerce]. Amazon weist eine `Pending` Status auf neu erstellte Bestellungen. Nachdem Amazon die Bestell- und Zahlungsmethode überprüft hat, wird der Auftragsstatus in `Unshipped`. Dieser Status ändert den Trigger des Bestellimports und [!DNL Commerce] erstellt eine passende, entsprechende Reihenfolge.

Aus Amazon importierte Bestellungen können im [!DNL Commerce] [Auftragsworkflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html). Siehe auch [Bestellungen verwalten](./managing-orders.md).

## Bestelleinstellungen konfigurieren {#configure-order-settings}

1. Klicks **[!UICONTROL Order Settings]** im Store-Dashboard.

1. Für **[!UICONTROL Import Amazon Orders]** (erforderlich), wählen Sie eine Option:

   - `Disabled` - Wählen Sie aus, wann Sie keine entsprechenden Bestellungen in der [!DNL Commerce] wenn neue Bestellungen von Amazon empfangen werden. Wenn diese Option aktiviert ist, sind alle anderen Felder auf dieser Seite deaktiviert.

   - `Enabled` - (Standard) Wählen Sie aus, wann Sie die entsprechenden [!DNL Commerce] Bestellungen, wenn neue Bestellungen von Amazon empfangen werden. [!DNL Commerce] Bestellungen werden basierend auf dem Amazon-Status und den Lagerbeständen erstellt.

     >[!NOTE]
     >
     >Importieren von Amazon-Bestellungen muss auf `Enabled` zur Verwaltung von Amazon-Bestellungen im [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) Arbeitsablauf. Wenn festgelegt auf `Disabled`, haben Ihre Amazon-Bestellungen keine entsprechende [!DNL Commerce] Bestellnummer und kann nicht in verwaltet werden [!DNL Commerce]. Sie verwalten diese Bestellungen in Ihren [!DNL Amazon Seller Central] -Konto.

1. Für **[!UICONTROL Import Amazon Orders Into Magento Store]** auswählen, welche [!DNL Commerce] Speichern Sie die Amazon-Bestellungen, die mit verknüpft sind, wenn die entsprechende Bestellung in [!DNL Commerce].

   Diese Einstellung ist standardmäßig die Store-Ansicht für die Website, die ausgewählt wird, wenn Sie [Amazon Store hinzugefügt](./store-integration.md). Wenn Sie diese Einstellung ändern möchten, hängt die Liste der Optionen von der [!DNL Commerce] speichert, die Sie in Ihrer Konfiguration eingerichtet haben. Siehe [Stores](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html).

1. Für **[!UICONTROL Customer Creation]** eine Option auswählen:

   - `No Customer Creation (guest)` - (Standard) Wählen Sie aus, wann Sie kein Kundenkonto in erstellen möchten. [!DNL Commerce] Verwendung der importierten Kundendaten aus der Amazon-Bestellung. Wenn ausgewählt, [!DNL Commerce] verarbeitet eine importierte Amazon-Bestellung auf die gleiche Weise wie ein Gastkasse in [!DNL Commerce].

   - `Build New Customer Account` - Wählen Sie aus, wann Sie ein neues Kundenkonto in erstellen möchten. [!DNL Commerce] unter Verwendung der Kundendaten, die mit der Amazon-Bestellung importiert wurden. Diese Option hilft beim Aufbau Ihrer Kundendatenbank anhand Ihrer Amazon-Bestellungen.

1. Für **[!UICONTROL Order Number Source]** eine Option auswählen:

   - `Build Using Magento Order Number` - (Standard) Wählen Sie aus, wann eine eindeutige [!DNL Commerce] Bestellnummer für die entsprechende Amazon-Bestellung unter Verwendung der [!DNL Commerce] inkrementell zugewiesene Bestell-ID.

   - `Build Using Amazon Order Number` - Wählen Sie aus, wann Sie die [!DNL Commerce] Bestellnummer unter Verwendung der entsprechenden von Amazon zugewiesenen Bestellnummer.

   >[!NOTE]
   >
   >Nachdem eine Bestellung importiert wurde, wird die Amazon-Bestellnummer im _[!UICONTROL Recent Orders]_im Dashboard speichern. Die [!DNL Commerce] Die Bestellnummer wird angezeigt, wenn Sie die Bestelldetails im [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) Arbeitsbereich.

1. Für **[!UICONTROL Order Status]** (erforderlich), wählen Sie eine Option:

   - `Default Order Status` - (Standard) Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, Ihr Standardbestellungsstatus für neue Bestellungen zugewiesen werden soll. Der Standardstatus für neue Bestellungen (sofern Sie keinen benutzerdefinierten Bestellstatus für neue Bestellungen erstellt haben) lautet `Pending`. Siehe [Verarbeitungsaufträge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

   - `Custom Order Status` - Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, ein anderer Status als der Standardstatus zugewiesen werden soll.

   - `Processing Order Status` - Aktiviert bei **[!UICONTROL Order Status]** auf `Custom Order Status`. Wählen Sie den Status aus, den Sie für neu erstellte, aus Amazon importierte Bestellungen verwenden möchten. Die Optionen in diesem Feld basieren auf den Standardstatusoptionen in [!DNL Commerce]. Siehe [Bestellstatus](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). Sie können auch einen benutzerdefinierten Bestellstatus erstellen, der hier zur Auswahl angezeigt wird. Informationen zum Erstellen eines benutzerdefinierten Bestellstatus finden Sie unter [Benutzerdefinierter Bestellstatus](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html#custom-order-status).

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save order settings]**.

![Bestelleinstellungen](assets/amazon-order-settings.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | Optionen:<ul><li>**[!UICONTROL Disabled]** - Wählen Sie aus, wann Sie keine entsprechenden Bestellungen in der [!DNL Commerce] wenn neue Bestellungen von Amazon empfangen werden. Wenn diese Option aktiviert ist, sind alle anderen Felder auf dieser Seite deaktiviert.</li><li>**[!UICONTROL Enabled]** - (Standard) Wählen Sie aus, wann Sie die entsprechenden [!DNL Commerce] Bestellungen, wenn neue Bestellungen von Amazon empfangen werden. [!DNL Commerce] Bestellungen werden basierend auf dem Amazon-Status und den Lagerbeständen erstellt.</li></ul><br><br>`Enabled` muss für die Verwaltung von Amazon-Bestellungen in [!DNL Commerce]. Wann `Disabled` ausgewählt ist, werden Ihre Amazon-Bestellungen im Dashboard des Stores angezeigt, die Bestellungen müssen jedoch in Ihrer [!DNL Amazon Seller Central] -Konto. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Auswählen [!DNL Commerce] Speichern Sie die Amazon-Bestellungen, mit denen sie verknüpft sind, wenn sie im [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) Arbeitsbereich. Diese Einstellung ist standardmäßig auf die Store-Ansicht für die [!DNL Commerce] während der [Amazon Store hinzugefügt](./store-integration.md). Wenn Sie diese Einstellung ändern möchten, hängt die Liste der Optionen von der [!DNL Commerce] speichert, die Sie in Ihrer Konfiguration eingerichtet haben. Siehe [Stores](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html). |
| [!UICONTROL Customer Creation] | Optionen:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Standard) Wählen Sie aus, wann Sie kein Kundenkonto in erstellen möchten. [!DNL Commerce] Verwendung der importierten Kundendaten aus der Amazon-Bestellung. Wenn diese Option ausgewählt ist, wird [!DNL Commerce] um eine importierte Amazon-Bestellung auf die gleiche Weise zu verarbeiten wie ein Gastkasse.</li><li>**[!UICONTROL Build New Customer Account]** - Wählen Sie aus, wann Sie ein neues Kundenkonto in Ihrer [!DNL Commerce] Kundendatenbank mit den Kundendaten, die mit der Amazon-Bestellung importiert wurden. Diese Option hilft bei der Erstellung Ihrer [!DNL Commerce] Kundendatenbank aus Ihren Amazon-Bestellungen.</li></ul> |
| Bestellnummer | Optionen:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Standard) Wählen Sie aus, wann eine eindeutige [!DNL Commerce] Bestellnummer für die entsprechende Amazon-Bestellung unter Verwendung der [!DNL Commerce] inkrementell zugewiesene Bestell-ID. </li><li>**Erstellen mithilfe der Amazon-Bestellnummer** - Wählen Sie aus, wann Sie die [!DNL Commerce] Bestellnummer unter Verwendung der entsprechenden von Amazon zugewiesenen Bestellnummer.</li></ul> |
| Ausstehende Bestellungen | Optionen:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Wählen Sie aus, wann Sie Ihre [!DNL Commerce] von Ihren Amazon-Bestellungen betroffene Lagermenge. Wählen Sie aus, ob Sie Amazon für Ihren FBA-Prozess (FBA) verwenden. Wenn Sie eine Amazon-Bestellung erhalten, wirkt sich die bestellte Menge nicht auf Ihre [!DNL Commerce] Lagermenge.</li><li>**[!UICONTROL Reserve Quantity]** - Wählen Sie aus, wann die Auftragsmenge in der Amazon &quot;reserviert&quot;werden soll. [!DNL Commerce] Lagermenge. Wenn Sie eine Amazon-Bestellung erhalten, wird die bestellte Menge in Ihrer [!DNL Commerce] Lagermenge, um Ihre [!DNL Commerce] Lager aus &quot;Überverkauf&quot;. Die &quot;reservierte&quot;Menge kann nicht über Ihre [!DNL Commerce] Storefront.</li></ul> |
| [!UICONTROL Order Status] | Optionen:<ul><li>**[!UICONTROL Default Order Status]** - (Standard) Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, Ihr Standardbestellungsstatus für neue Bestellungen zugewiesen werden soll. Der Standardstatus für neue Bestellungen (sofern Sie keinen benutzerdefinierten Bestellstatus für neue Bestellungen erstellt haben) lautet `Pending`. Siehe [Verarbeitungsaufträge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).</li><li>**[!UICONTROL Custom Order Status]** - Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, ein anderer Status als der Standardstatus zugewiesen werden soll. Wenn ausgewählt, **[!UICONTROL Processing Order Status]** ermöglicht Ihnen die Auswahl des Status, den Sie für neu erstellte, aus Amazon importierte Bestellungen verwenden möchten.</li></ul> |
| [!UICONTROL Processing Orders Status] | Aktiviert bei _[!UICONTROL Order Status]_auf `Custom Order Status`. Wählen Sie den Bestellstatus aus, den Sie neuen Bestellungen zuweisen möchten. Die Optionen in diesem Feld hängen von den Standardstatusoptionen in [!DNL Commerce]. Siehe [Bestellstatus](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). Sie können auch einen benutzerdefinierten Bestellstatus erstellen, der hier angezeigt wird. Informationen zum Erstellen eines benutzerdefinierten Bestellstatus finden Sie unter [Benutzerdefinierter Bestellstatus] |

## [!DNL Commerce] Auftragserstellung

[!DNL Commerce] Bestellungen werden für Amazon-Bestellungen basierend auf den folgenden Status- und Lagerbedingungen erstellt.

### Auftragserstellung mit Inventory management

>[!NOTE]
>
>Wird nur in Adobe Commerce- und Magento Open Source 2.3.x-Integrationen unterstützt.

| Ausführungskanal | [!DNL Commerce] Inventarstatus | Amazon-Bestellstatus | [!UICONTROL Create Magento Order] Einstellung | Bestand reserviert |
|---------------------|-------------------------------------------|---------------------|-------------------------------------------|--------------------|
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Ausstehend | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | PendingAvailability | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Abgebrochen | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Fehler | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Unversandt | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Teilweise ausgeliefert | Nein | Nein |
| FBA | Vorrätig<br>Nicht verwalten | versandt | Ja | Nein |
| FBA | Nicht vorrätig | versandt | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Ausstehend | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | PendingAvailability | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Abgebrochen | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Fehler | Nein | Nein |
| FBM | Vorrätig<br>Nicht verwalten | Unversandt | Ja | Ja |
| FBM | Nicht vorrätig | Unversandt | Nein | Nein |
| FBM | Vorrätig<br>Nicht verwalten | Teilweise ausgeliefert | Ja | Ja |
| FBM | Nicht vorrätig | Teilweise ausgeliefert | Nein | Nein |
| FBM | Vorrätig<br>Nicht verwalten | versandt | Ja | Ja |
| FBM | Nicht vorrätig | versandt | Nein | Nein |

>[!NOTE]
>Wenn eine Amazon-Bestellung in eine `Partially Shipped` oder `Shipped` -Status, wird die Lagerbestandsreservierung für alle Elemente in der Bestellung erstellt. Der Amazon-Vertriebskanal kompensiert keine zuvor versandten Artikel.
>
>Wenn eine Bestellung von Amazon (FBA) ausgeführt wird, sich jedoch ein Artikel in `out of stock` Status, [!DNL Commerce] kann keine entsprechende Bestellung erstellen. Dies ist eine Einschränkung bei Inventory management-Integrationen.
