---
title: '''Beispiel: Bedingung definieren"'
description: Definieren Sie beim Erstellen Ihrer Listingregeln die Bedingungen für die Identifizierung der Commerce-Katalogprodukte, die auf dem Amazon Marketplace aufgelistet werden sollen.
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# Beispiel: Bedingung definieren

## Bedingungen

Alle Bereiche in den Bedingungen, die fett sind, können angeklickt werden, um die verschiedenen Optionen zu sehen.

**Fügen Sie keine Bedingungen hinzu, wenn alle Produkte auf der ausgewählten Website förderfähig sind.**

>[!NOTE]
>
>Es gibt eine komplexe Reihe von Back-End-Prozessen, die direkt mit Amazon-Systemen kommuniziert werden können. Aufgrund der Anzahl der Elemente, die Sie zu Listen versuchen, und der möglicherweise sehr ausgelasteten Amazon-Systeme (z. B. Black Freitag) kann es einige Zeit dauern, bis Ihre Artikel auf Amazon aufgelistet werden.

Siehe Abschnitt &quot;Bedingungen&quot; von [Erstellen einer Preisregel für Warenkorb](https://docs.magento.com/user-guide/marketing/price-rules-catalog-create.html){Zielgruppe=&quot;_blank&quot;}.

## Bedingung definieren

Dieser Vorgang kann je nach Katalogeinrichtung einfach oder detailliert sein. Sie können die Bedingungen so festlegen, dass wann `ALL` oder `ANY` der definierten Bedingungen `TRUE` oder `FALSE` für ein Produkt, ist das Produkt berechtigt, auf Amazon aufgeführt zu werden.

Die Bedingungen basieren auf vorhandenen Produktattributwerten. Lassen Sie den Bedingungsabschnitt leer, um die Regel auf alle Produkte anzuwenden.

>[!NOTE]
>
>Wenn Sie eine Bedingung basierend auf einem bestimmten Produktattribut definieren möchten, legen Sie die **[!UICONTROL Use for Promo Rule Conditions]** Einstellung für das Attribut `Yes`. Sie können auf diese Einstellung zugreifen auf [Storefront-Eigenschaften](https://docs.magento.com/user-guide/catalog/product-attributes-add.html){Zielgruppe=&quot;_blank&quot;} Seite für das Attribut.

![Bedingung - Zeile 1](assets/ob-listing-rule-conditions-start.png)

Die Regel in diesem Beispiel definiert eine Regel, die die Amazon-Berechtigung für alle Katalogprodukte festlegt, die _Amazon FBA_ Attribut festgelegt auf `Yes`.

Die Rule-Anweisung hat zwei fette Links, die, wenn sie angeklickt wird, die Optionen für diesen Teil der Anweisung anzeigen. Wenn Sie die Bedingung speichern, ohne eine fette Option zu ändern, gilt die Regel für alle Ihre Produkte.

- Klick **[!UICONTROL ALL]** und wählen Sie entweder `ALL` oder `ANY`.
- Klick **[!UICONTROL TRUE]** und wählen Sie entweder `TRUE` oder `FALSE`.
- Um die Regel auf alle Produkte anzuwenden, lassen Sie die Bedingung unverändert.

Sie können verschiedene Bedingungen erstellen, indem Sie die Kombination dieser Werte ändern. Für dieses Beispiel wird die folgende Bedingung verwendet:

`If ALL of these conditions are TRUE:`

1. Klicken Sie auf das Hinzufügen (![Symbol Hinzufügen](assets/btn-add-grn.png)) am Anfang der Bedingungslinie und wählen Sie ein Attribut aus, auf dem die Bedingung basieren soll, wie z. B. eine Bedingungskombination oder ein Produkteigenschaften.

   - **[!UICONTROL Conditions Combination]** - Erlauben Sie , dass Sie einen anderen Satz von `All/Any` und `True/False` Bedingungen innerhalb des vorhandenen Sets.

      ![Bedingungskombination](assets/ob-conditions-combinations.png)

   - **[!UICONTROL Product Attribute]** - Die Produktattribute hängen vom Setup des Attributs ab. Damit ein Attribut in der Liste angezeigt wird, muss es für die Verwendung in Werberegelbedingungen konfiguriert werden. Siehe _Für Promotion-Regelbedingungen verwenden_ in [Produktattribute](https://docs.magento.com/user-guide/stores/attributes-product.html){Zielgruppe=&quot;_blank&quot;}.

      In der Liste unter **[!UICONTROL Product Attribute]**, wählen Sie das Attribut aus, das Sie als Grundlage für die Bedingung verwenden möchten. In diesem Beispiel ist die ausgewählte Bedingung `Amazon FBA`.

      ![Bedingungslinie 2, Teil 2](assets/ob-condition-attribute-dropdown.png)

      Die ausgewählte Bedingung wird in der Anweisung angezeigt, gefolgt von zwei weiteren fett formatierten Links. Die Optionen sind je nach ausgewähltem Produktattribut unterschiedlich.

      Nachdem Sie das Attribut festgelegt haben, kann es nicht mehr geändert werden. Um das Attribut zu ändern, müssen Sie die Zeile löschen und das neue Attribut hinzufügen. Sie können eine Bedingungszeile löschen, indem Sie auf &quot;Löschen&quot; klicken (![Symbol löschen](assets/btn-del-red.png)) am Ende der Zeile.

      1. Klick **[!UICONTROL is]** und wählen Sie den Vergleichsoperator aus, der die Bedingung beschreibt, dass die Produkte erfüllt werden sollen.

         In diesem Beispiel ist der Vergleichsoperator `is`. Die verfügbaren Optionen hängen vom im vorherigen Schritt ausgewählten Attribut ab. Optionen können verschiedene Vergleichsoptionen wie Übereinstimmungswerte umfassen, die nicht mindestens einen Wert enthalten oder nicht enthalten und größer als, gleich und kleiner als ein numerischer Wert sind. In diesem Beispiel sind die Optionen `is` und `is not`.

      1. Klick **[!UICONTROL ...]** und wählen Sie den Attributwert, auf dem die Bedingung basiert.

         Die Optionen hängen vom Setup des Attributs ab. Sie werden möglicherweise aufgefordert, eine Option auszuwählen oder Text- oder Zahlenwerte für die Bedingung einzugeben. In diesem Beispiel ist die Auswahl `Yes`.

         Das ausgewählte Element wird in der Anweisung angezeigt, um die Bedingung zu vervollständigen.

         ![Bedingungslinie 2, Teil 3](assets/ob-listing-rule-condition-is.png)
   Diese Bedingung ist vollständig. Wie angegeben bedeutet diese Bedingung, dass jedes Produkt in Ihrem [!DNL Commerce] Katalog, für den das Amazon FBA-Attribut auf einen Wert von `Yes` ist für die Aufnahme in Amazon für die Region und das Geschäft zugelassen. Sie können weitere Bedingungslinien hinzufügen, um die förderfähigen Produkte weiter einzuschränken.

1, Um der Anweisung eine weitere Bedingungszeile hinzuzufügen, kehren Sie zu Schritt 1 zurück und wiederholen Sie den Prozess, bis alle gewünschten Bedingungen erfüllt sind.

Sie können eine Zeile der Bedingungsanweisung jederzeit löschen, indem Sie auf Löschen (![Symbol löschen](assets/btn-del-red.png)) am Ende der Zeile.
