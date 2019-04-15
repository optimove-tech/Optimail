## Migrating Sendgrid current account to Optimail
<a id="migrate"></a>
   - [Can I use my existing IP?](#existing-ip)
   - [Do i still need to do IP warmup?](#ip-warmup-mig)
   - [Could metrics stats be migrated?](#metrics-stats)
   
   
### <a id="existing-ip"></a>Can I use my existing IP?
Yes, you can use your existing IP. However, the IP/domain will be moved to Optimail Sub Account.

### <a id="ip-warmup-mig"></a>Do I still need to do IP warmup?
Regardless if you moved your existing IP/domain to Optimail Sub Account, you will have to go through a "light" IP warmup.
Even though the sending domain and IPs remain the same, small changes in SendGrid configurations are still required.
The "light" warmup process defers a lot on the daily volume, the sending domain used, the current reputation of the sending domain and IP. 
Normally, it shouldn't take longer than 5-6 days. However, it could take more depending on the changes made and the reputation status. 



### <a id="metrics-statsg"></a>Could metrics statistics be migrated?
Metrics statistics could not be migrated from one account to another. If you would like to add data to your new Optimail account, you may export a report (up to 30 days only) from your existing Sendgrid account and ask Optimove to manually add the statistics into your new Optimail account.


<HR>
