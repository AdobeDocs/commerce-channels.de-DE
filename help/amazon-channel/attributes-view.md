---
title: Attribute
description: Amazon Sales Channel bietet [!UICONTROL Attributes] , um die Liste von Amazon- und Commerce-Attributen und deren Zuordnung zu Produkten zu überwachen.
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Attribute

Die _[!UICONTROL Attributes]_Ansicht zeigt Ihre Liste von Amazon und [!DNL Commerce] Attribute. Die Liste zeigt auch Attribute an, die für die Produktübereinstimmung zugeordnet wurden. Weitere Informationen finden Sie unter [Attribute verwalten](./managing-attributes.md).

![Attributes-Ansicht](assets/amazon-attributes-view.png)

Von _[!UICONTROL Attributes]_Ansicht, Sie und überprüfen Sie Ihre Attributeinstellungen in der Tabelle und [erstellen oder bearbeiten](./creating-attributes.md) ein Attribut.

## Liste der Attribute Ansicht

1. Auf _Admin_ Sidebar, Gehe zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klick **[!UICONTROL Attributes]** im linken Menü ein Amazon-Attribut suchen und die Liste Ihrer Attribute überprüfen.

1. Erstellen oder bearbeiten Sie ein Attribut nach Bedarf:

   - nach [erstellen](./creating-attributes.md#create-an-attribute) und legen Sie die entsprechenden Attributwerte für das Attribut fest. Klicken Sie **[!UICONTROL Create]**.

   - Zum Deaktivieren oder [Einstellungen bearbeiten](./creating-attributes.md#edit-an-attribute) oder &quot;Passende Attributwerte für das Attribut&quot;, klicken Sie **[!UICONTROL Edit]**.

      Beim Bearbeiten eines Attributs wird die Attributzuordnung für die Produktzuordnung geändert.

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Country] | Das Land, in dem die Aktivität des Verkaufs definiert wird in  **[!DNL Amazon Marketplace]Land** während [Speicherintegration](./store-integration.md). |
| [!UICONTROL ID] | Generischer Attributwert erstellt von [!DNL Commerce] wenn das Attribut erstellt wird. |
| [!UICONTROL Amazon Attribute Name] | Der Name des aus Amazon importierten Attributs. |
| [!UICONTROL Product Catalog Attribute Code] | Wenn zugeordnet, wird die [!DNL Commerce] Attribut, das der Zuordnung zu _[!UICONTROL Amazon Attribute Name]_für übereinstimmende Katalog- und Produktauflistungen. |
| [!UICONTROL Overwrite Magento Values] | Wenn das Attribut auf `Overwrite Existing Magento Values` in den Attributeinstellungen zeigt die Tabelle `Enabled`. &quot;Aktiviert&quot;bedeutet, dass bei Erhalt aktualisierter Produktinformationen für das Attribut von Amazon die neuen Informationen die entsprechenden Informationen für das Produkt in Ihrem [!DNL Commerce] Katalog. Es kann sich auch auf Ihre Produkte auswirken, die in Ihren [!DNL Commerce] Geschäfte. |
| Status | Gibt an, ob die Attributwerte in importiert wurden [!DNL Commerce] und einem [!DNL Commerce] Attribut. Optionen: `Enabled` / `Disabled` |
| Aktion | Gibt die für das Attribut verfügbaren Optionen für die Aufgabe an. Optionen: `Create` / `Edit` |
