---
title: Erstellen und Bearbeiten von Attributen für den Amazon-Vertriebskanal
description: Amazon Sales Channel bietet die Ansicht "Attributes", mit der Sie die aktuellen Amazon-Attribute und verknüpften Commerce-Attribute überprüfen können.
feature: Sales Channels, Products, Configuration
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# Attribute erstellen und bearbeiten

Erstellen oder aktualisieren [!DNL Commerce] -Attribute, während Sie über Amazon verkaufen und Ihre Geschäfte aktualisieren. Überprüfen Sie die aktuellen Amazon-Attribute und verknüpften [!DNL Commerce] -Attribute über die [_[!UICONTROL Attributes]_Ansicht](./attributes-view.md) der Startseite des Amazon-Vertriebskanals. Die_[!UICONTROL Action]_ zeigt die verfügbaren Aktionen für das Attribut an. Sie können entweder eine neue [!DNL Commerce] für ein nicht verknüpftes Amazon-Attribut oder Sie können ein vorhandenes [!DNL Commerce] -Attribut und dessen Zuordnung zu einem Amazon-Attribut.

Beim Erstellen und Aktualisieren von Attributen sollten Sie die Attributwerte für [!DNL Commerce] und Amazon-Produkte. Diese Werte unterscheiden sich möglicherweise, wenn Sie keine Werte aus Amazon synchronisieren und importieren. Informationen zum Überprüfen der Amazon-Werte für diese Attribute finden Sie unter [Überprüfen der Amazon-Attributzuordnung](./amazon-matching-attributes-values.md). Wenn Sie diese Werte ändern möchten, können Sie [Bearbeiten oder Erstellen einer Zuordnung](./amazon-manually-update-incomplete-listing.md) zwischen Amazon und [!DNL Commerce].

## Attribut erstellen {#create-an-attribute}

Diese Schritte erstellen eine [!DNL Commerce] zuordnen und sie einem Amazon-Attribut zuzuordnen. Je nach Konfiguration können die Werte mit der Synchronisierung zwischen Katalogen beginnen.

1. Im _Admin_ Seitenleiste, navigieren Sie zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicks **[!UICONTROL Attributes]** Suchen Sie im Menü links nach einem Amazon-Attribut und klicken Sie auf **[!UICONTROL Create Attribute]** im _[!UICONTROL Action]_Spalte.

1. So aktivieren Sie die Synchronisierung der Amazon-Werte mit der verknüpften [!DNL Commerce] Attribut festlegen **[!UICONTROL Is Active]** nach `Yes`.

   Wenn festgelegt auf `Yes`, werden die Werte gemäß Ihrer Konfiguration synchronisiert.

1. Auswählen `Create New Magento Attribute` für **[!UICONTROL Select Magento Product Attribute]**.

   Das Attribut wird dem für **[!UICONTROL Amazon Attribute Name]**.

1. Geben Sie einen **[!UICONTROL Magento Product Attribute Name]**.

1. Geben Sie einen **[!UICONTROL Magento Product Attribute Code]**.

   Dieser Wert muss in Kleinbuchstaben ohne Leerzeichen eingegeben werden.

1. Für **[!UICONTROL Attribute Set Ids]** auswählen, wählen Sie einen Attributsatz, der zugewiesen werden soll.

   In der Regel sind Attribute Teil eines Attributsatzes, z. B. ein Satz für Farben mit Attributen für Blau, Grün, Gelb und Rot.

1. Für **[!UICONTROL Type]**, wählen Sie den Typ des Attributwerts aus, z. B. Text und Zahlen.

   Diese Option wirkt sich auf den zulässigen Wert für das Attribut aus.

1. Für **[!UICONTROL Use for Promo Rule Conditions]**, auf `Yes` , damit das -Attribut für einen Parameter in Ihren Werbebedingungen verfügbar ist.

1. Für **[!UICONTROL Used in Search]**, auf `Yes` , wenn das Attribut und der Wert in Produktsuchen verwendet werden können.

