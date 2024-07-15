---
title: Erstellen und Bearbeiten von Attributen für den Amazon-Vertriebskanal
description: Amazon Sales Channel bietet die Ansicht "Attributes", mit der Sie die aktuellen Amazon-Attribute und verknüpften Commerce-Attribute überprüfen können.
feature: Sales Channels, Products, Configuration
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# Attribute erstellen und bearbeiten

Erstellen oder aktualisieren Sie [!DNL Commerce] -Attribute, während Sie über Amazon verkaufen und Ihre Geschäfte aktualisieren. Überprüfen Sie die aktuellen Amazon-Attribute und verknüpften [!DNL Commerce] -Attribute über die [_[!UICONTROL Attributes]_Ansicht](./attributes-view.md) der Homepage des Amazon-Vertriebskanals. Die Spalte_[!UICONTROL Action]_ enthält die verfügbaren Aktionen für das Attribut. Sie können entweder ein neues [!DNL Commerce] -Attribut für ein nicht verknüpftes Amazon-Attribut erstellen und zuordnen oder ein vorhandenes [!DNL Commerce] -Attribut und dessen Zuordnung zu einem Amazon-Attribut bearbeiten.

Beim Erstellen und Aktualisieren von Attributen sollten Sie die Attributwerte für [!DNL Commerce] und Amazon-Produkte überprüfen. Diese Werte unterscheiden sich möglicherweise, wenn Sie keine Werte aus Amazon synchronisieren und importieren. Informationen zum Überprüfen von Amazon-Werten für diese Attribute finden Sie unter [Überprüfen der Amazon-Attributzuordnung](./amazon-matching-attributes-values.md). Wenn Sie diese Werte ändern möchten, können Sie [die Zuordnung](./amazon-manually-update-incomplete-listing.md) zwischen Amazon und [!DNL Commerce] bearbeiten oder erstellen.

## Attribut erstellen {#create-an-attribute}

Diese Schritte erstellen ein [!DNL Commerce] -Attribut und ordnen es einem Amazon-Attribut zu. Je nach Konfiguration können die Werte mit der Synchronisierung zwischen Katalogen beginnen.

1. Wechseln Sie in der Seitenleiste _Admin_ zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicken Sie im Menü links auf &quot;**[!UICONTROL Attributes]**&quot;, suchen Sie ein Amazon-Attribut und klicken Sie in der Spalte &quot;_[!UICONTROL Action]_&quot;auf &quot;**[!UICONTROL Create Attribute]**&quot;.

1. Um die Synchronisierung der Amazon-Werte mit dem verknüpften Attribut [!DNL Commerce] zu aktivieren, setzen Sie **[!UICONTROL Is Active]** auf `Yes`.

   Wenn der Wert auf `Yes` gesetzt ist, werden die Werte entsprechend Ihrer Konfiguration synchronisiert.

1. Wählen Sie `Create New Magento Attribute` für **[!UICONTROL Select Magento Product Attribute]** aus.

   Das Attribut wird dem für **[!UICONTROL Amazon Attribute Name]** ausgewählten Attribut zugeordnet.

1. Geben Sie einen **[!UICONTROL Magento Product Attribute Name]** ein.

1. Geben Sie einen **[!UICONTROL Magento Product Attribute Code]** ein.

   Dieser Wert muss in Kleinbuchstaben ohne Leerzeichen eingegeben werden.

1. Wählen Sie für &quot;**[!UICONTROL Attribute Set Ids]**&quot;einen Attributsatz, der zugewiesen werden soll.

   In der Regel sind Attribute Teil eines Attributsatzes, z. B. ein Satz für Farben mit Attributen für Blau, Grün, Gelb und Rot.

1. Wählen Sie für **[!UICONTROL Type]** den Typ des Attributwerts aus, z. B. Text und Zahlen.

   Diese Option wirkt sich auf den zulässigen Wert für das Attribut aus.

1. Setzen Sie für **[!UICONTROL Use for Promo Rule Conditions]** den Wert auf `Yes`, damit das Attribut für einen Parameter innerhalb Ihrer Werbebedingungen verfügbar ist.

1. Setzen Sie für &quot;**[!UICONTROL Used in Search]**&quot;auf &quot;`Yes`&quot;, wenn das Attribut und der Wert bei Produktsuchen verwendet werden können.

