---
title: Amazon-Bestelleinstellungen
description: Verwenden Sie die Bestelleinstellungen, um zu bestimmen, wie Amazon-Bestellungen in Ihren Commerce-Store importiert und dort verarbeitet werden.
feature: Sales Channels, Orders, Inventory, Configuration
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: a93ba31a95f32cc6ea285aed2399255021985693
workflow-type: tm+mt
source-wordcount: '1388'
ht-degree: 0%

---

# Amazon-Bestelleinstellungen

Mit den Bestelleinstellungen wird definiert, ob und wie Amazon-Bestellungen in [!DNL Commerce] importiert und verarbeitet werden. Sie können auf das Dashboard [store](./amazon-store-dashboard.md) zugreifen.

Die Einstellungen für den Bestellimport sind standardmäßig auf &quot;`Enabled`&quot; eingestellt, was bedeutet, dass Ihre Amazon-Bestellungen im Store-Dashboard angezeigt werden und die entsprechenden [!DNL Commerce] Bestellungen erstellen. Importierte Bestellungen können im Workflow [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) verwaltet werden.

>[!NOTE]
>
>Unabhängig von Ihren Bestelleinstellungen werden Amazon-Bestellungen, die vor Ihrer Store-Integration existierten, nicht importiert.

Nachdem die [Speicherintegration](./store-integration.md) abgeschlossen ist, können Sie Ihre Bestelleinstellungen ändern. Wenn Sie Ihre Bestelleinstellungen auf &quot;`Disabled`&quot; setzen, werden Amazon-Bestellungen im Store-Dashboard angezeigt, müssen aber in Ihrem [!DNL Amazon Seller Central] -Konto verwaltet werden.

Wenn eine Bestellung in Amazon erstellt wird, wird sie nicht sofort in [!DNL Commerce] importiert. Amazon weist neu erstellten Bestellungen den Status &quot;`Pending`&quot;zu. Nachdem Amazon die Bestell- und Zahlungsmethode überprüft hat, wird der Auftragsstatus in `Unshipped` geändert. Diese Statusänderung Trigger den Bestellimport und [!DNL Commerce] erstellt eine übereinstimmende, entsprechende Reihenfolge.

Aus Amazon importierte Bestellungen können im Workflow [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) verwaltet werden. Siehe auch [Bestellungen verwalten](./managing-orders.md).

## Bestelleinstellungen konfigurieren {#configure-order-settings}

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Order Settings]** .

1. Wählen Sie für &quot;**[!UICONTROL Import Amazon Orders]**&quot;(erforderlich) eine Option:

   - `Disabled` - Wählen Sie aus, wann Sie keine entsprechenden Bestellungen in [!DNL Commerce] erstellen möchten, wenn neue Bestellungen von Amazon empfangen werden. Wenn diese Option aktiviert ist, sind alle anderen Felder auf dieser Seite deaktiviert.

   - `Enabled` - (Standard) Wählen Sie aus, wann Sie entsprechende [!DNL Commerce] Bestellungen erstellen möchten, wenn neue Bestellungen von Amazon empfangen werden. [!DNL Commerce] Bestellungen werden basierend auf dem Amazon-Status und den Lagerbeständen erstellt.

     >[!NOTE]
     >
     >Für den Import von Amazon-Bestellungen muss der Wert &quot;`Enabled`&quot;festgelegt sein, damit Amazon-Bestellungen im Workflow [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) verwaltet werden können. Wenn der Wert auf `Disabled` gesetzt ist, haben Ihre Amazon-Bestellungen keine entsprechende [!DNL Commerce] Bestellnummer und können nicht in [!DNL Commerce] verwaltet werden. Sie verwalten diese Bestellungen in Ihrem [!DNL Amazon Seller Central] -Konto.

