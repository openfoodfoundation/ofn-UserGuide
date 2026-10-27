# Customers

Hub and producer sellers on the Open Food Network can access the Customers page whilst logged in to see a list of customers who have placed an order with them. Customers are added to this list automatically when an order is placed, and enterprise managers can also manually add customers if they wish to use the [Tag Rules](shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md) functionality for example. Customer codes can also be added if required.

## Balance and Credit

The Customers page shows a **Balance** amount against each customer (if not displayed, you can adjust which columns are shown via the **Columns** dropdown above the list). This shows the total amount owed to or owed by the customer, taking into account orders that have not yet been paid and refunds or credits that are owed to the customer. In the example below, the customer owes £10.00 to the enterprise.

<figure><img src="../.gitbook/assets/Screenshot 2026-10-27 at 14.08.54.png" alt="" width="375"><figcaption></figcaption></figure>

The **Available Credit** column (again, this can be displayed via the **Columns** dropdown if not showing) shows the total credit available on the customer's account. Credit is awarded either by [crediting the customer directly from an order](orders/refunds-and-adjusting-payments.md), e.g. to refund a missing item, [via the API](https://ofn-user-guide.gitbook.io/ofn-api-handbook/ofn-api-v1/customer-account-transaction-customer-credit), or manually from the Customers screen. You can click the amount in the **Available Credit** column to display a pop-up showing the history of credits awarded and spent by the customer.

<figure><img src="../.gitbook/assets/Screenshot 2026-10-27 at 14.37.53.png" alt="" width="323"><figcaption><p>Click '£0.33' to launch the credit history pop-up </p></figcaption></figure>

Credit is automatically deducted from the customer's next order at checkout. Credit history is shown with a transaction date, a description (e.g. which order the credit was spent on or refunded from), who created it (only if credit was applied using the API), the amount, and a running balance.

<figure><img src="../.gitbook/assets/Screenshot 2026-10-27 at 14.36.35.png" alt=""><figcaption></figcaption></figure>

### Manually Adding Credit

To add credit to a customer's account manually, for example to award a gift voucher or reward a volunteer, click the **+ Add Credit** button shown above the credit history:

<figure><img src="../.gitbook/assets/Screenshot 2026-10-27 at 14.36.35 (1).png" alt="" width="375"><figcaption></figcaption></figure>

You can then enter an amount and a description - it's sensible to enter a clear description rather than just 'credit' to help keep records useful, especially if you have multiple managers helping to manage your enterprise.

<figure><img src="../.gitbook/assets/Screenshot 2026-10-27 at 15.09.48.png" alt="" width="375"><figcaption></figcaption></figure>

{% hint style="info" %}
N.B. You cannot enter a negative amount, so double check the amount you enter before adding credit. If you make a mistake and need to remove credit, contact your support team.
{% endhint %}
