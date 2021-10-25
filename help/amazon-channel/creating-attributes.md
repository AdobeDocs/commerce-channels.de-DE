---
title: Attribute erstellen und bearbeiten
description: Amazon Sales Channel bietet die Attributes-Ansicht, mit der Sie die aktuellen Amazon-Attribute und verknüpften Commerce-Attribute überprüfen können.
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Attribute erstellen und bearbeiten

Erstellen oder aktualisieren [!DNL Commerce] -Attribute, während Sie über Amazon verkaufen und Ihre Geschäfte aktualisieren. Aktuelle Amazon-Attribute und verknüpfte Elemente überprüfen [!DNL Commerce] Attribute durch [_[!UICONTROL Attributes]_Ansicht](./attributes-view.md) der Amazon Sales Kanal Startseite. Die_[!UICONTROL Action]_ zeigt die verfügbaren Aktionen für das Attribut an. Sie können entweder eine neue erstellen und zuordnen [!DNL Commerce] Attribut für ein nicht verknüpftes Amazon-Attribut oder Sie können ein vorhandenes Attribut bearbeiten [!DNL Commerce] -Attribut und dessen Zuordnung zu einem Amazon-Attribut.

Wenn Sie Attribute erstellen und aktualisieren, sollten Sie die Attributwerte überprüfen für [!DNL Commerce] und Amazon. Diese Werte können sich unterscheiden, wenn Sie keine Werte aus Amazon synchronisieren und importieren. Informationen zum Überprüfen der Amazon-Werte für diese Attribute finden Sie unter [Amazon-Attributzuordnung überprüfen](./amazon-matching-attributes-values.md). Wenn Sie diese Werte ändern möchten, können Sie [Zuordnungen bearbeiten oder erstellen](./amazon-manually-update-incomplete-listing.md) zwischen Amazon und [!DNL Commerce].

## Attribut erstellen {#create-an-attribute}

Diese Schritte erstellen eine [!DNL Commerce] -Attribut und zuordnen Sie es einem Amazon-Attribut zu. Abhängig von den Konfigurationen können die Werte die Synchronisierung zwischen den Katalogen Beginn haben.

1. Auf _Admin_ Sidebar, Gehe zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klick **[!UICONTROL Attributes]** im linken Menü ein Amazon-Attribut suchen und **[!UICONTROL Create Attribute]** in _[!UICONTROL Action]_Spalte.

1. So aktivieren Sie die Synchronisierung der Amazon-Werte mit den verknüpften [!DNL Commerce] Attribut, Satz **[!UICONTROL Is Active]** nach `Yes`.

   Wenn festgelegt auf `Yes`, werden die Werte entsprechend Ihrer Konfiguration synchronisiert.

1. Auswählen `Create New Magento Attribute` für **[!UICONTROL Select Magento Product Attribute]**.

   Das Attribut wird dem ausgewählten Attribut zugeordnet für **[!UICONTROL Amazon Attribute Name]**.

1. Geben Sie ein **[!UICONTROL Magento Product Attribute Name]**.

1. Geben Sie ein **[!UICONTROL Magento Product Attribute Code]**.

   Dieser Wert muss in Kleinbuchstaben ohne Leerzeichen angegeben werden.

1. für **[!UICONTROL Attribute Set Ids]**, wählen Sie einen Attributsatz, der zugewiesen werden soll.

   In der Regel sind Attribute Teil eines Attributsatzes, z. B. ein Farbsatz mit Attributen für Blau, Grün, Gelb und Rot.

1. für **[!UICONTROL Type]**, wählen Sie den Typ des Attributwerts aus, z. B. Text und Zahlen.

   Diese Option wirkt sich auf den zulässigen Wert des Attributs aus.

1. für **[!UICONTROL Use for Promo Rule Conditions]**, eingestellt auf `Yes` , damit das Attribut für einen Parameter innerhalb Ihrer Werbebedingungen verfügbar ist.

1. für **[!UICONTROL Used in Search]**, eingestellt auf `Yes` , wenn Attribut und Wert bei Produktsuchen verwendet werden können.

1. für **[!UICONTROL Comparable on Storefront]**, eingestellt auf `Yes` wenn der Attributwert in der Amazon-Funktion &quot;Vergleichen mit&quot; verwendet werden kann.

