# Reports for Bulk Order Management

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

The reports available in the Bulk Coop section are ideal for enterprises on the OFN platform, such as buying groups, who use the [Group Buy feature](../products-1/group-buy-for-bulk-ordering.md).

There are four reports in this section are:

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left">Use</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Supplier Report</td>
      <td style="text-align:left">
        <p>List products by supplier.</p>
        <p>A good place to look to see if</p>
        <p>enough of a product has been</p>
        <p>ordered to justify the supplier&apos;s
          <br />bulk size.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Allocation</td>
      <td style="text-align:left">
        <p>Lists products by customer.</p>
        <p>A good place to look to</p>
        <p>ensure you over / under</p>
        <p>allocate bulk buy items to</p>
        <p>customers evenly (ie. one</p>
        <p>person is not short on all</p>
        <p>items in their order)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Packing Sheet</td>
      <td style="text-align:left">
        <p>Re-packing products delivered
          <br />a supplier in bulk for customer</p>
        <p>collection</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Customer totals</td>
      <td style="text-align:left">
        <p>Documents refunds to/extra</p>
        <p>payment required by customer</p>
        <p>after adjusting stock levels</p>
        <p>to make up a bulk order</p>
      </td>
    </tr>
  </tbody>
</table>

## Data

The data in each report is as follows:

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left">Supplier Report</th>
      <th style="text-align:left">Allocation</th>
      <th style="text-align:left">Packing</th>
      <th style="text-align:left">
        <p>Customer</p>
        <p>Totals</p>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Customer</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
    </tr>
    <tr>
      <td style="text-align:left">Supplier</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
    </tr>
    <tr>
      <td style="text-align:left">Product name</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">N</td>
    </tr>
    <tr>
      <td style="text-align:left">Variant details</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">N</td>
    </tr>
    <tr>
      <td style="text-align:left">Bulk unit</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
    </tr>
    <tr>
      <td style="text-align:left">Quantity Purchased</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">N</td>
    </tr>
    <tr>
      <td style="text-align:left">Units required</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
    </tr>
    <tr>
      <td style="text-align:left">Unallocated</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
    </tr>
    <tr>
      <td style="text-align:left">Max excess quantity</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
    </tr>
    <tr>
      <td style="text-align:left">Date of order</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">Y</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>Amount paid, owing</p>
        <p>&amp; total cost</p>
      </td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">Y</td>
    </tr>
  </tbody>
</table>

{% hint style="warning" %}
Products stocked by a hub which do not have bulk buy enabled will display with Bulk Unit = 0
{% endhint %}

![Bulk Coop Supplier Report](../../.gitbook/assets/bulksuppliertot.jpg)

![Bulk Coop Allocation](../../.gitbook/assets/bulkallocation.jpg)

![Bulk Coop Packing](../../.gitbook/assets/bulkpacking.jpg)

![Bulk Coop Customer Totals](../../.gitbook/assets/bulkpayment.jpg)

## Example: Bulk Co-op Suppliers Report

This report will show the following information:

* Did customers order enough of a product to justify ordering the bulk size from the supplier?
* How much extra product are customers willing to purchase to help the group reach the bulk size threshold \(if [Group Buy](../products-1/group-buy-for-bulk-ordering.md#enabling-group-buy-for-a-product) is enabled\)
* How many bulk sizes are required to meet customer demand?
* If the bulk size is ordered, how much stock will be left over.
* How many customers will be disappointed if this product isn’t ordered?

See the example below for an illustration of how the Bulk Co-op Totals by Supplier report can be used:

Example 1: Where the bulk ordering quantity has been reached:

![Radishes](../../.gitbook/assets/radishess.png)

Example 2: where the bulk order quantity has not been reached:

![Bok Choy](../../.gitbook/assets/bok-choy.png)

* _Note the ‘Bulk Co-op Allocations’ report is similar in function to this report, but shows each customer’s order individually, rather than the cumulative total across all customers._

