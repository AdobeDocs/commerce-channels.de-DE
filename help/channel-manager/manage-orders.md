---
title: Verwalten von Walmart Marketplace-Bestellungen
description: Anzeigen und Verwalten [!DNL Walmart Marketplace] Bestellungen mit [!DNL Channel Manager] für Adobe Commerce und Magento Open Source.
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: ec85dc2496c22cd8173c550ca35f2bd207501c19
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Verwalten von Walmart Marketplace-Bestellungen

[!DNL Walmart Marketplace] Bestellungen [!DNL Commerce] Produktlisten werden automatisch synchronisiert zu [!DNL Channel Manager] nachdem Walmart die Bestellung bearbeitet hat. Wenn die Synchronisierung abgeschlossen ist, können Sie die Bestellinformationen anzeigen, indem Sie **[!UICONTROL Orders]** aus der Ansicht des verbundenen Kanalspeichers in [!DNL Channel Manager].

![Ansicht &quot;Channel Manager Orders&quot;zur Verwaltung von Walmart Marketplace-Bestellungen](assets/orders-dashboard-view.png)

>[!NOTE]
>
>Es kann bis zu 35 Minuten dauern für eine [!DNL Walmart Marketplace] Reihenfolge der Anzeige im [!DNL Channel Manager] Bestellliste. [!DNL Walmart] benötigt ca. 30 Minuten, um eingehende Bestellungen zu verarbeiten und an [!DNL Channel Manager]. Nachdem der Kanal-Manager die Bestellung erhalten hat, dauert es etwa fünf Minuten, bis die Bestellung in Adobe Commerce oder Magento Open Source erstellt und angezeigt wird.

## Bestellungen überprüfen

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** , um [!UICONTROL Channel Manager Marketplace Stores] Seite.

1. Öffnen Sie die Store-Ansicht, indem Sie das Stiftsymbol in einer Store-Einstiegszeile auswählen.

1. Um Bestellinformationen anzuzeigen, klicken Sie auf *[!UICONTROL *Orders]**.

1. Informationen über die Reihenfolge abrufen und die nächsten Schritte bestimmen, indem Sie die **[Status](#about-order-status)** -Spalte, um Informationen zu den Bestellungen zu erhalten.

## Bestelldetails anzeigen

Nachdem eine Bestellung vom Marktplatz empfangen und in die Adobe Commerce oder Magento Open Source importiert wurde, verwenden Sie die [!DNL Commerce] Bestell-ID zum Anzeigen der Bestellung in Adobe Commerce.

Von **[!UICONTROL Orders]**, wählen Sie die **[!UICONTROL Commerce Order Number]** , um [!DNL Commerce] Bestelldetails.

![Commerce Order detail view for a Walmart Marketplace order](assets/order-detail-with-external-order-id.png)

### Bestellsteuerung und Spaltenbeschreibungen

In den folgenden Tabellen werden die für Bestellungen verfügbaren Steuerelemente und Spalten beschrieben.

**Steuerelemente für[!UICONTROL Orders]**
| **Kontrolle**                    | **Beschreibung**                                                                                                                                               | |—|—| | [!UICONTROL Filter orders]     | Sortieren Sie die Ansicht, indem Sie eine der [!UICONTROL Order Status] Karten.                                                                                        | | Fehlermeldungsdetails | Bewegen Sie den Mauszeiger über die [!UICONTROL Error Status] für eine Bestellung, um die detaillierte Fehlermeldung anzuzeigen.                                                                      | | [!UICONTROL View order detail] | Um Bestelldetails anzuzeigen, wählen Sie die [!DNL Commerce] Bestellnummer im [!UICONTROL Order] Tabelle. Verwenden Sie dann [!DNL Commerce] Bestelloptionen, um die Bestellung zu verarbeiten. |

**Spaltenbeschreibungen**

| Feld | Beschreibung |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL  Walmart Order Number] | Die Bestellnummer, die der Bestellung in der [!DNL Walmart Marketplace]. Beim erstmaligen Import einer Bestellung in [!DNL Channel Manager], wird nur die Walmart-Bestellnummer angezeigt. Wenn die [!DNL Commerce] -Reihenfolge erstellt wird, wird die [!DNL Walmart] Die Bestellnummer wird im [!UICONTROL External ID] Produktattribut. |
| [!DNL Commerce]  Bestellnummer | Die der [!DNL Commerce]  aus der [!DNL Walmart Marketplace] bestellen. |
| Elemente | Anzahl der bestellten Artikel [!DNL Walmart Marketplace]. |
| [!UICONTROL Order Value] | Gesamtkosten der bestellten Artikel. |
| [!UICONTROL Date Created] | Das Datum, an dem die Bestellung erstellt wurde [!DNL Walmart Marketplace]. |
| [!UICONTROL Ship By Date] | Datum, an dem die Bestellung versandt werden muss, um sie zu erfüllen [!DNL Walmart Marketplace] Anforderungen. |
| [!UICONTROL Order Status] | Gibt den aktuellen Bestellstatus im [!DNL Commerce] Bestellworkflow. Der Status wird aktualisiert, wenn Sie erfolgreich Produkte zu [!DNL Channel Manager] und wenn Sie Produkte auf der [!DNL Walmart Marketplace]. Wenn ein Vorgang fehlschlägt, wird in der Liste der Fehlerstatus angezeigt. Nachdem Sie den Fehler behoben haben, [!DNL Channel Manager] wiederholt den Vorgang und aktualisiert den Status. |

