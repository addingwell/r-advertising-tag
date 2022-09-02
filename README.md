# R Advertising Tag for Google Tag Manager Server Side

The R Advertising Tag allows advertisers to store a server-side cookie and send a conversion event (S2S) to [R Advertising](https://www.r-advertising.com/ "R Advertising's Homepage").

This tag tracks three events types:
- `page_view` reads R Advertising's query parameter from the URL (`tduid`) and stores it on a server-side cookie named `radv`
- `purchase` sends the event to R Advertising


By default the value sent is using the GA4 data model:
- `orderNumber` is using the `transactionId` from GA4
- `orderValue` is using the operation: `eventModel.value - eventModel.tax - eventModel.shipping` to get the value without tax and shipping.

Both of those parameters can be overwritten in the advanced parameters section.


### Reporting Bugs/Feedback
Please raise any issue on GitHub.

### Open Source
Kwanko Tag Tag for GTM Server Side is developed and maintained by [Addingwell](https://www.addingwell.com/) under the Apache 2.0 license.