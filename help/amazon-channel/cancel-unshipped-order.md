---
title: Abbrechen einer nicht versandten Bestellung
description: Abbrechen einer ausstehenden oder teilweise ausgelieferten (nicht versandten) Bestellung über Ihr Amazon [!DNL Seller Central] Konto.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Abbrechen einer nicht versandten Bestellung

Amazon-Bestellungen können nur storniert werden, wenn sie den Status `Unshipped` aufweisen. Wenn die Bestellung ausstehend oder teilweise versandt (nicht versandt) ist, kann die Bestellung nur über Ihr [!DNL Amazon Seller Central] Konto storniert werden. Wenn der Artikel versandt wurde, müssen Rücksendungen und Umtausch auch in Ihrem [!DNL Amazon Seller Central] -Konto durchgeführt werden.

>[!NOTE]
>
>Für andere Aufgaben als den Abbruch einer Bestellung:
>
>- Wenn Sie [Bestellimport](./order-settings.md) aktiviert haben, werden die Bestellungen im [[!DNL Commerce] Auftrags-Workflow](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} verwaltet.
>- Wenn [Bestellimport](./order-settings.md) deaktiviert ist, müssen Sie Ihre Bestellungen in [!DNL Amazon Seller Central] verwalten.


## Abbrechen einer Bestellung im Status `Unshipped`

1. Klicken Sie auf der Store-Karte auf **[!UICONTROL View Store]**.

1. Klicken Sie im Abschnitt _[!UICONTROL Recent Orders]_des Store-Dashboards auf eine Bestellnummer.

   Die Seite _[!UICONTROL Amazon Order Details]_wird angezeigt.

1. Klicken Sie in der Kopfzeilenleiste auf **[!UICONTROL Cancel Order]** .

   Diese Option wird nur bei Bestellungen mit dem Status `Unshipped` angezeigt.

1. Wählen Sie für **[!UICONTROL Reason for cancellation]** eine Option aus.

1. Klicken Sie auf **[!UICONTROL Confirm]**.

   Die Bestellung wird abgebrochen und der Status wird in den Bestelldetails auf `Canceled` aktualisiert.

Die Stornierungsbenachrichtigung wird an Ihr [!DNL Amazon Seller Central]-Konto gesendet und der mit der Bestellung verbundene Kunde wird ebenfalls benachrichtigt. Der Status der entsprechenden [!DNL Commerce]-Bestellung ändert sich, falls vorhanden, in `Complete`.