1. Setzen Sie für **[!UICONTROL Comparable on Storefront]** den Wert auf `Yes` , wenn der Attributwert in der Amazon-Funktion &quot;Vergleichen nach&quot;verwendet werden kann.

1. Wählen Sie den [!DNL Commerce] [Perimeter](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) für das Attribut aus und wählen Sie dann mindestens eine Store-Ansicht aus, in die Amazon-Werte importiert werden sollen.

   Wenn der Umfang auf `Global` festgelegt ist, kann der _[!UICONTROL Store View]_nach der Erstellung des Attributs nicht mehr geändert werden.

   Wenn Sie &quot;`All Store Views (Global)`&quot;auswählen, werden Werte synchronisiert und für alle Amazon Store-Ansichten gespeichert. Sie können Werte nur mit bestimmten Store-Ansichten synchronisieren.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save Attribute Settings]**.

Nach dem Speichern können Sie das Attribut bearbeiten, um die Einstellungen zu überprüfen und die entsprechenden Amazon- und [!DNL Commerce]-Werte für das Attribut zu überprüfen. Sie können auch angeben, ob Amazon-Werte [!DNL Commerce]-Werte überschreiben sollen.

![Attributeinstellungen erstellen](assets/amazon-attribute-settings-create.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Gibt an, ob dieses Attribut live ist und aktiv zwischen Amazon und [!DNL Commerce] synchronisiert wird. Setzen Sie dies auf &quot;`Yes`&quot;, um sicherzustellen, dass die Attributwerte aus Amazon und &quot;[!DNL Commerce]&quot;für das ausgewählte Attribut synchronisiert bleiben. |
| Magento Product Attribute auswählen | Gibt das ausgewählte Attribut an, das mit dem aufgelisteten Amazon-Attributnamen verknüpft werden soll. Wählen Sie beim Erstellen eines Attributs `Create New Magento Attribute` aus. |
| [!UICONTROL Amazon Attribute Name] | Zeigt den Namen des von Ihnen gewählten Amazon-Attributs an. Das ausgewählte Attribut ist mit diesem Amazon-Attribut verknüpft. Sie können diesen Wert nicht über [!DNL Commerce] bearbeiten. |
| [!UICONTROL Magento Product Attribute Name] | Gibt den Attributnamen oder die Bezeichnung an. |
| [!UICONTROL Magento Product Attribute Code] | Gibt den Attributcode an, alle in Kleinbuchstaben ohne Leerzeichen. |
| [!UICONTROL Attribute Set Ids] | Gibt den Attributsatz an, dem das Attribut zugewiesen werden soll. Attribute sind in der Regel Teil eines Attributsatzes, z. B. eines Farbsatzes mit Attributen für Blau, Grün, Gelb und Rot. |
| [!UICONTROL Type] | Gibt den Werttyp des Attributwerts an, z. B. Text und Zahlen. Die Auswahl wirkt sich auf den zulässigen Wert für das Attribut aus. |
| [!UICONTROL Use for Promo Rule Conditions] | Schalten Sie zu `Yes` um, damit das Attribut für einen Parameter innerhalb Ihrer Werbebedingungen verfügbar ist. |
| [!UICONTROL Used in Search] | Gibt an, ob das Attribut und der Wert bei Produktsuchen verwendet werden können. |
| [!UICONTROL Comparable on Storefront] | Gibt an, ob der Attributwert in der Amazon-Funktion &quot;Vergleichen nach&quot;verwendet werden kann. |
| [!UICONTROL Magento Product Attribute Scope] | Gibt den [Gültigkeitsbereich](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) für das Attribut an. Optionen: Globale/Store-Ansicht<br>Wenn auf `Global` festgelegt, kann die Store-Ansicht nach der Erstellung des Attributs nicht mehr bearbeitet werden. |
| [!UICONTROL Store Views (to import values into to)] | Wird nur angezeigt, wenn der Umfang auf `Store View` festgelegt ist. Wählen Sie die [Store-Ansicht](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) aus, mit der die Amazon-Attributwerte synchronisiert werden. Bei Auswahl von `All Store Views (Global)` wird der Wert für alle [!DNL Commerce] Store-Ansichten aktualisiert. |

## Attribut bearbeiten {#edit-an-attribute}

1. Wechseln Sie in der Seitenleiste _Admin_ zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicken Sie im Menü links auf &quot;**[!UICONTROL Attributes]**&quot;, suchen Sie ein Amazon-Attribut und klicken Sie in der Spalte &quot;_[!UICONTROL Action]_&quot;auf &quot;**[!UICONTROL Edit]**&quot;.

1. Um die Synchronisierung der Amazon-Werte mit dem verknüpften Attribut [!DNL Commerce] zu aktivieren bzw. zu deaktivieren, setzen Sie **Is Active** auf `Yes` oder `No`.

   Wenn der Wert auf `Yes` gesetzt ist, werden die Werte entsprechend Ihrer Konfiguration synchronisiert.

1. Überprüfen oder aktualisieren Sie für **[!UICONTROL Select Magento Product Attribute]** das Attribut, das der ausgewählten **[!UICONTROL Amazon Attribute Name]** zugeordnet werden soll.

1. Geben Sie an, ob der eingehende Amazon-Attributwert den vorhandenen Attributwert überschreiben soll.

   So können Sie beispielsweise die Preise von Amazon nicht in [!DNL Commerce] überschreiben.

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - Behält den Wert bei, wobei für Ihre [!DNL Commerce]- und Amazon-Stores unterschiedliche Werte beibehalten werden.

   - **[!UICONTROL Overwrite Existing Magento Values]** - Überschreibt den Wert im Produktkatalog [!DNL Commerce] mit dem eingehenden Amazon-Wert.

1. Wählen Sie mindestens einen **[!UICONTROL Store Views (to import Amazon values into)]** aus, falls er zur Bearbeitung verfügbar ist.

   Wenn das Attribut mit dem Gültigkeitsbereich `Global` erstellt wurde, kann die _Store-Ansicht_ nach der Erstellung des Attributs nicht mehr geändert werden.

   Wenn Sie &quot;`All Store Views (Global)`&quot;auswählen, werden Werte synchronisiert und für alle Store-Ansichten gespeichert. Sie können Werte nur mit bestimmten Store-Ansichten synchronisieren.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save Attribute Settings]**.

