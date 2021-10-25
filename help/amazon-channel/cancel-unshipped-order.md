---
title: Nicht versandte Bestellung abbrechen
description: Ausstehende oder teilweise ausgelieferte (nicht versandte) Bestellung über Ihr Amazon stornieren [!DNL Seller Central] Konto.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Nicht versandte Bestellung abbrechen

Amazon-Bestellungen können nur storniert werden, wenn sie in einer `Unshipped` Status. Wenn die Bestellung aussteht oder teilweise versandt (nicht versandt), kann die Bestellung nur über Ihre [!DNL Amazon Seller Central] Konto. Wenn das Element versendet wurde, müssen Rücksendungen und Austausche auch in Ihrer [!DNL Amazon Seller Central] Konto.

>[!NOTE]
>
>Für andere Aufgaben als die Stornierung einer Bestellung:
>
>- Wenn Sie [Import bestellen](./order-settings.md) aktiviert, werden Bestellungen in der [[!DNL Commerce] Auftragsarbeitsablauf](https://docs.magento.com/user-guide/sales/orders.html){Zielgruppe=&quot;_blank&quot;}.
>- Falls [Import bestellen](./order-settings.md) ist deaktiviert, müssen Sie Ihre Bestellungen verwalten in [!DNL Amazon Seller Central].


## Bestellung abbrechen in `Unshipped` Status

1. Klick **[!UICONTROL View Store]** auf der Ladenkarte.

1. In _[!UICONTROL Recent Orders]_im Store-Dashboard auf eine Bestellnummer klicken.

   Die _[!UICONTROL Amazon Order Details]_angezeigt.

1. Klick **[!UICONTROL Cancel Order]** in der Kopfzeile.

   Diese Option wird nur bei Bestellungen angezeigt in `Unshipped` Status.

1. für **[!UICONTROL Reason for cancellation]**, wählen Sie eine Option aus.

1. Klick **[!UICONTROL Confirm]**.

   Die Bestellung wird abgebrochen und der Status wird aktualisiert auf `Canceled` in den Auftragsdetails.

Die Stornierungsbenachrichtigung wird an Ihre [!DNL Amazon Seller Central] und der mit der Bestellung verbundene Kunde wird ebenfalls benachrichtigt. Der Status der entsprechenden [!DNL Commerce] gegebenenfalls Änderungen an `Complete`.
