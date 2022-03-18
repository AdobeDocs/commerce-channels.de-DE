---
title: Bedingungen für Preisregeln
description: Verwenden Sie die Preisregel-Bedingungen, um zu bestimmen, welche Produkte für die Regel des Listenpreises infrage kommen.
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Bedingungen für Preisregeln

Die Bedingungen bestimmen, welche Produkte für die Preisregel infrage kommen. Die Festlegung der Bedingungen für Ihre Amazon-Preisregeln folgt derselben Logik und demselben Prozess wie die Definition der Bedingungen für [Warenkorbpreisregeln](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;} in [!DNL Commerce].

>[!IMPORTANT]
>
>Wenn Ihre Preisregel für alle Produkte in Ihrer [!DNL Commerce] Katalog erstellen, lassen Sie diesen Abschnitt leer.

Auf alle Bereiche in den fett gedruckten Bedingungen kann geklickt werden, um die verschiedenen Optionen anzuzeigen.

## Beispiel: eine Preisregel-Bedingung erstellen

Dieser Vorgang kann je nach Konfiguration Ihres Katalogs einfach oder detailliert sein. Sie können Bedingungen so definieren, dass `ALL` oder `ANY` der Bedingungen `TRUE` oder `FALSE` für ein Produkt gilt die Preisregel für das Produkt.

Die Bedingungen basieren auf Ihren [Produktattribute](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}. Lassen Sie den Abschnitt Bedingungen leer, um die Regel auf alle Produkte anzuwenden.

>[!NOTE]
>
>Wenn Sie eine Bedingung basierend auf einem bestimmten Produktattribut definieren möchten, **Verwendung für Bedingungen für Angebotsregeln** für muss das Attribut auf `Yes` in [Storefront-Eigenschaften](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;} für das Attribut.

![Bedingung der Preisregel - Zeile 1](assets/ob-price-rules-condition-1.png)

In diesem Beispiel wird eine Regel definiert, die einen Rabatt von 25 % auf alle Produkte anwendet, die in der Variablen `Books` Kategorie.

Die Regelanweisung verfügt über zwei fette Links, die beim Klicken die Optionen für diesen Teil der Bedingungsanweisung anzeigen. Wenn Sie die Bedingung speichern, ohne eine fett gedruckte Option zu ändern, gilt die Regel für alle Ihre Produkte.

- Klicken **[!UICONTROL ALL]** und wählen Sie entweder `ALL` oder `ANY`.
- Klicken **[!UICONTROL TRUE]** und wählen Sie entweder `TRUE` oder `FALSE`.
- Um die Regel auf alle Produkte anzuwenden, lassen Sie die Bedingung unverändert.

Sie können unterschiedliche Bedingungen erstellen, indem Sie die Kombination dieser Werte ändern. Für dieses Beispiel wird die folgende Bedingung verwendet:

`If ALL of these conditions are TRUE:`

1. Klicken Sie auf Hinzufügen (![Symbol hinzufügen](assets/btn-add-grn.png)) am Anfang der Bedingungszeile und wählen Sie ein Attribut aus, auf dem die Bedingung basieren soll.

   **[!UICONTROL Conditions Combination]** - Wählen Sie aus, einen weiteren Satz von `All/Any` und `True/False` Bedingungen innerhalb der vorhandenen Bedingung.

   ![Kombination von Preisregelbedingungen](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]** - Die verfügbaren Produktattribute hängen von der [Einrichtung des Attributs](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}. Damit ein Attribut in der Liste angezeigt wird, *[!UICONTROL Use for Promo Rule Conditions]* für muss das Attribut auf `Yes` in [Storefront-Eigenschaften](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}.

   - Für **[!UICONTROL Product Attribute]**, wählen Sie das Attribut aus, das Sie als Basis der Bedingung definieren möchten. In diesem Beispiel lautet die ausgewählte Bedingung: `Category`.

      ![Bedingung für Preisregel - Zeile 2, Teil 2](assets/ob-price-rule-condition-2.png)

      Die ausgewählte Bedingung wird in der Anweisung angezeigt, gefolgt von zwei weiteren fett gedruckten Links. Die Optionen variieren je nach ausgewähltem Produktattribut.

      Nachdem Sie das Attribut festgelegt haben, kann es nicht mehr bearbeitet werden. Um das Attribut zu ändern, müssen Sie die Zeile löschen und das neue Attribut hinzufügen. Sie können eine Bedingungszeile löschen, indem Sie auf Löschen (![Löschsymbol](assets/btn-del-red.png) -Symbol am Ende der Zeile.

   - Klicken **[!UICONTROL is]** und wählen Sie den Vergleichsoperator aus, der die Bedingung für die zu erfüllenden Produkte beschreibt.

      In diesem Beispiel lautet der Vergleichsoperator `is`. Die verfügbaren Optionen hängen vom im vorherigen Schritt ausgewählten Attribut ab und können verschiedene Vergleichsoptionen enthalten. Optionen können übereinstimmende Werte umfassen, die mindestens einen Wert nicht enthalten oder darunter fallen, sowie größer, gleich und kleiner als ein numerischer Wert. In diesem Beispiel sind die Optionen `is` und `is not`.

   - Klicken **[!UICONTROL ...]** und wählen Sie den Attributwert aus, auf dem die Bedingung basiert. Die Optionen hängen von der Einrichtung des Attributs ab.

      Sie werden möglicherweise aufgefordert, eine Option auszuwählen oder einen Wert für die Bedingung einzugeben. In diesem Beispiel wird das Feld leer angezeigt. Klicken Sie auf das Auswahlsymbol (![Auswahlsymbol](assets/btn-chooser.png)), um Ihre Auswahloptionen anzuzeigen. Diese Regel gilt für _Bücher_, wählen Sie die **[!UICONTROL Books]** aktivieren. Die Kategorienummer wird ausgefüllt. Um Ihre Kategorieauswahlen zu akzeptieren, klicken Sie auf das grüne Häkchensymbol (![Symbol &quot;Häkchen&quot;](assets/btn-check-mark-green.png)).

      ![Bedingung für Preisregel - Zeile 2, Teil 3](assets/ob-price-rule-condition-3.png)

      Das ausgewählte Element wird in der Anweisung angezeigt, um die Bedingung abzuschließen.

      ![Bedingung für Preisregel - Zeile 2, Teil 4](assets/ob-price-rule-condition-4.png)

      Diese Beispielbedingung ist abgeschlossen. Wie angegeben bedeutet diese Bedingung, dass jedes Produkt in Ihrer [!DNL Commerce] Katalog mit einer definierten Kategorie von Büchern (`4`) für diese Preisregel infrage kommt. Sie können weitere Bedingungszeilen hinzufügen, um Ihre infrage kommenden Produkte weiter einzuschränken.

1. Um der Anweisung eine weitere Bedingungszeile hinzuzufügen, kehren Sie zu Schritt 1 zurück und wiederholen Sie den Prozess, bis alle gewünschten Bedingungen erfüllt sind.

   Sie können eine Zeile der Bedingungsanweisung jederzeit löschen, indem Sie auf Löschen (![Löschsymbol](assets/btn-del-red.png)) am Ende der Zeile.
