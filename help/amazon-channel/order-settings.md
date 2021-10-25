---
title: Auftragseinstellungen
description: Verwenden Sie die Bestelleinstellungen, um zu bestimmen, wie Amazon-Bestellungen in Ihren Commerce-Store importiert und verarbeitet werden.
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Auftragseinstellungen

Mit den Auftragseinstellungen wird festgelegt, ob und wie Amazon-Bestellungen in importiert und verarbeitet werden. [!DNL Commerce] und kann auf der [Dashboard speichern](./amazon-store-dashboard.md).

Die Importeinstellungen für die Reihenfolge sind auf `Enabled` Standardmäßig werden Ihre Amazon-Bestellungen im Store-Dashboard angezeigt und erstellen Sie die entsprechenden [!DNL Commerce] Bestellungen. Importierte Bestellungen können verwaltet werden im [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html)Workflow für {Zielgruppe=&quot;_blank&quot;}.

>[!NOTE]
>
>Unabhängig von Ihren Bestelleinstellungen werden Amazon-Bestellungen, die vor der Store-Integration bestanden, nicht importiert.

Nach [Speicherintegration](./store-integration.md) ist abgeschlossen, können Sie Ihre Bestelleinstellungen ändern. Wenn Sie die Bestelleinstellungen auf `Disabled`, werden Amazon-Bestellungen auf dem Store-Dashboard angezeigt, müssen aber in Ihrer [!DNL Amazon Seller Central] Konto.

Wenn eine Bestellung auf Amazon erstellt wird, wird sie nicht sofort in importiert [!DNL Commerce]. Amazon weist ein `Pending` Status auf neu erstellte Bestellungen. Nachdem Amazon die Bestellungs- und Zahlungsmethode überprüft hat, wird der Status der Bestellung geändert in `Unshipped`. Diese Statusänderung Trigger den Auftragsimport und [!DNL Commerce] erstellt eine entsprechende Reihenfolge.

