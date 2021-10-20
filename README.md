**The GTM UIM Profiling Container is a simple way to integrate the UIM Profiling Container via the Google Tag Manager**

#  UIM Profiling Container

The UIM Profiling Container is the data basis for dynamic product retargeting at all stages of the conversion funnel. The event-based profiling solution can be used to readdress interested parties within the media reach of [United Internet Media](https://www.united-internet-media.de/).

## Configuration

![UIM Profiling Container](/uim-profiling-container.png)

### UIM Profiling Container name

Enter your UIM Profiling Container name

### event type

For different stages of the conversion funnel select one of the following "Event" values via dropdown:

* `general`: marking user on unspecific pages 
* `category`: category of product
* `product`: detail of product
* `basket`: view of basket
* `checkout`: sucessfull order

#### general

* `page_name`: Title of the page the customer is visiting.

#### category

* `category_id`: ID of the category.
* `category_name`: Name of the category.

Select at least one of the above.

#### product

* `product_id`: Individual product ID of product. The values of product_id have to match the product ID of your product feed.
* `product_name`: (optional) Product name, e.g. "Red Shoes".
* `product_price`: (optional) Gross product price incl. tax (e.g. "123.45"). Use decimal points "." as separator. No thousands separators.
* `product_currency`: Currency code corresponding to ISO 4217 (e.g. "EUR", "CHF", ...).

#### basket

* `basket_total`: Total gross price incl. tax of the basket (e.g. "123.45"). Use decimal points ".". No thousands separators.
* `basket_items`: (optional) Comma separated list of item IDs in the basket.
* `basket_currency`: Currency code corresponding to ISO 4217 (e.g. "EUR", "CHF", ...).

#### checkout

* `order_id`: Individual order ID (order number/PO number).
* `order_items`: Comma separated list of purchased items (product id).
* `order_total`: Total gross price incl. tax of order items (e.g. "123.45"). Use decimal points "." as separator. No thousands separators.
* `order_shipping`: (optional) Shipping price for the order (e.g. "4.99"). Use decimal points "." as separator. No thousands separators.
* `order_currency`: Currency code corresponding to ISO 4217 (e.g. "EUR", "CHF", ...).

### netID

* `uuid_netid`: netID Identifier if available - for more Information see [netid.de](https://netid.de/)

### Privacy

* `privacy_law`: Possible values: gdpr, ccpa, ...
* `privacy_consent`: Defines if a consent was given by the user. Possible values: 1 if consent is granted, 0 if not.