1. Wählen Sie [!DNL Commerce] [Anwendungsbereich](https://docs.magento.com/user-guide/configuration/scope.html){Zielgruppe=&quot;_blank&quot;} für das Attribut und wählen Sie dann eine oder mehrere Store-Ansichten aus, in die Amazon-Werte importiert werden sollen.

   Wenn der Anwendungsbereich auf `Global`, _[!UICONTROL Store View]_kann nicht geändert werden, nachdem das Attribut erstellt wurde.

   Wählen Sie `All Store Views (Global)`, synchronisiert und speichert Werte für alle Amazon Store-Ansichten. Sie können die Werte nur mit bestimmten Store-Ansichten synchronisieren.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save Attribute Settings]**.

Nach dem Speichern können Sie das Attribut bearbeiten, um die Einstellungen zu überprüfen und die Übereinstimmung mit Amazon und [!DNL Commerce] Werte für das Attribut. Sie können auch angeben, ob Amazon-Werte überschrieben werden sollen [!DNL Commerce] Werte.

![Attributeinstellungen erstellen](assets/amazon-attribute-settings-create.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Is Active] | Gibt an, ob dieses Attribut live ist und zwischen Amazon und aktiv synchronisiert wird [!DNL Commerce]. Festlegen auf `Yes` um die Attributwerte von Amazon und [!DNL Commerce] für das ausgewählte Attribut synchron bleiben. |
| Magento-Produktattribut auswählen | Gibt das ausgewählte Attribut an, das mit dem aufgelisteten Amazon-Attributnamen verknüpft werden soll. Wählen Sie beim Erstellen eines Attributs `Create New Magento Attribute`. |
| [!UICONTROL Amazon Attribute Name] | Zeigt den Namen des ausgewählten Amazon-Attributs an. Das ausgewählte Attribut ist mit diesem Amazon-Attribut verknüpft. Sie können diesen Wert nicht bearbeiten über [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | Gibt den Attributnamen oder die Bezeichnung an. |
| [!UICONTROL Magento Product Attribute Code] | Gibt den Attributcode in Kleinbuchstaben ohne Leerzeichen an. |
| [!UICONTROL Attribute Set Ids] | Gibt den Attributsatz an, dem das Attribut zugewiesen werden soll. Attribute sind in der Regel Teil eines Attributsatzes, z. B. eines Farbsatzes mit Attributen für Blau, Grün, Gelb und Rot. |
| [!UICONTROL Type] | Gibt den Werttyp des Attributwerts an, z. B. Text und Zahlen. Die Auswahl wirkt sich auf den zulässigen Wert des Attributs aus. |
| [!UICONTROL Use for Promo Rule Conditions] | Wechseln zu `Yes` , damit das Attribut für einen Parameter innerhalb Ihrer Werbebedingungen verfügbar ist. |
| [!UICONTROL Used in Search] | Gibt an, ob das Attribut und der Wert bei Produktsuchen verwendet werden können. |
| [!UICONTROL Comparable on Storefront] | Gibt an, ob der Attributwert in der Amazon-Funktion &quot;Vergleichen mit&quot; verwendet werden kann. |
| [!UICONTROL Magento Product Attribute Scope] | Kennzeichnet die [Anwendungsbereich](https://docs.magento.com/user-guide/configuration/scope.html){Zielgruppe=&quot;_blank&quot;} für das Attribut. Optionen: Globale/Store-Ansicht<br>Wenn festgelegt auf `Global`, kann die Store-Ansicht nicht bearbeitet werden, nachdem das Attribut erstellt wurde. |
| [!UICONTROL Store Views (to import values into to)] | Wird nur angezeigt, wenn Gültigkeitsbereich auf `Store View`. Wählen Sie [Ansicht speichern](https://docs.magento.com/user-guide/stores/websites-stores-views.html){Zielgruppe=&quot;_blank&quot;}, mit der die Amazon-Attributwerte synchronisiert werden. Auswahl `All Store Views (Global)` aktualisiert den Wert für alle [!DNL Commerce] Ansichten speichern. |

## Attribut bearbeiten {#edit-an-attribute}

1. Auf _Admin_ Sidebar, Gehe zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klick **[!UICONTROL Attributes]** im linken Menü ein Amazon-Attribut suchen und **[!UICONTROL Edit]** in _[!UICONTROL Action]_Spalte.

1. So aktivieren oder deaktivieren Sie die Synchronisierung der Amazon-Werte mit den verknüpften [!DNL Commerce] Attribut, Satz **Ist aktiv** nach `Yes` oder `No`.

   Wenn festgelegt auf `Yes`, werden die Werte entsprechend Ihrer Konfiguration synchronisiert.

1. für **[!UICONTROL Select Magento Product Attribute]**, überprüfen oder aktualisieren Sie das Attribut, das den ausgewählten zugeordnet werden soll **[!UICONTROL Amazon Attribute Name]**.

1. Geben Sie an, ob der eingehende Amazon-Attributwert den vorhandenen Attributwert überschreiben soll.

   Sie möchten z. B. die Preise von Amazon nicht überschreiben in [!DNL Commerce].

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - Behält den Wert bei und behält dabei unterschiedliche Werte für [!DNL Commerce] und Amazon.

   - **[!UICONTROL Overwrite Existing Magento Values]** - Überschreibt den Wert in [!DNL Commerce] Produktkatalog mit dem eingehenden Amazon-Wert.

1. Wenn zur Bearbeitung verfügbar, wählen Sie eine oder mehrere **[!UICONTROL Store Views (to import Amazon values into)]**.

   Wenn das Attribut mit einem `Global` der _Ansicht speichern_ kann nicht geändert werden, nachdem das Attribut erstellt wurde.

   Wählen Sie `All Store Views (Global)`, synchronisiert und speichert Werte in allen Speicher-Ansichten. Sie können die Werte nur mit bestimmten Store-Ansichten synchronisieren.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save Attribute Settings]**.

![Attributeinstellungen bearbeiten](assets/amazon-attribute-settings-edit.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Is Active] | Gibt an, ob dieses Attribut live ist und zwischen Amazon und aktiv synchronisiert wird [!DNL Commerce]. Festlegen auf `Yes` um die Attributwerte von Amazon und [!DNL Commerce] für das ausgewählte Attribut synchron bleiben. |
| [!UICONTROL Select Magento Product Attribute] | Kennzeichnet die ausgewählte [!DNL Commerce] Attribut, das mit dem aufgelisteten Amazon-Attributnamen verknüpft werden soll. Wenn Sie den Link ändern möchten [!DNL Commerce] -Attribut ein anderes Attribut aus der Dropdown-Liste auswählen. Werte werden gemäß Konfigurationen synchronisiert. |
| [!UICONTROL Amazon Attribute Name] | Zeigt den Namen des Amazon-Attributs an, wie in [!DNL Amazon Seller Central]. Die ausgewählten [!DNL Commerce] -Attribut-Links zu diesem Amazon-Attribut. Sie können diesen Wert nicht bearbeiten über [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | Gibt an, ob die Amazon-Attributwerte vorhandene Werte überschreiben [!DNL Commerce] Werte, die sich auf alle Produkte mit dieser [!DNL Commerce] Attribut.<ul><li>**Vorhandene Magento-Werte nicht überschreiben** - (Standard) Behält die [!DNL Commerce] Wert, wobei unterschiedliche Werte für [!DNL Commerce] und Amazon.</li><li>**Vorhandene Magento-Werte überschreiben** - Speichert den Amazon-Wert über [!DNL Commerce] Wert in [!DNL Commerce] Produktkatalog.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | Wird nicht angezeigt, wenn ein Attribut bearbeitet wurde, wenn das Attribut mit der `Global` Anwendungsbereich. Kennzeichnet die [!DNL Commerce] [Anwendungsbereich](https://docs.magento.com/user-guide/configuration/scope.html){Zielgruppe=&quot;_blank&quot;} wurde erstellt und auf `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | Wählen Sie [!DNL Commerce] [Ansicht speichern](https://docs.magento.com/user-guide/stores/websites-stores-views.html){Zielgruppe=&quot;_blank&quot;}, mit der die Amazon-Attributwerte synchronisiert werden sollen. Auswahl `All Store Views (Global)` aktualisiert den Wert in allen Store-Ansichten. |