1. Für **[!UICONTROL Comparable on Storefront]**, auf `Yes` , wenn der Attributwert in der Amazon-Funktion &quot;Vergleichen nach&quot;verwendet werden kann.

1. Wählen Sie die [!DNL Commerce] [Umfang](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) und wählen Sie eine oder mehrere Store-Ansichten aus, in die Amazon-Werte importiert werden sollen.

   Wenn der Umfang auf `Global`, die _[!UICONTROL Store View]_kann nach der Erstellung des Attributs nicht mehr geändert werden.

   Wenn Sie `All Store Views (Global)`, synchronisiert und speichert Werte für alle Ihre Amazon Store-Ansichten. Sie können Werte nur mit bestimmten Store-Ansichten synchronisieren.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save Attribute Settings]**.

Nach dem Speichern können Sie das Attribut bearbeiten, um die Einstellungen zu überprüfen und Amazon und [!DNL Commerce] -Werte für das -Attribut. Sie können auch angeben, ob Amazon-Werte überschreiben sollen [!DNL Commerce] -Werte.

![Erstellen von Attributeinstellungen](assets/amazon-attribute-settings-create.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Gibt an, ob dieses Attribut live ist und aktiv zwischen Amazon und synchronisiert wird [!DNL Commerce]. Legen Sie `Yes` um die Attributwerte aus Amazon sicherzustellen und [!DNL Commerce] bleiben für das ausgewählte Attribut synchron. |
| Magento Product Attribute auswählen | Gibt das ausgewählte Attribut an, das mit dem aufgelisteten Amazon-Attributnamen verknüpft werden soll. Wählen Sie beim Erstellen eines Attributs `Create New Magento Attribute`. |
| [!UICONTROL Amazon Attribute Name] | Zeigt den Namen des von Ihnen gewählten Amazon-Attributs an. Das ausgewählte Attribut ist mit diesem Amazon-Attribut verknüpft. Sie können diesen Wert nicht bearbeiten über [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | Gibt den Attributnamen oder die Bezeichnung an. |
| [!UICONTROL Magento Product Attribute Code] | Gibt den Attributcode an, alle in Kleinbuchstaben ohne Leerzeichen. |
| [!UICONTROL Attribute Set Ids] | Gibt den Attributsatz an, dem das Attribut zugewiesen werden soll. Attribute sind in der Regel Teil eines Attributsatzes, z. B. eines Farbsatzes mit Attributen für Blau, Grün, Gelb und Rot. |
| [!UICONTROL Type] | Gibt den Werttyp des Attributwerts an, z. B. Text und Zahlen. Die Auswahl wirkt sich auf den zulässigen Wert für das Attribut aus. |
| [!UICONTROL Use for Promo Rule Conditions] | Umschalten auf `Yes` , damit das -Attribut für einen Parameter in Ihren Werbebedingungen verfügbar ist. |
| [!UICONTROL Used in Search] | Gibt an, ob das Attribut und der Wert bei Produktsuchen verwendet werden können. |
| [!UICONTROL Comparable on Storefront] | Gibt an, ob der Attributwert in der Amazon-Funktion &quot;Vergleichen nach&quot;verwendet werden kann. |
| [!UICONTROL Magento Product Attribute Scope] | Gibt die [Umfang](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) für das -Attribut. Optionen: Globale/Store-Ansicht<br>Wenn festgelegt auf `Global`festgelegt ist, kann die Store-Ansicht nach der Erstellung des Attributs nicht mehr bearbeitet werden. |
| [!UICONTROL Store Views (to import values into to)] | Wird nur angezeigt, wenn der Umfang auf `Store View`. Wählen Sie die [Store-Ansicht](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) an die die Amazon-Attributwerte synchronisiert werden. Auswahl `All Store Views (Global)` aktualisiert den Wert über alle [!DNL Commerce] Store-Ansichten. |

## Attribut bearbeiten {#edit-an-attribute}

1. Im _Admin_ Seitenleiste, navigieren Sie zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicks **[!UICONTROL Attributes]** Suchen Sie im Menü links nach einem Amazon-Attribut und klicken Sie auf **[!UICONTROL Edit]** im _[!UICONTROL Action]_Spalte.

1. So aktivieren oder deaktivieren Sie die Synchronisierung der Amazon-Werte mit der verknüpften [!DNL Commerce] Attribut festlegen **Ist aktiv** nach `Yes` oder `No`.

   Wenn festgelegt auf `Yes`, werden die Werte gemäß Ihrer Konfiguration synchronisiert.

1. Für **[!UICONTROL Select Magento Product Attribute]**, überprüfen oder aktualisieren Sie das Attribut, das der ausgewählten **[!UICONTROL Amazon Attribute Name]**.

1. Geben Sie an, ob der eingehende Amazon-Attributwert den vorhandenen Attributwert überschreiben soll.

   Sie möchten beispielsweise die Preise von Amazon nicht in überschreiben. [!DNL Commerce].

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - Behält den Wert bei, wobei unterschiedliche Werte für Ihre [!DNL Commerce] und Amazon Stores.

   - **[!UICONTROL Overwrite Existing Magento Values]** - Überschreibt den Wert im [!DNL Commerce] Produktkatalog mit dem eingehenden Amazon-Wert.

1. Wählen Sie eine oder mehrere aus, falls sie zur Bearbeitung verfügbar sind. **[!UICONTROL Store Views (to import Amazon values into)]**.

   Wenn das Attribut mit einer `Global` Umfang, _Store-Ansicht_ kann nach der Erstellung des Attributs nicht mehr geändert werden.

   Wenn Sie `All Store Views (Global)`, synchronisiert und speichert Werte für alle Store-Ansichten. Sie können Werte nur mit bestimmten Store-Ansichten synchronisieren.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save Attribute Settings]**.

![Attributeinstellungen bearbeiten](assets/amazon-attribute-settings-edit.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Gibt an, ob dieses Attribut live ist und aktiv zwischen Amazon und synchronisiert wird [!DNL Commerce]. Legen Sie `Yes` um die Attributwerte aus Amazon sicherzustellen und [!DNL Commerce] bleiben für das ausgewählte Attribut synchron. |
| [!UICONTROL Select Magento Product Attribute] | Gibt die ausgewählte [!DNL Commerce] -Attribut, das Sie mit dem aufgelisteten Amazon-Attributnamen verknüpfen möchten. Wenn Sie den Link ändern möchten [!DNL Commerce] ein anderes Attribut aus der Dropdown-Liste auswählen. Die Werte werden entsprechend den Konfigurationen synchronisiert. |
| [!UICONTROL Amazon Attribute Name] | Zeigt den Namen des Amazon-Attributs an, wie in [!DNL Amazon Seller Central]. Die ausgewählte [!DNL Commerce] -Attribut verknüpft. Sie können diesen Wert nicht bearbeiten über [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | Gibt an, ob die Amazon-Attributwerte vorhandene Werte überschreiben [!DNL Commerce] Werte, die alle Produkte mit diesem betreffen [!DNL Commerce] -Attribut.<ul><li>**Vorhandene Magento-Werte nicht überschreiben** - (Standard) Behält die [!DNL Commerce] Wert, wobei unterschiedliche Werte für [!DNL Commerce] und Amazon Stores.</li><li>**Vorhandene Magento-Werte überschreiben** - Speichert den Amazon -Wert über dem [!DNL Commerce] Wert in [!DNL Commerce] Produktkatalog.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | Wird beim Bearbeiten eines Attributs nicht angezeigt, wenn das Attribut mit der Variablen `Global` Umfang. Gibt an, dass die Variable [!DNL Commerce] [Umfang](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) wurde erstellt und auf `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | Wählen Sie [!DNL Commerce] [Store-Ansicht](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) an die die Amazon-Attributwerte synchronisiert werden sollen. Auswahl `All Store Views (Global)` aktualisiert den Wert über alle Store-Ansichten hinweg. |
