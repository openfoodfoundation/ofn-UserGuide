# Thermally printed receipts

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

{% hint style="danger" %}
This functionality is currently only available to OFN users in France. Contact your local OFN for more details, or to request use of this feature.
{% endhint %}

## Printer

What printer do I need to print a “receipt”, like the one you usually get in a store? You need a thermal printer that talks ESC/P control language \(most of them do\).

For instance:

Epson one \(most common in shops\). Available on Amazon for approx USD $135  
Low cost no-name one \(USD $33\): Available on Amazon for approx USD $33

## Setup

How do I setup my machine to be able to print receipts from the OFN?

First you need to install the printer by following the instructions for your operating system provided by your supplier.  \(For an USB printer you might not have to specify the URI; just make sure you use the relevant driver.\)

Then you need to install QZ Tray which is a plug-in for printers that will launch the printing of the receipt without you having to select the printer and click on “print”. You can download the QZ Tray [from this site](https://qz.io/download/#).

Launch QZ Tray if it didn’t launch automatically. Then open the page “print\_ticket.html” in your browser, digital certificates will not work but you will be able to print a test page.

## Printing receipts in OFN

Click orders in the blue menu, click on a customer order. Under the actions menu you will see print receipt. Click on it. A new tab should open, after allowing the communication with QZ Tray it will show a list of your printers, select the thermal one and it will print the receipt.

The selected printer will be saved in your browser, if you wish to change it there is a button for this under the same “actions” menu as for printing the receipt.

