---
title: Attribute für Amazon-Listen
description: Amazon Sales Channel stellt die [!UICONTROL Attributes] um die Liste der Amazon- und Commerce-Attribute und ihre Zuordnung für die Produktzuordnung zu überwachen.
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Attribute für Amazon-Listen

Die _[!UICONTROL Attributes]_zeigt Ihre Liste von Amazon und [!DNL Commerce] -Attribute. Die Liste zeigt auch Attribute an, die für die Produktzuordnung zugeordnet wurden. Weitere Informationen finden Sie unter [Attribute verwalten](./managing-attributes.md).

![Attributansicht](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

Aus dem _[!UICONTROL Attributes]_anzeigen, Sie anzeigen und Ihre Attributeinstellungen in der Tabelle überprüfen und [erstellen oder bearbeiten](./creating-attributes.md) ein Attribut.

## Anzeigen der Attributliste

1. Im _Admin_ Seitenleiste, navigieren Sie zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicks **[!UICONTROL Attributes]** Suchen Sie im Menü links ein Amazon-Attribut und überprüfen Sie Ihre Attributliste.

1. Erstellen oder bearbeiten Sie nach Bedarf ein Attribut:

   - nach [erstellen](./creating-attributes.md#create-an-attribute) und legen Sie übereinstimmende Attributwerte für das Attribut fest, klicken Sie auf **[!UICONTROL Create]**.

   - So deaktivieren Sie oder [Einstellungen bearbeiten](./creating-attributes.md#edit-an-attribute) oder Abgleichen von Attributwerten für das Attribut klicken Sie auf **[!UICONTROL Edit]**.

     Das Bearbeiten eines Attributs umfasst das Ändern der Attributzuordnung für die Produktzuordnung.

| Feld | Beschreibung |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country] | Das Land, in dem die Verkaufsaktivität definiert wurde in  **[!DNL Amazon Marketplace]Land** during [Store-Integration](./store-integration.md). |
| [!UICONTROL ID] | Generischer Attributwert, generiert von [!DNL Commerce] wenn das Attribut erstellt wird. |
| [!UICONTROL Amazon Attribute Name] | Der Name des aus Amazon importierten Attributs. |
| [!UICONTROL Product Catalog Attribute Code] | Wenn die Variable [!DNL Commerce] -Attribut, das der Zuordnung zum _[!UICONTROL Amazon Attribute Name]_für übereinstimmende Kataloge und Auflistungsprodukte. |
| [!UICONTROL Overwrite Magento Values] | Wenn das Attribut auf `Overwrite Existing Magento Values` in den Attributeinstellungen zeigt die Tabelle `Enabled`. Aktiviert bedeutet, dass bei aktualisierten Produktinformationen für das Attribut von Amazon die neuen Informationen die entsprechenden Informationen für das Produkt in Ihrer [!DNL Commerce] Katalog. Sie kann sich auch auf Ihre Produkte auswirken, die in Ihrer [!DNL Commerce] Stores. |
| Status | Gibt an, ob die Attributwerte in importiert wurden [!DNL Commerce] und einem [!DNL Commerce] -Attribut. Optionen: `Enabled` / `Disabled` |
| Aktion | Gibt die für das Attribut verfügbaren Aufgabenoptionen an. Optionen: `Create` / `Edit` |
