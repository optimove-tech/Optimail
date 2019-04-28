## Unsubscribes
<a id="Unsubscribes"></a>
   - [How should I manage unsubscribed users?](#man-unsub)
   - [How to syncornize unsubscribed customers from existing ESP?](#sync-unsub)
   - [Does Optimail have a re-subscribe option?](#resub)
   - [What is Optimail Preference Center?](#pref)
   - [Can I use List-Unsubscribe header?](#list-unsubscribe)
   
   
#### <a id="man-unsub"></a>How should I manage unsubscribed users?
It is recommended to allow Optimail to track and manage unsubscribes (using Sendgrid, Optimail’s underlying deliverability platform). This has the advantage of having an ‘Optimail Unsubscribed’ attribute in Optimove’s customer database, which can be seen in the Customer Explorer page and which can be used to define target groups and ensure more accurate results in Campaign Analysis.

#### <a id="sync-unsub"></a>How to syncornize unsubscribed customers from existing ESP?
To ensure that customers who have already unsubscribed from receiving emails from your company do not receive emails from Optimail, it is important to synchronize the list of unsubscribed customers from your existing email service provider (ESP) with Optimail.

If your existing ESP is fully integrated with Optimove, Optimove will automatically synchronize the unsubscribed lists between Optimail and your existing ESP. If you are not sure if this is the case, ask your CSM.

If your existing ESP is not fully integrated with Optimove, this synchronization must be performed manually. To do so, send your CSM an up-to-date CSV file containing only the email addresses of all customers who have already unsubscribed from your marketing email list. Your CSM will update Optimail accordingly. You need to send this list to your CSM prior to the date of the first campaign to be sent with Optimail. If you have multiple IP addresses, make sure to inform your CSM which unsubscribe list relates to which Optimail IP address.

If you plan to continue sending emails from your existing ESP as well as Optimail, you will need to continuously synchronize your unsubscribed between the two systems. Consult with your CSM to make sure this is handled appropriately.

#### <a id="resub"></a>Does Optimail have a re-subscribe option?
Yes, Optimove does offer re-subscribe option through our [Preference Center](#pref) feature.

#### <a id="pref"></a>What is Optimail Preference Center?
Optimail Preference Center allows your customers to easily choose which types of email communications they receive from you, and to update those choices at any time. For further informtaion, please read [this article](https://academy.optimove.com/successful-campaigns/implementing-optimail-preference-center) in Optimove Academy.
To implement Optimail Preference Center, please contact your CSM.



#### <a id="list-unsubscribe"></a>Can I use List-Unsubscribe header?
List-Unsubscribe header is an optional email header you can add to your email messages.
If you're using Optimail subscription tracking the List-Unsubscribe will be added automatically, both the mailto: and http: versions will be inserted. However, if you are the one managing your unsubscribes, this option is not available. Currently Optimail does not support this functionality unless using Optimail subscription tracking.
<HR>
