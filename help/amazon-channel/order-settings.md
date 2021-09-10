---
title: Bestelleinstellungen
description: 'Verwenden Sie die Bestelleinstellungen, um zu bestimmen, wie Amazon-Bestellungen in Ihren Commerce-Store importiert und dort verarbeitet werden.'
redirect_from: /sales-channels/asc/ob-order-settings.html: 
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 1462
ht-degree: 0%

---

# Bestelleinstellungen

Mit den Bestelleinstellungen wird definiert, ob und wie Amazon-Bestellungen in [!DNL Commerce] importiert und verarbeitet werden. Der Zugriff darauf erfolgt über das [Store-Dashboard](./amazon-store-dashboard.md).

Die Einstellungen für den Bestellimport sind standardmäßig auf `Enabled` eingestellt. Das bedeutet, dass Ihre Amazon-Bestellungen im Store-Dashboard angezeigt werden und die entsprechenden [!DNL Commerce] Bestellungen erstellt werden. Importierte Bestellungen können im Workflow [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} verwaltet werden.

>[!NOTE]
>
>Unabhängig von Ihren Bestelleinstellungen werden Amazon-Bestellungen, die vor Ihrer Store-Integration existierten, nicht importiert.

Nachdem die [Store-Integration](./store-integration.md) abgeschlossen ist, können Sie Ihre Bestelleinstellungen ändern. Wenn Sie Ihre Bestelleinstellungen auf `Disabled` festlegen, werden Amazon-Bestellungen im Store-Dashboard angezeigt, müssen aber in Ihrem [!DNL Amazon Seller Central]-Konto verwaltet werden.

Wenn eine Bestellung in Amazon erstellt wird, wird sie nicht sofort in [!DNL Commerce] importiert. Amazon weist neu erstellten Bestellungen den Status `Pending` zu. Nachdem Amazon die Bestell- und Zahlungsmethode überprüft hat, wird der Auftragsstatus in `Unshipped` geändert. Durch diese Statusänderung wird der Bestellimport Trigger und [!DNL Commerce] erstellt eine übereinstimmende, entsprechende Reihenfolge.

Aus Amazon importierte Bestellungen können im Workflow [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} verwaltet werden. Siehe auch [Bestellungen verwalten](./managing-orders.md).

## Bestelleinstellungen konfigurieren {#configure-order-settings}

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Order Settings]** .

1. Wählen Sie für **[!UICONTROL Import Amazon Orders]** (erforderlich) eine Option:

   - `Disabled` - Wählen Sie aus, wann Sie keine entsprechenden Bestellungen in erstellen möchten,  [!DNL Commerce] wenn neue Bestellungen von Amazon empfangen werden. Wenn diese Option aktiviert ist, sind alle anderen Felder auf dieser Seite deaktiviert.

   - `Enabled` - (Standard) Wählen Sie aus, wann Sie entsprechende  [!DNL Commerce] Bestellungen erstellen möchten, wenn neue Bestellungen von Amazon empfangen werden. [!DNL Commerce] Bestellungen werden basierend auf dem Amazon-Status und den Lagerbeständen erstellt.

      >[!NOTE]
      >
      >Für den Import von Amazon-Bestellungen muss `Enabled` festgelegt sein, damit Amazon-Bestellungen im Workflow [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} verwaltet werden können. Wenn der Wert auf `Disabled` festgelegt ist, weisen Ihre Amazon-Bestellungen keine entsprechende [!DNL Commerce] Bestellnummer auf und können nicht unter [!DNL Commerce] verwaltet werden. Sie verwalten diese Bestellungen in Ihrem [!DNL Amazon Seller Central] -Konto.

1. Wählen Sie für **[!UICONTROL Import Amazon Orders Into Magento Store]** aus, mit welchem [!DNL Commerce] Speicher die Amazon-Bestellungen verknüpft sind, wenn die entsprechende Bestellung in [!DNL Commerce] erstellt wird.

   Diese Einstellung ist standardmäßig die Store-Ansicht für die Website, die ausgewählt wurde, wenn Sie [den Amazon Store](./store-integration.md) hinzugefügt haben. Wenn Sie diese Einstellung ändern möchten, hängt die Liste der Optionen von den [!DNL Commerce] Stores ab, die Sie in Ihrer Konfiguration eingerichtet haben. Siehe [Stores](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){:target=&quot;_blank&quot;}.

