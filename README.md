


## Getting Started with Optimail
<a id="intro"></a>Congratulations on choosing Optimail, Optimove’s native email delivery platform. This document describes the steps involved in creating your Optimail account and configuring it for use, as well as answers to commonly asked questions about this process.

- [Optimail Setup Process](#setup)
- [Synchronizing Unsubscribed Customers](#sync-unsub)
- [Improving Email Deliverability](#improve-email-del)
- Frequently Asked Questions
    - [What is IP warming?](#ip-warm)
    - [Do I need more than one IP address?](#one-ip)
    - [How many dedicated IP addresses do I need?](#how-many-ip)
    - [What is a domain name? ](#what-is-domain)
    - [How should I manage unsubscribed users?](#man-unsub)
    - [Does Optimail provide an email preference center?](#email-pref)
    - [Does Optimail have a re-subscribe option?](#resub)
    - [Links Privacy Error](#privacy)
    
<HR>

### <a id="setup"></a>Optimail Setup Process
Before you can begin sending customer email campaigns using Optimove, you will need to perform the following steps.

 1. If customer email addresses are not already included in the tables provided to Optimove as part of your daily data transfer, add the “email address” field to your customer tables. 
 2. Complete and submit the [Optimail Marketing Request Form](https://optimoveteams.atlassian.net/servicedesk/customer/portal/1/group/4/create/30) and/or  [Optimail Transactional Request Form](https://optimoveteams.atlassian.net/servicedesk/customer/portal/1/group/4/create/29) using our Customer Request Portal. After the form is filled out completely, Optimove Product Integration team will send you instructions for adding DNS records to your domain name servers and validating them. 
 3. After the DNS records have been validated, Optimove will enable your Optimail account to your Optimove instance. Your CSM will notify you when you may start using Optimail. 
 4. To get started working with Optimail, you will need to prepare your first email templates and send some test campaigns. For detailed instructions on these steps, see [this Academy article](https://academy.optimove.com/successful-campaigns/getting-started-with-optimail).
 5. Warm up your account to establish a positive sending reputation. See the “Improving Email Deliverability” section, below, for Optimail best practices. 

### <a id="sync-unsub"></a>Synchronizing Unsubscribed Customers from an existing ESP 
To ensure that customers who have already unsubscribed from receiving emails    from your company do not receive emails from Optimail, it is important to synchronize the list of unsubscribed customers from your existing email service provider (ESP) with Optimail.

If your existing ESP is fully integrated with Optimove, Optimove will automatically synchronize the unsubscribed lists between Optimail and your existing ESP. If you are not sure if this is the case, ask your CSM.

If your existing ESP is not fully integrated with Optimove, this synchronization must be performed manually. To do so, send your CSM an up-to-date CSV file containing only the email addresses of all customers who have already unsubscribed from your marketing email list. Your CSM will update Optimail accordingly. You need to send this list to your CSM prior to the date of the first campaign to be sent with Optimail. If you have multiple IP addresses, make sure to inform your CSM which unsubscribe list relates to which Optimail IP address.

If you plan to continue sending emails from your existing ESP as well as Optimail, you will need to continuously synchronize your unsubscribed between the two systems. Consult with your CSM to make sure this is handled appropriately.

### <a id="improve-email-del"></a>Improving Email Deliverability
Deliverability refers to the percentage of emails that are actually delivered to recipients’ inboxes. For obvious reasons, it is important to do everything possible to maximize your deliverability when using Optimail. We recommend implementing the following best practices:

 - Regularly send emails to your most engaged customers (those who tend to respond to them) and to those who have specifically opted in to receive your emails.
 - Regularly cleanse your mailing list by removing bounced email addresses, [role](https://sendgrid.com/blog/role-addresses-and-their-effect-on-email-deliverability/) email addresses and addresses of users who never open your emails.
 - Learn how your template content can affect deliverability. For example, avoid using exclamation marks and currency symbols in your subject line, as well as phrases in the email body that can trigger spam filters.
 - To ensure high open and click rates during the IP warm-up period, it is highly recommended to provide Optimove with a list of your customers’ last clicked and opened events. You can also send Optimove a list of all customers who have opened or clicked emails in the past 60-90 days.
 - Learn more about email deliverability [here](https://sendgrid.com/resource/email-deliverability/).

### <a id="faq"></a>Frequently Asked Questions

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

#### <a id="what-is-domain"></a>What is a domain name? 
The domain name is the root domain for your subdomain. This is the domain that will receive the email reputation from the white label. Your root domain name should match your FROM email address. For example, if you will be sending email from updates@bestdomain.com, the domain name is bestdomain.com.

#### <a id="man-unsub"></a>How should I manage unsubscribed users?
It is recommended to allow Optimail to track and manage unsubscribes (using Sendgrid, Optimail’s underlying deliverability platform). This has the advantage of having an ‘Optimail Unsubscribed’ attribute in Optimove’s customer database, which can be seen in the Customer Explorer page and which can be used to define target groups and ensure more accurate results in Campaign Analysis.

An alternative method is for you to manage unsubscribes manually. If you choose this approach, it is important to include a daily list of unsubscribers, as part of the daily data feed provided to Optimove. This will add a customer attribute that you can use to filter out members of the target groups you use to send email campaigns.

#### <a id="email-pref"></a>Does Optimail provide an email preference center?
Optimail does not currently include this functionality. Once a user clicked has clicked an unsubscribe link, that address is instantly removed from your mailing list. If you wish to present your customers with a custom landing page following an unsubscribe click, you can specify a redirect URL of your own to which Optimail will redirect the user, or allow Optimail to create a landing page with your chosen text.

#### <a id="resub"></a>Does Optimail have a re-subscribe option?
Optimail does not offer this as a built-in feature, but you can offer this to your customers as follows: Create a landing page at which a customer can re-subscribe to your email list. Once you receive an email address in this way, you will need to manually remove the address from the unsubscribers list in Sendgrid.

#### <a id="privacy"></a>Why do my clients get a privacy error while clicking the email's links?
The links in Optimail's emails are tracked by SendGrid, this allows SendGrid to track all clicks per email sent. This option is called "Click Tracking" and is set to the defult option while configuring Optimail accounts.

Enabling Click Tracking through SendGrid allows SendGrid to track all clicks per email sent. Once enabled, SendGrid will wrap the links and URLs in your Optimail templates so that they first are forwarded to SendGrid’s servers and the click is properly tracked, and then instantly redirected to the intended location of the link. Up to 1,000 links per template can be tracked.
However, you may find that once your Optimove success team enables Click Tracking for your account, you encounter a “Wrong Link” error page or “Your connection is not private” message.
This happens because Click Tracking does not support HTTPS URLs or links. If the links to your site are encrypted.  To solve for this, it’s imperative that you consider a long-term solution that modifies where you’re sending traffic to SendGrid from  before Click Tracking is enabled.

#### Turn off HSTS
One option to consider is turning off HSTS.  This is what is forcing all of the links and URLs in your templates to be sent using HTTPS.  By turning off HSTS and using HTTP links in your links and using an SSL certificate, the issue will be fixed and click tracking can be enabled successfully.
#### Use a CDN to Configure an SSL Certificate
Below are the steps to enable SSL Click Tracking for your Optimail account. Note that these steps are not unique to a specific CDN (content delivery network). Should you require detailed support based on your specific CDN, we recommend you work directly with the support team at your CDN.
1.	Create an SSL Certificate for your authenticated domain
Reach out to your CDN or DNS provider to request and/or manage this certificate.  We do not recommend creating wildcard certificates as they have proven not to be stable for click tracking purposes.  As Optimove and SendGrid are not the record owners for this domain, we are unable to make or request the SSL certificate ourselves.
NOTE: Make sure your CDN has the SSL certificate forward all traffic to sendgrid.net. This is necessary so tracking details can be ingested and links can be resolved to the correct location.

2.	Point white label link domain to SSL certificate
Once your SSL certificate has been created, you can start forwarding traffic to this certificate.  Just as you pointed white label link CNAME, you can edit the DATA portion in the domain’s DNS to point to the CDN handling your domain’s SSL certificate.  For example, if you are using a content delivery network you would want to update your records from your authenticated domain pointing to sendgrid.net (i.e. em.yourbrand.com  sendgrid.net) to now have the authenticated domain point to the SSL certificate (i.e. em.yourbrand.com  cdm.em.yourbrand.com)

Now, when someone clicks on one of the links in your template, it will point to the SSL certificate which will forward the traffic back to sendgrid.net.

3.	Confirm SSL creation and updated link pointing with Optimove team
Once you’ve completed steps 1 and 2, let your Optimove success team know and we’ll go ahead and turn SSL Click Tracking on for you.  Before we do, however, we’ll make sure to ensure the following:
a.	The white label link is assigned to the sub-user requesting SSL Click Tracking
b.	The white label link is not pointing at sendgrid.net any longer
c.	The white label link domain is terminating is an SSL connection correctly 


#### Use a custom SSL Certificate
Below are the steps to enable SSL Click Tracking for your Optimail account using your own proxy rather than a CDN.
1.	Prepare a proxy
Prepare the proxy (like a web application, NGINX, or Amazon API Gateway for example) to take all traffic for your branded link (link.yourdomain.com) and forward it to sendgrid.net.

2.	Configure the proxy
Set up the proxy to use HTTP or HTTPS.  For HTTPS, you will want to provide a valid SSL certificate for your branded domain (link.yourdomain.com).

Forward  traffic by setting Host HTTP header to your branded domain and point the CNAME record to your proxy.
3.	Confirm proxy configuration and updated link pointing with Optimove team
Once you’ve completed steps 1 and 2, let your Optimove success team know and we’ll go ahead and turn SSL Click Tracking on for you.  Before we do, however, we’ll make sure to ensure the following:
a.	The white label link is assigned to the sub-user requesting SSL Click Tracking
b.	The white label link is not pointing at sendgrid.net any longer
c.	The white label link domain is terminating is an SSL connection correctly 


