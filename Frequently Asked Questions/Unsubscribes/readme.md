## Unsubscribes
<a id="Unsubscribes"></a>
   - [How should I manage unsubscribed users?](#man-unsub)
   - [Does Optimail have a re-subscribe option?](#resub)
   
   
#### <a id="man-unsub"></a>How should I manage unsubscribed users?
It is recommended to allow Optimail to track and manage unsubscribes (using Sendgrid, Optimail’s underlying deliverability platform). This has the advantage of having an ‘Optimail Unsubscribed’ attribute in Optimove’s customer database, which can be seen in the Customer Explorer page and which can be used to define target groups and ensure more accurate results in Campaign Analysis.


#### <a id="resub"></a>Does Optimail have a re-subscribe option?
Optimail does not offer this as a built-in feature, however you may create a landing page at which a customer can re-subscribe to your email list. Once you receive an email address in this way, you will need to manually remove the address from the unsubscribers list in Optimail.

#### <a id="resub"></a>Can I use List-Unsubscribe header?
List-Unsubscribe header is an optional email header you can add to your email messages.
If you're using Optimail subscription tracking the List-Unsubscribe will be added automatically, both the mailto: and http: versions will be inserted. However, if you're not using Optimail subscription tracking you will need to insert both manually. However, currently Optimial does not support this functionality and unless using Optimail subscription tracking, List-Unsubscribe header could not be implemented.
<HR>
