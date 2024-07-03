# Reports for Bulk Order Management

The reports available in the Bulk Coop section are ideal for enterprises on the OFN platform, such as buying groups, who use the [Group Buy feature](../products-1/group-buy-for-bulk-ordering.md).

There are four reports in this section are:

|                 | Use                                                                                                                                                                                                                            |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Supplier Report | <p>List products by supplier.</p><p>A good place to look to see if</p><p>enough of a product has been </p><p>ordered to justify the supplier's<br>bulk size.</p>                                                               |
| Allocation      | <p>Lists products by customer.</p><p>A good place to look to </p><p>ensure you over / under</p><p>allocate bulk buy items to</p><p>customers evenly (ie. one </p><p>person is not short on all</p><p>items in their order)</p> |
| Packing Sheet   | <p>Re-packing products delivered <br>a supplier in bulk for customer </p><p>collection</p>                                                                                                                                     |
| Customer totals | <p>Documents refunds to/extra</p><p>payment required by customer</p><p>after adjusting stock levels</p><p>to make up a bulk order</p>                                                                                          |

## Data

The data in each report is as follows:

|                                                   | Supplier Report | Allocation | Packing | <p>Customer</p><p>Totals</p> |
| ------------------------------------------------- | --------------- | ---------- | ------- | ---------------------------- |
| Customer                                          | N               | Y          | Y       | Y                            |
| Supplier                                          | Y               | N          | N       | N                            |
| Product name                                      | Y               | Y          | Y       | N                            |
| Variant details                                   | Y               | Y          | Y       | N                            |
| Bulk unit                                         | Y               | Y          | N       | N                            |
| Quantity Purchased                                | Y               | Y          | Y       | N                            |
| Units required                                    | Y               | Y          | N       | N                            |
| Unallocated                                       | Y               | Y          | N       | N                            |
| Max excess quantity                               | Y               | Y          | N       | N                            |
| Date of order                                     | N               | N          | N       | Y                            |
| <p>Amount paid, owing</p><p>&#x26; total cost</p> | N               | N          | N       | Y                            |

{% hint style="warning" %}
Products stocked by a hub which do not have bulk buy enabled will display with Bulk Unit = 0
{% endhint %}

![Bulk Coop Supplier Report](<../../.gitbook/assets/bulk suppliers report.jpg>)

![Bulk Coop Allocation](<../../.gitbook/assets/bulk allocation report.jpg>)

![Bulk Coop Packing](<../../.gitbook/assets/bulk coop packing sheets.jpg>)

![Bulk Coop Customer Payments](<../../.gitbook/assets/bulk coop customer payment.jpg>)

## Example: Bulk Co-op Suppliers Report

This report will show the following information:

* Did customers order enough of a product to justify ordering the bulk size from the supplier?
* How much extra product are customers willing to purchase to help the group reach the bulk size threshold (if [Group Buy](../products-1/group-buy-for-bulk-ordering.md#enabling-group-buy-for-a-product) is enabled)
* How many bulk sizes are required to meet customer demand?
* If the bulk size is ordered, how much stock will be left over.
* How many customers will be disappointed if this product isn’t ordered?

See the example below for an illustration of how the Bulk Co-op Totals by Supplier report can be used:

Example 1: Where the bulk ordering quantity has been reached:

![Radishes](../../.gitbook/assets/radishess.png)

Example 2: where the bulk order quantity has not been reached:

![Bok Choy](../../.gitbook/assets/bok-choy.png)

* _Note the ‘Bulk Co-op Allocations’ report is similar in function to this report, but shows each customer’s order individually, rather than the cumulative total across all customers._
