---
title: Attribute
description: Amazon Sales Channel bietet die Registerkarte [!UICONTROL Attributes] , um die Liste der Amazon- und Commerce-Attribute und ihre Zuordnung für die Produktabstimmung zu überwachen.
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Attribute

Die _[!UICONTROL Attributes]_-Ansicht zeigt Ihre Liste der Amazon- und [!DNL Commerce]-Attribute an. Die Liste zeigt auch Attribute an, die für die Produktzuordnung zugeordnet wurden. Weitere Informationen finden Sie unter [Attribute verwalten](./managing-attributes.md).

![Attributansicht](assets/amazon-attributes-view.png)

In der _[!UICONTROL Attributes]_-Ansicht können Sie Ihre Attributeinstellungen in der Tabelle überprüfen und [ein Attribut erstellen oder bearbeiten](./creating-attributes.md).

## Anzeigen der Attributliste

1. Gehen Sie in der Seitenleiste _Admin_ zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicken Sie im Menü links auf **[!UICONTROL Attributes]**, suchen Sie ein Amazon-Attribut und überprüfen Sie Ihre Attributliste.

1. Erstellen oder bearbeiten Sie nach Bedarf ein Attribut:

   - Um [create](./creating-attributes.md#create-an-attribute) und define Matching Attribute Values for the attribute zu erstellen, klicken Sie auf **[!UICONTROL Create]**.

   - Um die Einstellungen ](./creating-attributes.md#edit-an-attribute) oder [zu deaktivieren oder zu bearbeiten, klicken Sie auf **[!UICONTROL Edit]**, um die Attributwerte abzugleichen.

      Das Bearbeiten eines Attributs umfasst das Ändern der Attributzuordnung für die Produktzuordnung.

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Country] | Das Land für die Verkaufsaktivität, definiert in **[!DNL Amazon Marketplace]Land** während der [Store-Integration](./store-integration.md). |
| [!UICONTROL ID] | Generischer Attributwert, der von [!DNL Commerce] bei der Erstellung des Attributs generiert wird. |
| [!UICONTROL Amazon Attribute Name] | Der Name des aus Amazon importierten Attributs. |
| [!UICONTROL Product Catalog Attribute Code] | Wenn das Attribut [!DNL Commerce] zugeordnet ist, wird es dem _[!UICONTROL Amazon Attribute Name]_für den entsprechenden Katalog und die Liste der Produkte zugeordnet. |
| [!UICONTROL Overwrite Magento Values] | Wenn das Attribut in den Attributeinstellungen auf `Overwrite Existing Magento Values` festgelegt ist, zeigt die Tabelle `Enabled` an. Aktiviert bedeutet, dass bei aktualisierten Produktinformationen für das Attribut von Amazon die neuen Informationen die entsprechenden Informationen für das Produkt in Ihrem [!DNL Commerce]-Katalog aktualisiert (überschrieben) werden. Sie kann sich auch auf Ihre Produkte auswirken, die in Ihren [!DNL Commerce] Stores aufgeführt sind. |
| Status | Gibt an, ob die Attributwerte in [!DNL Commerce] importiert und einem [!DNL Commerce] -Attribut zugeordnet wurden. Optionen: `Enabled` / `Disabled` |
| Aktion | Gibt die für das Attribut verfügbaren Aufgabenoptionen an. Optionen: `Create` / `Edit` |