Aus Amazon importierte Bestellungen können verwaltet werden in [!DNL Commerce] [Auftragsarbeitsablauf](https://docs.magento.com/user-guide/sales/orders.html){Zielgruppe=&quot;_blank&quot;}. Siehe auch [Bestellungen verwalten](./managing-orders.md).

## Auftragseinstellungen konfigurieren {#configure-order-settings}

1. Klick **[!UICONTROL Order Settings]** auf dem Dashboard.

1. für **[!UICONTROL Import Amazon Orders]** (erforderlich), wählen Sie eine Option aus:

   - `Disabled` - Wählen Sie aus, wenn Sie keine entsprechenden Bestellungen erstellen möchten in [!DNL Commerce] wenn neue Bestellungen von Amazon eingegangen sind. Bei Auswahl dieser Option sind alle anderen Felder auf dieser Seite deaktiviert.

   - `Enabled` - (Standard) Wählen Sie aus, wann Sie entsprechende Elemente erstellen möchten [!DNL Commerce] Bestellungen bei neuen Bestellungen von Amazon. [!DNL Commerce] Bestellungen werden auf Basis des Amazon-Status und der Lagerbestände erstellt.

      >[!NOTE]
      >
      >Amazon-Aufträge importieren muss auf `Enabled` zur Verwaltung von Amazon-Bestellungen im [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html)Workflow für {Zielgruppe=&quot;_blank&quot;}. Wenn festgelegt auf `Disabled`, haben Ihre Amazon-Bestellungen keine entsprechende [!DNL Commerce] Auftragsnummer und kann nicht verwaltet werden in [!DNL Commerce]. Sie verwalten diese Aufträge in Ihren [!DNL Amazon Seller Central] Konto.

1. für **[!UICONTROL Import Amazon Orders Into Magento Store]**, welche [!DNL Commerce] speichern Sie die Amazon-Bestellungen, mit denen verbunden ist, wenn die entsprechende Bestellung erstellt wurde in [!DNL Commerce].

   Diese Einstellung setzt standardmäßig auf die Store-Ansicht der Website, die bei der Auswahl ausgewählt wurde [hat Amazon Store hinzugefügt](./store-integration.md). Wenn Sie diese Einstellung ändern möchten, hängt die Liste der Optionen von der [!DNL Commerce] speichert, die Sie in Ihrer Konfiguration eingerichtet haben. Siehe [Geschäfte](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){Zielgruppe=&quot;_blank&quot;}.

1. für **[!UICONTROL Customer Creation]**, wählen Sie eine Option aus:

   - `No Customer Creation (guest)` - (Standard) Wählen Sie aus, wenn Sie kein Kundenkonto erstellen möchten in [!DNL Commerce] Verwendung der importierten Kundendaten aus der Amazon-Bestellung. Wenn ausgewählt, [!DNL Commerce] verarbeitet eine importierte Amazon-Bestellung auf die gleiche Weise wie ein Gast-Checkout in [!DNL Commerce].

   - `Build New Customer Account` - Wählen Sie aus, wann Sie ein neues Kundenkonto erstellen möchten in [!DNL Commerce] die mit der Amazon-Bestellung importierten Kundendaten verwenden. Mit dieser Option können Sie Ihre Kundendatenbank aus Ihren Amazon-Bestellungen aufbauen.

1. für **[!UICONTROL Order Number Source]**, wählen Sie eine Option aus:

   - `Build Using Magento Order Number` - (Standard) Wählen Sie aus, wann Sie eine eindeutige Datei erstellen möchten [!DNL Commerce] Bestellnummer für entsprechende Amazon-Bestellung unter Verwendung der [!DNL Commerce] inkrementell zugewiesene Bestell-ID.

   - `Build Using Amazon Order Number` - Wählen Sie aus, wann Sie die [!DNL Commerce] Bestellnummer unter Verwendung der entsprechenden Amazon-zugewiesenen Bestellnummer.
   >[!NOTE]
   >
   >Nach dem Importieren einer Bestellung wird die Amazon-Bestellnummer im _[!UICONTROL Recent Orders]_Liste auf dem Dashboard des Ladens. Die [!DNL Commerce] Bestellnummer wird angezeigt, wenn die Auftragsdetails im [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){Zielgruppe=&quot;_blank&quot;} Arbeitsbereich.

1. für **[!UICONTROL Order Status]** (erforderlich), wählen Sie eine Option aus:

   - `Default Order Status` - (Standard) Wählen Sie aus, wann neu erstellte Bestellungen, die aus Amazon importiert wurden, Ihrem definierten Standardbestellstatus für neue Bestellungen zugewiesen werden sollen. Der Standardstatus für neue Bestellungen (es sei denn, Sie haben einen benutzerdefinierten Bestellstatus für neue Bestellungen erstellt) ist `Pending`. Siehe [Bestellungen werden verarbeitet](https://docs.magento.com/user-guide/sales/order-processing.html){Zielgruppe=&quot;_blank&quot;}.

   - `Custom Order Status` - Wählen Sie aus, wann neu erstellte Bestellungen aus Amazon einem anderen Status als dem Standardstatus zugewiesen werden sollen.

   - `Processing Order Status` - Aktiviert bei **[!UICONTROL Order Status]** ist eingestellt auf `Custom Order Status`. Wählen Sie den Status aus, den Sie für neu erstellte Bestellungen verwenden möchten, die aus Amazon importiert wurden. Die Optionen in diesem Feld basieren auf den Standardstatusoptionen in [!DNL Commerce]. Siehe [Auftragsstatus](https://docs.magento.com/user-guide/sales/order-status.html). Sie können auch einen benutzerdefinierten Bestellstatus erstellen, der hier zur Auswahl angezeigt wird. Informationen zum Erstellen eines benutzerdefinierten Bestellstatus finden Sie unter [Benutzerdefinierter Auftragsstatus](https://docs.magento.com/user-guide/sales/order-status-custom.html){Zielgruppe=&quot;_blank&quot;}.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save order settings]**.

![Auftragseinstellungen](assets/amazon-order-settings.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Import Amazon Orders] | Optionen:<ul><li>**[!UICONTROL Disabled]** - Wählen Sie aus, wenn Sie keine entsprechenden Bestellungen erstellen möchten in [!DNL Commerce] wenn neue Bestellungen von Amazon eingegangen sind. Bei Auswahl dieser Option sind alle anderen Felder auf dieser Seite deaktiviert.</li><li>**[!UICONTROL Enabled]** - (Standard) Wählen Sie aus, wann Sie entsprechende Elemente erstellen möchten [!DNL Commerce] Bestellungen bei neuen Bestellungen von Amazon. [!DNL Commerce] Bestellungen werden auf Basis des Amazon-Status und der Lagerbestände erstellt.</li></ul><br><br>`Enabled` muss zur Verwaltung von Amazon-Bestellungen in [!DNL Commerce]. Wann `Disabled` ausgewählt wurde, werden Ihre Amazon-Bestellungen im Store-Dashboard angezeigt, die Bestellungen müssen jedoch in Ihrer [!DNL Amazon Seller Central] Konto. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Auswählen [!DNL Commerce] speichern Sie die Amazon-Bestellungen, mit denen sie verbunden sind, wenn sie in der [!DNL Commerce] [Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){Zielgruppe=&quot;_blank&quot;} Arbeitsbereich. Diese Einstellung setzt standardmäßig auf die Store-Ansicht für [!DNL Commerce] Website ausgewählt, wenn [hat Amazon Store hinzugefügt](./store-integration.md). Wenn Sie diese Einstellung ändern möchten, hängt die Liste der Optionen von der [!DNL Commerce] speichert, die Sie in Ihrer Konfiguration eingerichtet haben. Siehe [Geschäfte](https://docs.magento.com/user-guide/stores/stores-all-stores.html){Zielgruppe=&quot;_blank&quot;}. |
| [!UICONTROL Customer Creation] | Optionen:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Standard) Wählen Sie aus, wenn Sie kein Kundenkonto erstellen möchten in [!DNL Commerce] Verwendung der importierten Kundendaten aus der Amazon-Bestellung. Wenn diese Option ausgewählt ist, teilt diese Option Folgendes mit: [!DNL Commerce] um eine importierte Amazon-Bestellung auf die gleiche Weise wie ein Gast-Checkout zu verarbeiten.</li><li>**[!UICONTROL Build New Customer Account]** - Wählen Sie aus, wann Sie ein neues Kundenkonto in Ihrem [!DNL Commerce] Kundendatenbank unter Verwendung der mit der Amazon-Bestellung importierten Kundendaten. Diese Option hilft Ihnen bei der Erstellung Ihrer [!DNL Commerce] Kundendatenbank aus Ihren Amazon-Bestellungen.</li></ul> |
| Auftragsnummernquelle | Optionen:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Standard) Wählen Sie aus, wann Sie eine eindeutige Datei erstellen möchten [!DNL Commerce] Bestellnummer für entsprechende Amazon-Bestellung unter Verwendung der [!DNL Commerce] inkrementell zugewiesene Bestell-ID. </li><li>**Erstellen mit Amazon-Auftragsnummer** - Wählen Sie aus, wann Sie die [!DNL Commerce] Bestellnummer unter Verwendung der entsprechenden Amazon-zugewiesenen Bestellnummer.</li></ul> |
| Ausstehende Aufträge | Optionen:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Wählen Sie aus, wenn Sie Ihre [!DNL Commerce] die von Ihren Amazon-Bestellungen betroffene Lagermenge. Wählen Sie aus, ob Sie Amazon für Ihren FBA-Prozess verwenden. Wenn Sie eine Bestellung bei Amazon erhalten, wirkt sich die bestellte Menge nicht auf Ihre Bestellung aus [!DNL Commerce] Bestandsmenge.</li><li>**[!UICONTROL Reserve Quantity]** - Wählen Sie aus, wann die Bestellmenge im Amazon &quot;reserviert&quot; werden soll. [!DNL Commerce] Bestandsmenge. Wenn Sie eine Bestellung bei Amazon erhalten, wird die bestellte Menge in Ihrem [!DNL Commerce] zur Vermeidung Ihrer [!DNL Commerce] Bestand aus &quot;Überverkauf&quot;. Die &quot;reservierte&quot; Menge steht nicht zum Kauf über [!DNL Commerce] Schaufenster.</li></ul> |
| [!UICONTROL Order Status] | Optionen:<ul><li>**[!UICONTROL Default Order Status]** - (Standard) Wählen Sie aus, wann neu erstellte Bestellungen aus Amazon Ihrem Standardbestellstatus für neue Bestellungen zugewiesen werden sollen. Der Standardstatus für neue Bestellungen (es sei denn, Sie haben einen benutzerdefinierten Bestellstatus für neue Bestellungen erstellt) ist `Pending`. Siehe [Bestellungen werden verarbeitet](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]** - Wählen Sie aus, wann neu erstellte Bestellungen aus Amazon einem anderen Status als dem Standardstatus zugewiesen werden sollen. Wenn ausgewählt, **[!UICONTROL Processing Order Status]** ermöglicht es Ihnen, den Status auszuwählen, den Sie für neu erstellte Bestellungen verwenden möchten, die aus Amazon importiert werden.</li></ul> |
| [!UICONTROL Processing Orders Status] | Aktiviert bei _[!UICONTROL Order Status]_ist eingestellt auf `Custom Order Status`. Wählen Sie den Bestellstatus, den Sie neuen Bestellungen zuweisen möchten. Die Optionen in diesem Feld hängen von den Standardstatusoptionen in [!DNL Commerce]. Siehe [Auftragsstatus](https://docs.magento.com/user-guide/sales/order-status.html){Zielgruppe=&quot;_blank&quot;}. Sie können hier auch einen benutzerdefinierten Bestellstatus erstellen. Informationen zum Erstellen eines benutzerdefinierten Bestellstatus finden Sie unter [Benutzerdefinierter Auftragsstatus](https://docs.magento.com/user-guide/sales/order-status-custom.html){Zielgruppe=&quot;_blank&quot;}. |

## [!DNL Commerce] Auftragserstellung

[!DNL Commerce] Bestellungen werden für Amazon Bestellungen auf Basis der folgenden Status- und Bestandsbedingungen erstellt.

### Auftragserstellung mit Lagerbestandsverwaltung

>[!NOTE]
>
>Wird nur in Adobe Commerce und Magento Open Source 2.3.x-Integrationen unterstützt.

| Fulfillment-Kanal | [!DNL Commerce] Bestandsstatus | Amazon-Auftragsstatus | [!UICONTROL Create Magento Order] Einstellung | Bestand reserviert |
|---|---|---|---|---|
| FBA | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Ausstehend | Nein | Nein |
| FBA | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Ausstehende Verfügbarkeit | Nein | Nein |
| FBA | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Abgebrochen | Nein | Nein |
| FBA | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Fehler | Nein | Nein |
| FBA | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Nicht versandt | Nein | Nein |
| FBA | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Teilweise versandt | Nein | Nein |
| FBA | Auf Lager<br>Nicht verwalten | Versand | Ja | Nein |
| FBA | Nicht auf Lager | Versand | Nein | Nein |
| FBM | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Ausstehend | Nein | Nein |
| FBM | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Ausstehende Verfügbarkeit | Nein | Nein |
| FBM | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Abgebrochen | Nein | Nein |
| FBM | Auf Lager<br>Nicht auf Lager<br>Nicht verwalten | Fehler | Nein | Nein |
| FBM | Auf Lager<br>Nicht verwalten | Nicht versandt | Ja | Ja |
| FBM | Nicht auf Lager | Nicht versandt | Nein | Nein |
| FBM | Auf Lager<br>Nicht verwalten | Teilweise versandt | Ja | Ja |
| FBM | Nicht auf Lager | Teilweise versandt | Nein | Nein |
| FBM | Auf Lager<br>Nicht verwalten | Versand | Ja | Ja |
| FBM | Nicht auf Lager | Versand | Nein | Nein |

>[!NOTE]
>Wenn eine Amazon-Bestellung in eine `Partially Shipped` oder `Shipped` -Status, die erstellte Lagerungsreservierung ist für alle Artikel in der Bestellung. Amazon Sales Kanal kompensiert nicht die zuvor versandten Artikel.
>
>Wenn eine Bestellung von Amazon (FBA) ausgefüllt wurde, jedoch ein Artikel in `out of stock` Status, [!DNL Commerce] kann keine entsprechende Bestellung erstellen. Dies ist eine Beschränkung der Lagerbestandsverwaltung.
