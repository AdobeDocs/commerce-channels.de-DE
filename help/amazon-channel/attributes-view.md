---
title: Attribute für Amazon-Listen
description: Amazon Sales Channel bietet die Registerkarte "[!UICONTROL Attributes]", um die Liste der Amazon- und Commerce-Attribute und ihre Zuordnung für die Produktzuordnung zu überwachen.
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Attribute für Amazon-Listen

Die _[!UICONTROL Attributes]_-Ansicht zeigt Ihre Liste der Amazon- und [!DNL Commerce]-Attribute an. Die Liste zeigt auch Attribute an, die für die Produktzuordnung zugeordnet wurden. Weitere Informationen finden Sie unter [Attribute verwalten](./managing-attributes.md).

![Attributansicht](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

Überprüfen Sie in der Ansicht &quot;_[!UICONTROL Attributes]_&quot;Ihre Attributeinstellungen in der Tabelle und [erstellen oder bearbeiten](./creating-attributes.md) Sie ein Attribut.

## Anzeigen der Attributliste

1. Wechseln Sie in der Seitenleiste _Admin_ zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicken Sie im Menü links auf &quot;**[!UICONTROL Attributes]**&quot;, suchen Sie ein Amazon-Attribut und überprüfen Sie Ihre Attributliste.

1. Erstellen oder bearbeiten Sie nach Bedarf ein Attribut:

   - Um [create](./creating-attributes.md#create-an-attribute) und Matching Attribute Values für das Attribut zu definieren, klicken Sie auf **[!UICONTROL Create]**.

   - Um die Einstellungen ](./creating-attributes.md#edit-an-attribute) oder Matching Attribute Values für das Attribut zu deaktivieren oder [zu bearbeiten, klicken Sie auf **[!UICONTROL Edit]**.

     Das Bearbeiten eines Attributs umfasst das Ändern der Attributzuordnung für die Produktzuordnung.

| Feld | Beschreibung |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country] | Das Land für die Verkaufsaktivität, das in **[!DNL Amazon Marketplace]Land** während der [Speicherintegration](./store-integration.md) definiert wurde. |
| [!UICONTROL ID] | Generischer Attributwert, der von [!DNL Commerce] bei der Erstellung des Attributs generiert wird. |
| [!UICONTROL Amazon Attribute Name] | Der Name des aus Amazon importierten Attributs. |
| [!UICONTROL Product Catalog Attribute Code] | Wenn das Attribut [!DNL Commerce] zugeordnet ist, wird es dem _[!UICONTROL Amazon Attribute Name]_für den entsprechenden Katalog und die Liste der Produkte zugeordnet. |
| [!UICONTROL Overwrite Magento Values] | Wenn das Attribut in den Attributeinstellungen auf &quot;`Overwrite Existing Magento Values`&quot; gesetzt ist, zeigt die Tabelle &quot;`Enabled`&quot; an. Aktiviert bedeutet, dass bei aktualisierten Produktinformationen für das Attribut von Amazon die neuen Informationen die entsprechenden Informationen für das Produkt in Ihrem [!DNL Commerce] -Katalog aktualisiert (überschrieben) werden. Sie kann sich auch auf Ihre in Ihren [!DNL Commerce] Stores aufgelisteten Produkte auswirken. |
| Status | Gibt an, ob die Attributwerte in [!DNL Commerce] importiert und einem [!DNL Commerce] -Attribut zugeordnet wurden. Optionen: `Enabled` / `Disabled` |
| Aktion | Gibt die für das Attribut verfügbaren Aufgabenoptionen an. Optionen: `Create` / `Edit` |
