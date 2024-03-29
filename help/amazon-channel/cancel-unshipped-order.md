---
title: Abbrechen einer nicht versandten Amazon-Bestellung
description: Abbrechen einer ausstehenden oder teilweise ausgelieferten (unausgelieferten) Bestellung über Ihre Amazon [!DNL Seller Central] -Konto.
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Abbrechen einer nicht versandten Amazon-Bestellung

Amazon-Bestellungen können nur storniert werden, wenn sie sich in einer `Unshipped` -Status. Wenn die Bestellung ausstehend oder teilweise versandt (nicht versandt) ist, kann die Bestellung nur über Ihre [!DNL Amazon Seller Central] -Konto. Wenn der Artikel versandt wurde, müssen auch die Rücksendungen und der Austausch in Ihrer [!DNL Amazon Seller Central] Konto.

>[!NOTE]
>
>Für andere Aufgaben als den Abbruch einer Bestellung:
>
>- Wenn Sie [Bestellimport](./order-settings.md) aktiviert ist, werden die Bestellungen im [[!DNL Commerce] Auftragsworkflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).
>- Wenn [Bestellimport](./order-settings.md) deaktiviert ist, müssen Sie Ihre Bestellungen in [!DNL Amazon Seller Central].

## Abbrechen einer Bestellung in `Unshipped` status

1. Klicks **[!UICONTROL View Store]** auf der Speicherkarte.

1. Im _[!UICONTROL Recent Orders]_Klicken Sie im Store-Dashboard auf eine Bestellnummer.

   Die _[!UICONTROL Amazon Order Details]_angezeigt.

1. Klicks **[!UICONTROL Cancel Order]** in der Kopfzeile.

   Diese Option wird nur bei Bestellungen in `Unshipped` -Status.

1. Für **[!UICONTROL Reason for cancellation]**, wählen Sie eine Option.

1. Klicken **[!UICONTROL Confirm]**.

   Die Bestellung wird abgebrochen und der Status wird aktualisiert auf `Canceled` in den Bestelldetails.

Die Stornierungsbenachrichtigung wird an Ihre [!DNL Amazon Seller Central] -Konto und der mit der Bestellung verbundene Kunde wird ebenfalls benachrichtigt. Der Status der entsprechenden [!DNL Commerce] gegebenenfalls die Reihenfolge der Änderungen an `Complete`.