![Attributeinstellungen bearbeiten](assets/amazon-attribute-settings-edit.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Gibt an, ob dieses Attribut live ist und aktiv zwischen Amazon und [!DNL Commerce] synchronisiert wird. Setzen Sie dies auf &quot;`Yes`&quot;, um sicherzustellen, dass die Attributwerte aus Amazon und &quot;[!DNL Commerce]&quot;für das ausgewählte Attribut synchronisiert bleiben. |
| [!UICONTROL Select Magento Product Attribute] | Gibt das ausgewählte [!DNL Commerce] -Attribut an, das Sie mit dem aufgelisteten Amazon-Attributnamen verknüpfen möchten. Wenn Sie das verknüpfte Attribut [!DNL Commerce] ändern möchten, wählen Sie ein anderes Attribut aus der Dropdownliste aus. Die Werte werden entsprechend den Konfigurationen synchronisiert. |
| [!UICONTROL Amazon Attribute Name] | Zeigt den Namen des Amazon-Attributs an, wie in [!DNL Amazon Seller Central] definiert. Das ausgewählte Attribut [!DNL Commerce] ist mit diesem Amazon-Attribut verknüpft. Sie können diesen Wert nicht über [!DNL Commerce] bearbeiten. |
| [!UICONTROL Overwrite Existing Value] | Gibt an, ob die Amazon-Attributwerte vorhandene [!DNL Commerce] -Werte überschreiben, was sich auf alle Produkte mit diesem [!DNL Commerce] -Attribut auswirkt.<ul><li>**Vorhandene Magento-Werte nicht überschreiben** - (Standard) Behält den Wert [!DNL Commerce] bei, wobei unterschiedliche Werte für [!DNL Commerce] und Amazon-Stores beibehalten werden.</li><li>**Vorhandene Magento-Werte überschreiben** - Speichert den Amazon-Wert über dem [!DNL Commerce] -Wert im Produktkatalog [!DNL Commerce].</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | Wird beim Bearbeiten eines Attributs nicht angezeigt, wenn das Attribut mit dem Gültigkeitsbereich `Global` erstellt wurde. Gibt an, dass der [!DNL Commerce] [scope](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) erstellt und auf `Store View` festgelegt wurde. |
| [!UICONTROL Store Views (to import values into to)] | Wählen Sie Ihre [!DNL Commerce] [Store-Ansicht](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) aus, mit der die Amazon-Attributwerte synchronisiert werden sollen. Bei Auswahl von `All Store Views (Global)` wird der Wert für alle Store-Ansichten aktualisiert. |