1. Wählen Sie für **[!UICONTROL Customer Creation]** eine Option:

   - `No Customer Creation (guest)` - (Standard) Wählen Sie aus, wann Sie kein Kundenkonto in  [!DNL Commerce] Verwendung der importierten Kundendaten aus der Amazon-Bestellung erstellen möchten. Wenn diese Option aktiviert ist, verarbeitet [!DNL Commerce] eine importierte Amazon-Bestellung auf die gleiche Weise wie ein Gastkasse in [!DNL Commerce].

   - `Build New Customer Account` - Wählen Sie aus, wann Sie ein neues Kundenkonto unter  [!DNL Commerce] Verwendung der mit der Amazon-Bestellung importierten Kundendaten erstellen möchten. Diese Option hilft beim Aufbau Ihrer Kundendatenbank anhand Ihrer Amazon-Bestellungen.

1. Wählen Sie für **[!UICONTROL Order Number Source]** eine Option:

   - `Build Using Magento Order Number` - (Standard) Wählen Sie aus, wann Sie eine eindeutige  [!DNL Commerce] Bestellnummer für die entsprechende Amazon-Bestellung mit der  [!DNL Commerce] inkrementell zugewiesenen Bestell-ID erstellen möchten.

   - `Build Using Amazon Order Number` - Wählen Sie aus, wann Sie die  [!DNL Commerce] Bestellnummer mit der entsprechenden von Amazon zugewiesenen Bestellnummer erstellen möchten.
   >[!NOTE]
   >
   >Nach dem Import einer Bestellung wird die Amazon-Bestellnummer in der Liste _[!UICONTROL Recent Orders]_im Store-Dashboard angezeigt. Die Bestellnummer [!DNL Commerce] wird angezeigt, wenn die Bestelldetails im Arbeitsbereich [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} angezeigt werden.

