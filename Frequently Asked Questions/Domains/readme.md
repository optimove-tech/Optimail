## Domains
<a id="domains"></a>
   - [What is a domain name? ](#what-is-domain)
   - [Could multiple 'from' addresses with different sub-domains affect my deliverability? ](#mult-from)
   - [Can I use the same domain for other email purposes? ](#same-domain)
   - [Can I use the same domain for both my marketing and transactional accoounts? ](#same-domain-tr-mkg)
   - [I want to change my domain, will an IP warmup be needed? ](#change-domain-warmup)
 
#### <a id="what-is-domain"></a>What is a domain name? 
The domain name is the root domain for your subdomain. This is the domain that will receive the email reputation from the white label. Your root domain name should match your FROM and REPLY TO email address. For example, if you will be sending email from updates@bestdomain.com, the domain name is bestdomain.com. If there's a mismatch between the two it could affect your reputation and might reduce deliverability rates.

#### <a id="mult-from"></a>Can multiple 'from' addresses with different sub-domains affect my deliverability?
As long as the domain name (example.com) is used in the 'from' email subdomain (example@<b>example.com</b>) the deliverability should not be affected. However, when the 'from' email (updates@example2.com) domain does not match the domain name (example.com) the deliverability might be affected.

#### <a id="same-domain"></a>Can I use the same domain for other email purposes?
This is not recommended, as a conflight might occur and it might affect your reputation. We recommend using differnt subdomain to avoid any conflicts.
For example: instead of using example.com, use email.exmple.com

#### <a id="same-domain-tr-mkg"></a>Can I use the same domain for both my marketing and transactional accoounts? 
This is not recommended, as a conflit might occur and it might affect your reputation. We recommend using differnt subdomain to avoid any conflicts.
For example: for transactional emails use: tran.example.com and for marketing mkg.example.com.
NOTE: FROM address should match the domain name. For example: info@mkg.example.com.

#### <a id="change-domain-warmup"></a>I want to change my IP, will an IP warmup be needed?
Yes, the reputation is specific to the IP/domain combination and any change requires a new warmup.

#### <a id="change-domain-warmup"></a>I want to change my domain, will an IP warmup be needed?
Yes, the reputation is specific to the IP/domain combination and any change requires a new warmup.



<HR>
