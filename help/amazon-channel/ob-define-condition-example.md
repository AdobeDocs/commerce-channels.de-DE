---
title: "Beispiel: Bedingung für Amazon-Listening-Regeln definieren"
description: Definieren Sie beim Erstellen Ihrer Listening-Regeln Bedingungen zur Identifizierung der Commerce-Katalogprodukte, die auf dem Amazon Marketplace aufgeführt werden sollen.
feature: Sales Channels, Products, Configuration
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Beispiel: Bedingung definieren

## Bedingungen

Auf alle Bereiche in den fett gedruckten Bedingungen kann geklickt werden, um die verschiedenen Optionen anzuzeigen.

**Fügen Sie keine Bedingungen hinzu, wenn alle Produkte auf der ausgewählten Website förderfähig sind.**

>[!NOTE]
>
>Es gibt eine komplexe Reihe von Back-End-Prozessen, die direkt mit den Systemen von Amazon kommunizieren. Je nachdem, wie viele Elemente Sie auflisten möchten und wie beschäftigt die Amazon-Systeme sein könnten (z. B. Black Friday), kann es einige Zeit dauern, bis Ihre Artikel in Amazon aufgelistet werden.

Siehe den Abschnitt &quot;Bedingungen&quot;von [Erstellen einer Warenkorbpreisregel](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog-create.html).

## Bedingung definieren

Dieser Vorgang kann je nach Katalogeinrichtung einfach oder detailliert sein. Sie können Ihre Bedingungen so einrichten, dass das Produkt in Amazon aufgeführt werden kann, wenn `ALL` oder `ANY` der definierten Bedingungen für ein Produkt entweder `TRUE` oder `FALSE` sind.

Bedingungen basieren auf vorhandenen Produktattributwerten. Lassen Sie den Abschnitt Bedingungen leer, um die Regel auf alle Produkte anzuwenden.

>[!NOTE]
>
>Wenn Sie eine Bedingung basierend auf einem bestimmten Produktattribut definieren möchten, setzen Sie die Einstellung **[!UICONTROL Use for Promo Rule Conditions]** für das Attribut auf `Yes`. Sie können auf diese Einstellung auf der Seite [Storefront-Eigenschaften](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes-add.html) für das Attribut zugreifen.

![Bedingung - Zeile 1](assets/ob-listing-rule-conditions-start.png){width="500"}

Die Regel in diesem Beispiel definiert eine Regel, die die Amazon-Eignung für alle Katalogprodukte festlegt, für die das Attribut _Amazon FBA_ auf `Yes` gesetzt ist.

Die Regelanweisung enthält zwei fette Links, die beim Klicken die Optionen für diesen Teil der Anweisung anzeigen. Wenn Sie die Bedingung speichern, ohne eine fett gedruckte Option zu ändern, gilt die Regel für alle Ihre Produkte.

- Klicken Sie auf **[!UICONTROL ALL]** und wählen Sie entweder `ALL` oder `ANY` aus.
- Klicken Sie auf **[!UICONTROL TRUE]** und wählen Sie entweder `TRUE` oder `FALSE` aus.
- Um die Regel auf alle Produkte anzuwenden, lassen Sie die Bedingung unverändert.

Sie können unterschiedliche Bedingungen erstellen, indem Sie die Kombination dieser Werte ändern. Für dieses Beispiel wird die folgende Bedingung verwendet:

`If ALL of these conditions are TRUE:`

1. Klicken Sie am Anfang der Bedingungszeile auf das Symbol Hinzufügen (![Symbol hinzufügen](assets/btn-add-grn.png)) und wählen Sie ein Attribut aus, auf dem die Bedingung basieren soll, z. B. eine Bedingungskombination oder ein Produktattribut.

   - **[!UICONTROL Conditions Combination]** - Ermöglicht es Ihnen, einen weiteren Satz von `All/Any` und `True/False` Bedingungen innerhalb des vorhandenen Satzes zu erstellen.

     ![Bedingungskombination](assets/ob-conditions-combinations.png){width="500"}

   - **[!UICONTROL Product Attribute]** - Die Produktattribute hängen von der Einrichtung des Attributs ab. Damit ein Attribut in der Liste angezeigt wird, muss es für die Verwendung in Bedingungen für Werberegeln konfiguriert werden. Siehe _Für Angebotsregelbedingungen verwenden_ in [Produktattributen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

     Wählen Sie in der Liste unter **[!UICONTROL Product Attribute]** das Attribut aus, das Sie als Grundlage für die Bedingung verwenden möchten. In diesem Beispiel ist die ausgewählte Bedingung `Amazon FBA`.

     ![Bedingungszeile 2, Teil 2](assets/ob-condition-attribute-dropdown.png){width="350"}

     Die ausgewählte Bedingung wird in der Anweisung angezeigt, gefolgt von zwei weiteren fett gedruckten Links. Die Optionen variieren je nach ausgewähltem Produktattribut.

     Nachdem Sie das Attribut festgelegt haben, kann es nicht mehr geändert werden. Um das Attribut zu ändern, müssen Sie die Zeile löschen und das neue Attribut hinzufügen. Sie können eine Bedingungszeile löschen, indem Sie am Ende der Zeile auf das Symbol Löschen (![Löschsymbol](assets/btn-del-red.png)) klicken.

      1. Klicken Sie auf **[!UICONTROL is]** und wählen Sie den Vergleichsoperator aus, der die Bedingung für die zu erfüllenden Produkte beschreibt.

         In diesem Beispiel ist der Vergleichsoperator `is`. Die verfügbaren Optionen hängen vom im vorherigen Schritt ausgewählten Attribut ab. Optionen können verschiedene Vergleichsoptionen umfassen, z. B. übereinstimmende Werte, die mindestens einen Wert nicht enthalten oder darunter stehen, sowie größer, gleich und kleiner als ein numerischer Wert. In diesem Beispiel sind die Optionen `is` und `is not`.

      1. Klicken Sie auf **[!UICONTROL ...]** und wählen Sie den Attributwert aus, auf dem die Bedingung basiert.

         Die Optionen hängen von der Einrichtung des Attributs ab. Sie werden möglicherweise aufgefordert, eine Option auszuwählen oder Text- oder Zahlenwerte für die Bedingung einzugeben. In diesem Beispiel ist die Auswahl `Yes`.

         Das ausgewählte Element wird in der Anweisung angezeigt, um die Bedingung abzuschließen.

         ![Bedingungszeile 2, Teil 3](assets/ob-listing-rule-condition-is.png){width="500"}

   Diese Bedingung ist abgeschlossen. Wie angegeben bedeutet diese Bedingung, dass jedes Produkt in Ihrem [!DNL Commerce]-Katalog, für das das Amazon FBA-Attribut auf den Wert `Yes` gesetzt ist, für die Auflistung der Region und des Stores an Amazon berechtigt ist. Sie können weitere Bedingungszeilen hinzufügen, um Ihre infrage kommenden Produkte weiter einzuschränken.

1. Um der Anweisung eine weitere Bedingungszeile hinzuzufügen, kehren Sie zu Schritt 1 zurück und wiederholen Sie den Prozess, bis alle gewünschten Bedingungen abgeschlossen sind.

Sie können eine Zeile der Bedingungsanweisung jederzeit löschen, indem Sie am Ende der Zeile auf das Symbol Löschen (![Löschsymbol](assets/btn-del-red.png)) klicken.