1. Wählen Sie für **[!UICONTROL Order Status]** (erforderlich) eine Option:

   - `Default Order Status` - (Standard) Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, Ihr Standardbestellungsstatus für neue Bestellungen zugewiesen werden soll. Der Standardstatus für neue Bestellungen (es sei denn, Sie haben einen benutzerdefinierten Bestellstatus für neue Bestellungen erstellt) ist `Pending`. Siehe [Verarbeitungsaufträge](https://docs.magento.com/user-guide/sales/order-processing.html){:target=&quot;_blank&quot;}.

   - `Custom Order Status` - Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, ein anderer Status als der Standardstatus zugewiesen werden soll.

   - `Processing Order Status` - Aktiviert, wenn  **[!UICONTROL Order Status]** auf  `Custom Order Status`gesetzt ist. Wählen Sie den Status aus, den Sie für neu erstellte, aus Amazon importierte Bestellungen verwenden möchten. Die Optionen in diesem Feld basieren auf den Standardstatusoptionen in [!DNL Commerce]. Siehe [Bestellstatus](https://docs.magento.com/user-guide/sales/order-status.html). Sie können auch einen benutzerdefinierten Bestellstatus erstellen, der hier zur Auswahl angezeigt wird. Informationen zum Erstellen eines benutzerdefinierten Bestellstatus finden Sie unter [Benutzerdefinierter Bestellstatus](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;}.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save order settings]**.

![Bestelleinstellungen](assets/amazon-order-settings.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Import Amazon Orders] | Optionen:<ul><li>**[!UICONTROL Disabled]** - Wählen Sie aus, wann Sie keine entsprechenden Bestellungen in erstellen möchten,  [!DNL Commerce] wenn neue Bestellungen von Amazon empfangen werden. Wenn diese Option aktiviert ist, sind alle anderen Felder auf dieser Seite deaktiviert.</li><li>**[!UICONTROL Enabled]** - (Standard) Wählen Sie aus, wann Sie entsprechende  [!DNL Commerce] Bestellungen erstellen möchten, wenn neue Bestellungen von Amazon empfangen werden. [!DNL Commerce] Bestellungen werden basierend auf dem Amazon-Status und den Lagerbeständen erstellt.</li></ul><br><br>`Enabled` muss ausgewählt sein, um Amazon-Bestellungen in zu verwalten  [!DNL Commerce]. Wenn `Disabled` ausgewählt ist, werden Ihre Amazon-Bestellungen im Store-Dashboard angezeigt, die Bestellungen müssen jedoch in Ihrem [!DNL Amazon Seller Central]-Konto verwaltet werden. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Wählen Sie aus, mit welchen [!DNL Commerce]-Speichern die Amazon-Bestellungen verknüpft sind, wenn sie im Arbeitsbereich [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} erstellt werden. Diese Einstellung ist standardmäßig die Store-Ansicht für die [!DNL Commerce]-Website, die ausgewählt wurde, als [Sie den Amazon Store](./store-integration.md) hinzugefügt haben. Wenn Sie diese Einstellung ändern möchten, hängt die Liste der Optionen von den [!DNL Commerce] Stores ab, die Sie in Ihrer Konfiguration eingerichtet haben. Siehe [Stores](https://docs.magento.com/user-guide/stores/stores-all-stores.html){:target=&quot;_blank&quot;}. |
| [!UICONTROL Customer Creation] | Optionen:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Standard) Wählen Sie aus, wann Sie kein Kundenkonto in  [!DNL Commerce] Verwendung der importierten Kundendaten aus der Amazon-Bestellung erstellen möchten. Wenn diese Option aktiviert ist, weist [!DNL Commerce]  an, eine importierte Amazon-Bestellung auf dieselbe Weise zu verarbeiten wie ein Gast-Checkout.</li><li>**[!UICONTROL Build New Customer Account]** - Wählen Sie aus, wann Sie ein neues Kundenkonto in Ihrer  [!DNL Commerce] Kundendatenbank mit den mit der Amazon-Bestellung importierten Kundendaten erstellen möchten. Diese Option hilft beim Erstellen Ihrer [!DNL Commerce] Kundendatenbank aus Ihren Amazon-Bestellungen.</li></ul> |
| Bestellnummer | Optionen:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Standard) Wählen Sie aus, wann Sie eine eindeutige  [!DNL Commerce] Bestellnummer für die entsprechende Amazon-Bestellung mit der  [!DNL Commerce] inkrementell zugewiesenen Bestell-ID erstellen möchten. </li><li>**Mit Amazon-Bestellnummer erstellen**  - Wählen Sie aus, wann Sie die  [!DNL Commerce] Bestellnummer mit der entsprechenden Amazon-zugewiesenen Bestellnummer erstellen möchten.</li></ul> |
| Ausstehende Bestellungen | Optionen:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Wählen Sie aus, wann Ihre  [!DNL Commerce] Lagermenge nicht von Ihren Amazon-Bestellungen betroffen sein soll. Wählen Sie aus, ob Sie Amazon für Ihren FBA-Prozess (FBA) verwenden. Wenn Sie eine Amazon-Bestellung erhalten, wirkt sich die bestellte Menge nicht auf Ihre [!DNL Commerce] Lagermenge aus.</li><li>**[!UICONTROL Reserve Quantity]** - Wählen Sie aus, wann die Bestellmenge in der Amazon in Ihrer  [!DNL Commerce] Lagermenge &quot;reserviert&quot;werden soll. Wenn Sie eine Amazon-Bestellung erhalten, wird die bestellte Menge in Ihrer [!DNL Commerce] Lagermenge &quot;reserviert&quot;, um zu verhindern, dass Ihr [!DNL Commerce]-Lager &quot;überverkauft&quot;wird. Die &quot;reservierte&quot; Menge kann nicht über Ihre [!DNL Commerce] Storefront gekauft werden.</li></ul> |
| [!UICONTROL Order Status] | Optionen:<ul><li>**[!UICONTROL Default Order Status]** - (Standard) Wählen Sie aus, wann neu erstellten Bestellungen, die aus Amazon importiert wurden, Ihr Standardbestellungsstatus für neue Bestellungen zugewiesen werden soll. Der Standardstatus für neue Bestellungen (es sei denn, Sie haben einen benutzerdefinierten Bestellstatus für neue Bestellungen erstellt) ist `Pending`. Siehe [Verarbeitungsaufträge](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]** - Wählen Sie aus, wann neu erstellten aus Amazon importierten Bestellungen ein anderer Status als der Standardstatus zugewiesen werden soll. Wenn diese Option aktiviert ist, können Sie mit **[!UICONTROL Processing Order Status]** den Status auswählen, den Sie für neu erstellte, aus Amazon importierte Bestellungen verwenden möchten.</li></ul> |
| [!UICONTROL Processing Orders Status] | Aktiviert, wenn _[!UICONTROL Order Status]_auf `Custom Order Status` gesetzt ist. Wählen Sie den Bestellstatus aus, den Sie neuen Bestellungen zuweisen möchten. Die Optionen in diesem Feld hängen von den Standardstatusoptionen in [!DNL Commerce] ab. Siehe [Bestellstatus](https://docs.magento.com/user-guide/sales/order-status.html){:target=&quot;_blank&quot;}. Sie können auch einen benutzerdefinierten Bestellstatus erstellen, der hier angezeigt wird. Informationen zum Erstellen eines benutzerdefinierten Bestellstatus finden Sie unter [Benutzerdefinierter Bestellstatus](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;}. |

## [!DNL Commerce] Auftragserstellung

[!DNL Commerce] Bestellungen werden für Amazon-Bestellungen basierend auf den folgenden Status- und Lagerbedingungen erstellt.

### Auftragserstellung mit Lagerbestandsverwaltung

>[!NOTE]
>
>Wird nur in Adobe Commerce- und Magento Open Source 2.3.x-Integrationen unterstützt.

| Fulfillment-Kanal | [!DNL Commerce] Inventarstatus | Amazon-Bestellstatus | [!UICONTROL Create Magento Order] Einstellung | Bestand reserviert |
|---|---|---|---|---|
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Ausstehend | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | PendingAvailability | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Abgebrochen | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Fehler | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Unversandt | Nein | Nein |
| FBA | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Teilweise ausgeliefert | Nein | Nein |
| FBA | Auf Lager<br>Nicht verwalten | versandt | Ja | Nein |
| FBA | Nicht vorrätig | versandt | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Ausstehend | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | PendingAvailability | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Abgebrochen | Nein | Nein |
| FBM | Vorrätig<br>Nicht vorrätig<br>Nicht verwalten | Fehler | Nein | Nein |
| FBM | Auf Lager<br>Nicht verwalten | Unversandt | Ja | Ja |
| FBM | Nicht vorrätig | Unversandt | Nein | Nein |
| FBM | Auf Lager<br>Nicht verwalten | Teilweise ausgeliefert | Ja | Ja |
| FBM | Nicht vorrätig | Teilweise ausgeliefert | Nein | Nein |
| FBM | Auf Lager<br>Nicht verwalten | versandt | Ja | Ja |
| FBM | Nicht vorrätig | versandt | Nein | Nein |

>[!NOTE]
>Wenn eine Amazon-Bestellung in den Status `Partially Shipped` oder `Shipped` importiert wird, gilt für alle Elemente in der Reihenfolge die Erstellung einer Lagerbestandsreservierung. Der Amazon-Vertriebskanal kompensiert keine zuvor versandten Artikel.
>
>Wenn eine Bestellung von Amazon (FBA) ausgeführt wird, ein Element jedoch den Status `out of stock` aufweist, kann [!DNL Commerce] keine entsprechende Bestellung erstellen. Dies ist eine Beschränkung der Lagerbestandsverwaltungsintegrationen.