| [!UICONTROL Error description]    | Bietet detailliertere Informationen zu Bestellungen mit einer *Fehler* status.|

### Über den Bestellstatus

[!UICONTROL Order Status] liefert Informationen zum aktuellen Status von [!DNL Walmart Marketplace] Bestellungen, die von Adobe Commerce oder Magento Open Source verwaltet werden. Aktualisierungen des Bestellstatus treten auf, wenn [!DNL Channel Manager] erhält aktualisierte Bestellinformationen von entweder [!DNL Walmart Marketplace] oder [!DNL Commerce] Bestellsystem. Bestellungen können den folgenden Status aufweisen:

* **[!UICONTROL Open]**-Bestellungen, die von der [!DNL Walmart Marketplace] bereit zur Überprüfung und Verarbeitung in Adobe Commerce oder Magento Open Source.

   Nachdem ein Kunde ein Produkt von der [!DNL Walmart Marketplace]kann es bis zu 35 Minuten dauern, bis die geöffnete Bestellung im Arbeitsbereich für die Bestellung des verbundenen Kanals angezeigt wird. [!DNL Commerce] benötigt ca. 30 Minuten, um eingehende Bestellungen zu verarbeiten und an [!DNL Channel Manager]. Nachdem der Kanal-Manager die Bestellung erhalten hat, dauert es fünf weitere Minuten, um die [!DNL Commerce] bestellen.

* **[!UICONTROL Processed]**-Bestellungen, die versandt, storniert oder von der [!DNL Commerce] speichern.

   Um alle versandten, stornierten und rückerstatteten Bestellungen anzuzeigen, wählen Sie die **Verarbeitet** Statuskarte.

* **[!UICONTROL Canceled]**-Bestellungen, die vom [!DNL Commerce] speichern.

   Nach Abschluss der Auftragsstornierung wird die [!DNL Commerce] Bestandsmengenaktualisierungen, um die zurückgegebenen Elemente widerzuspiegeln. Dann [!DNL Channel Manager] synchronisiert die Aktualisierung mit dem [!DNL Walmart Marketplace].

* **[!UICONTROL Refunded]**-Bestellungen, die vom [!DNL Commerce] speichern.

   Nach Abschluss der Rückerstattung wird die [!DNL Commerce] Bestandsmengenaktualisierungen, um die erstatteten Artikel widerzuspiegeln. Dann [!DNL Channel Manager] synchronisiert die Aktualisierung mit dem [!DNL Walmart Marketplace].

* **[!UICONTROL Error]**- Fehlerhafte Bestellungen. Fehler können auftreten, wenn ein Bestellaktualisierungsvorgang fehlschlägt. Beispielsweise treten Fehler auf, wenn [!DNL Channel Manager] kann keine neue Bestellung von Walmart erhalten. Sie können auch auftreten, wenn [!DNL Channel Manager] kann eine Auftragsversand- oder Löschungsaktualisierung nicht an die [!DNL Walmart Marketplace].

* **[!UICONTROL Error description]**-Enthält detaillierte Informationen zu Bestellfehlern, die aufgrund von Problemen auftreten, wie fehlende Informationen oder ungültige Werte, falsche Versanddetails oder eine fehlgeschlagene Auftragsstornierung. Anhand der Beschreibung kann festgestellt werden, ob ein Fehler auf der [!DNL Commerce] -Instanz oder auf [!DNL Walmart Marketplace].
