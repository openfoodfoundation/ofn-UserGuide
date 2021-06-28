# Embed a Group Page in a Website

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

It is now possible to embed a group page into a website external to OFN. Here you will find step by step instructions for setting this up.  This feature is relatively new, and has not been comprehensively tested across all platforms. Please [contact your local OFN ](https://www.openfoodnetwork.org/find-your-local-open-food-network/)if you experience issues with embedding a group page in your website. 

## Pre-requisites for Embedding a Group Page 

### Platform

It is possible to embed a group page on any website where you can add custom html to the destination page, including platforms such as WordPress, Squarespace or Wix.

Below are some platform specific resources:

* [Go to Squarespace](https://support.squarespace.com/hc/en-us/articles/206543167) for more information about adding custom html using “codeblocks” 

### Security

Because OFN is an eCommerce platform, and handles monetary transactions, it has a higher security requirement than some websites. Therefore, you’ll need to have SSL/TLS set up on the website you want to embed your group page into. You can get a free security certificate from [Let’s Encrypt](https://letsencrypt.org/) or for around $10-$30 for other paid service.

### OFN Group page

Before proceeding, you should complete [setting up your group page on the Open Food Network](group-page.md). You’ll need to know your OFN group page URL to complete the setup steps below.

## How to Embed a Group Page

**1\) Contact your local OFN team**

First of all, you’ll need to contact [your local OFN team](https://openfoodnetwork.org/ofn-local/) and let them know you want to embed your OFN group page in your website. You’ll need to provide them with your external domain. eg. regionalgroup.com.au so they can grant permission for your website to communicate with OFN.

**2\) Adding Custom HTML to your website**

Embedding your group page is as simple as inserting a line of code into your website. Below is an example of the HTML that you should insert into the page where you want to embed your OFN group page. You will need to replace ‘flavour-crusader’ with your shop’s unique OFN permalink. 

```text
<iframe src="https://openfoodnetwork.org.au/groups/flavour-crusader?embedded_shopfront=true" style="width:100%;min-height:35em"></iframe>
```

Once you’ve done this, you should see your OFN group page appear within your website at the location where you inserted the HTML.

NOTE: See the instructions on [creating and managing a group page](group-page.md) to find out how to edit your unique OFN permalink.

**3\) Styling**

Depending on the styling of your website you may need to edit the CSS. If you are not familiar with CSS you may need to engage the services of your website administrator. CSS may be needed to avoid having two scroll bars, and to make sure the length and width of the embedded group page is visually appealing. Make sure to test the display of your group page on a mobile device as well as this may require further changes.

## Instructions for Visitors

### Cookies

Most people have cookies enabled on their web browsers. But if a visitor doesn’t enable cookies they may see an error message similar to the one below, and not be able to view the embedded group.

![](../../.gitbook/assets/cookies.png)

