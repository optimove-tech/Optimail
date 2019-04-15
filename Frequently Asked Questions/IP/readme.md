## IP
<a id="IP"></a>
   - [What is IP warming?](#ip-warm)
   - [Do I need more than one IP address?](#one-ip)
   - [How many dedicated IP addresses do I need?](#how-many-ip)
   
 
#### <a id="ip-warm"></a>What is IP warming?
IP warming is the process of gradually increasing the volume of mail sent with a new IP address, in order to establish a positive sending reputation with Internet Services Providers (ISPs).

When ISPs observe large volumes of email suddenly coming from a new or “cold” IP address, they may take notice and begin monitoring the traffic coming from that IP. Since ISPs treat email volume as a key determining factor when detecting spam, it is best to begin sending low to moderate volumes of email, eventually working your way up to larger volumes.

A gradual warm-up does not always guarantee a perfect sending reputation. It is still important to follow the [recommendations](https://sendgrid.com/blog/10-tips-to-keep-email-out-of-the-spam-folder/) mentioned above, in Improving Email Deliverability.

#### <a id="one-ip"></a>Do I need more than one IP address?
There are two main situations in which when an additional IP address is advisable:

 1. High sending volume: If you send batches of over one million email messages and it’s important that they are delivered within a certain timeframe, it may be necessary to use multiple IP addresses.
 2. Separating types of emails: Since each IP address maintains its own deliverability reputation, sending different types of emails via different IP addresses will keep the reputation of each type of email separate. Some examples of email types that you might want to keep separate are transactional messages (e.g., order confirmations, shipping updates), marketing/promotional messages, newsletters and different brands managed by a single company.

#### <a id="how-many-ip"></a>How many dedicated IP addresses do I need?
For email volumes up to 1.5M per day, we advise using at least two IP addresses. Learn more [here](https://sendgrid.com/docs/assets/IPWarmupSchedule.pdf).
<HR>