1. Wählen Sie für **[!UICONTROL Import Amazon Orders Into Magento Store]** aus, mit welchem [!DNL Commerce] Speicher die Amazon-Bestellungen verknüpft sind, wenn die entsprechende Bestellung in [!DNL Commerce] erstellt wird.

   Diese Einstellung ist standardmäßig auf die Store-Ansicht der Website festgelegt, die ausgewählt wurde, als Sie den Amazon Store ](./store-integration.md) [hinzugefügt haben. Wenn Sie diese Einstellung ändern möchten, hängt die Liste der Optionen von den [!DNL Commerce] Stores ab, die Sie in Ihrer Konfiguration eingerichtet haben. Siehe [Stores](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html).

1. Wählen Sie für **[!UICONTROL Customer Creation]** eine Option:

   - `No Customer Creation (guest)` - (Standard) Wählen Sie aus, ob Sie kein Kundenkonto in [!DNL Commerce] erstellen möchten, das die importierten Kundendaten aus der Amazon-Bestellung verwendet. Wenn diese Option aktiviert ist, verarbeitet [!DNL Commerce] eine importierte Amazon-Bestellung auf die gleiche Weise wie ein Gastkasse in [!DNL Commerce].

   - `Build New Customer Account` - Wählen Sie aus, wann Sie ein neues Kundenkonto in [!DNL Commerce] mit den mit der Amazon-Bestellung importierten Kundendaten erstellen möchten. Diese Option hilft beim Aufbau Ihrer Kundendatenbank anhand Ihrer Amazon-Bestellungen.

1. Wählen Sie für **[!UICONTROL Order Number Source]** eine Option:

   - `Build Using Magento Order Number` - (Standard) Legen Sie fest, wann Sie eine eindeutige [!DNL Commerce] Bestellnummer für die entsprechende Amazon-Bestellung erstellen möchten, indem Sie die schrittweise zugewiesene Bestell-ID [!DNL Commerce] verwenden.

   - `Build Using Amazon Order Number` - Wählen Sie aus, wann Sie die [!DNL Commerce] Bestellnummer mit der entsprechenden von Amazon zugewiesenen Bestellnummer erstellen möchten.

   >[!NOTE]
   >
   >Nach dem Import einer Bestellung wird die Amazon-Bestellnummer in der Liste _[!UICONTROL Recent Orders]_im Store-Dashboard angezeigt. Die [!DNL Commerce] Bestellnummer wird angezeigt, wenn die Bestelldetails im Arbeitsbereich [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) angezeigt werden.

1. Wählen Sie für &quot;**[!UICONTROL Order Status]**&quot;(erforderlich) eine Option:

   - `Default Order Status` - (Standard) Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, Ihr definierter standardmäßiger Bestellstatus für neue Bestellungen zugewiesen werden soll. Der Standardstatus für neue Bestellungen (es sei denn, Sie haben einen benutzerdefinierten Bestellstatus für neue Bestellungen erstellt) ist `Pending`. Siehe [Bestellungen verarbeiten](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

   - `Custom Order Status` - Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, ein anderer Status als der Standardstatus zugewiesen werden soll.

   - `Processing Order Status` - Aktiviert, wenn **[!UICONTROL Order Status]** auf `Custom Order Status` gesetzt ist. Wählen Sie den Status aus, den Sie für neu erstellte, aus Amazon importierte Bestellungen verwenden möchten. Die Optionen in diesem Feld basieren auf den Standardstatusoptionen in [!DNL Commerce]. Siehe [Bestellstatus](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). Sie können auch einen benutzerdefinierten Bestellstatus erstellen, der hier zur Auswahl angezeigt wird. Informationen zum Erstellen eines benutzerdefinierten Bestellstatus finden Sie unter [Benutzerdefinierter Bestellstatus](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html#custom-order-status).

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save order settings]**.

![Bestelleinstellungen](assets/amazon-order-settings.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | Optionen:<ul><li>**[!UICONTROL Disabled]** - Wählen Sie aus, wann Sie keine entsprechenden Bestellungen in [!DNL Commerce] erstellen möchten, wenn neue Bestellungen von Amazon empfangen werden. Wenn diese Option aktiviert ist, sind alle anderen Felder auf dieser Seite deaktiviert.</li><li>**[!UICONTROL Enabled]** - (Standard) Wählen Sie aus, wann Sie entsprechende [!DNL Commerce] Bestellungen erstellen möchten, wenn neue Bestellungen von Amazon empfangen werden. [!DNL Commerce] Bestellungen werden basierend auf dem Amazon-Status und den Lagerbeständen erstellt.</li></ul><br><br>`Enabled` muss ausgewählt sein, um Amazon-Bestellungen in [!DNL Commerce] zu verwalten. Wenn `Disabled` ausgewählt ist, werden Ihre Amazon-Bestellungen im Store-Dashboard angezeigt, die Bestellungen müssen jedoch in Ihrem [!DNL Amazon Seller Central] -Konto verwaltet werden. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Wählen Sie aus, mit welchem [!DNL Commerce]-Speicher die Amazon-Bestellungen verknüpft sind, wenn sie im Arbeitsbereich [!DNL Commerce] [Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) erstellt werden. Diese Einstellung wird standardmäßig auf die Store-Ansicht für die [!DNL Commerce]-Website festgelegt, die ausgewählt wurde, als Sie [den Amazon Store hinzugefügt haben](./store-integration.md). Wenn Sie diese Einstellung ändern möchten, hängt die Liste der Optionen von den [!DNL Commerce] Stores ab, die Sie in Ihrer Konfiguration eingerichtet haben. Siehe [Stores](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html). |
| [!UICONTROL Customer Creation] | Optionen:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Standard) Wählen Sie aus, ob Sie kein Kundenkonto in [!DNL Commerce] erstellen möchten, das die importierten Kundendaten aus der Amazon-Bestellung verwendet. Wenn diese Option ausgewählt ist, wird [!DNL Commerce] angewiesen, eine importierte Amazon-Bestellung auf die gleiche Weise zu verarbeiten wie ein Gastkasse.</li><li>**[!UICONTROL Build New Customer Account]** - Wählen Sie aus, wann Sie ein neues Kundenkonto in Ihrer [!DNL Commerce] Kundendatenbank mit den mit der Amazon-Bestellung importierten Kundendaten erstellen möchten. Mit dieser Option können Sie Ihre [!DNL Commerce] -Kundendatenbank aus Ihren Amazon-Bestellungen erstellen.</li></ul> |
| Bestellnummer Source | Optionen:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Standard) Legen Sie fest, wann Sie eine eindeutige [!DNL Commerce] Bestellnummer für die entsprechende Amazon-Bestellung erstellen möchten, indem Sie die schrittweise zugewiesene Bestell-ID [!DNL Commerce] verwenden. </li><li>**Mit Amazon-Bestellnummer erstellen** - Wählen Sie aus, wann die [!DNL Commerce] Bestellnummer mit der entsprechenden von Amazon zugewiesenen Bestellnummer erstellt werden soll.</li></ul> |
| Ausstehende Bestellungen | Optionen:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Wählen Sie aus, wann Ihre [!DNL Commerce] Lagermenge nicht von Ihren Amazon-Bestellungen betroffen sein soll. Wählen Sie aus, ob Sie Amazon für Ihren FBA-Prozess (FBA) verwenden. Wenn Sie eine Amazon-Bestellung erhalten, wirkt sich die bestellte Menge nicht auf Ihre [!DNL Commerce] Lagermenge aus.</li><li>**[!UICONTROL Reserve Quantity]** - Wählen Sie aus, wann die Bestellmenge in der Amazon-Bestellung in Ihrer [!DNL Commerce] Lagermenge &quot;reserviert&quot;werden soll. Wenn Sie eine Amazon-Bestellung erhalten, wird die bestellte Menge in Ihrer [!DNL Commerce] Lagermenge &quot;reserviert&quot;, um zu verhindern, dass Ihr [!DNL Commerce]-Lager &quot;überverkauft&quot;wird. Die &quot;reservierte&quot;Menge kann nicht über Ihre [!DNL Commerce] Storefront gekauft werden.</li></ul> |
| [!UICONTROL Order Status] | Optionen:<ul><li>**[!UICONTROL Default Order Status]** - (Standard) Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, Ihr standardmäßiger Bestellstatus für neue Bestellungen zugewiesen werden soll. Der Standardstatus für neue Bestellungen (es sei denn, Sie haben einen benutzerdefinierten Bestellstatus für neue Bestellungen erstellt) ist `Pending`. Siehe [Bestellungen verarbeiten](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).</li><li>**[!UICONTROL Custom Order Status]** - Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, ein anderer Status als der Standardstatus zugewiesen werden soll. Wenn diese Option aktiviert ist, können Sie mit **[!UICONTROL Processing Order Status]** den Status auswählen, den Sie für neu erstellte, aus Amazon importierte Bestellungen verwenden möchten.</li></ul> |
| [!UICONTROL Processing Orders Status] | Aktiviert, wenn _[!UICONTROL Order Status]_auf `Custom Order Status` gesetzt ist. Wählen Sie den Bestellstatus aus, den Sie neuen Bestellungen zuweisen möchten. Die Optionen in diesem Feld hängen von den Standardstatusoptionen in [!DNL Commerce] ab. Siehe [Bestellstatus](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). Sie können auch einen benutzerdefinierten Bestellstatus erstellen, der hier angezeigt wird. Informationen zum Erstellen eines benutzerdefinierten Bestellstatus finden Sie unter [Benutzerdefinierter Bestellstatus] |

## [!DNL Commerce] Auftragserstellung

[!DNL Commerce] Bestellungen werden für Amazon-Bestellungen basierend auf den folgenden Status- und Lagerbestandsbedingungen erstellt.

### Auftragserstellung mit Inventory management

>[!NOTE]
>
>Wird nur in Adobe Commerce- und Magento Open Source 2.3.x-Integrationen unterstützt.

| Ausführungskanal | [!DNL Commerce] Lagerbestandsstatus | Amazon-Bestellstatus | [!UICONTROL Create Magento Order] Einstellung | Bestand reserviert |
|---------------------|-------------------------------------------|---------------------|-------------------------------------------|--------------------|
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Ausstehend | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | PendingAvailability | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Abgebrochen | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Fehler | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Unversandt | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Teilweise ausgeliefert | Nein | Nein |
| FBA | Auf Lager<br>nicht verwalten | versandt | Ja | Nein |
| FBA | Nicht vorrätig | versandt | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Ausstehend | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | PendingAvailability | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Abgebrochen | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Fehler | Nein | Nein |
| FBM | Auf Lager<br>nicht verwalten | Unversandt | Ja | Ja |
| FBM | Nicht vorrätig | Unversandt | Nein | Nein |
| FBM | Auf Lager<br>nicht verwalten | Teilweise ausgeliefert | Ja | Ja |
| FBM | Nicht vorrätig | Teilweise ausgeliefert | Nein | Nein |
| FBM | Auf Lager<br>nicht verwalten | versandt | Ja | Ja |
| FBM | Nicht vorrätig | versandt | Nein | Nein |

>[!NOTE]
>Wenn eine Amazon-Bestellung in den Status `Partially Shipped` oder `Shipped` importiert wird, gilt für alle Elemente in der Reihenfolge die Lagerplatzreservierung. Der Amazon-Vertriebskanal kompensiert keine zuvor versandten Artikel.
>
>Wenn eine Bestellung von Amazon (FBA) ausgeführt wird, ein Element jedoch den Status `out of stock` aufweist, kann [!DNL Commerce] keine entsprechende Bestellung erstellen. Dies ist eine Einschränkung bei Inventory management-Integrationen.
