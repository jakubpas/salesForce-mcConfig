salesForce-mcConfig
-------------------

mcconfig endpoints:

SalesForce:

 - https://salesforcetest.eniro.com/mcconfig/form - form
 - https://salesforcetest.eniro.com/mcconfig/order - xml
 - https://salesforcetest.eniro.com/mcconfig/demo - xml

SoloTest:

 - http://web2.test.media.eniro/mcconfig/*

== Minimal curl request to get form page: ==

```
curl 'http://web2.test.media.eniro/mcconfig/form' --data 'country=SE&locale=sv_SE&currency=SEK&packageLabel=SMB_BASIC&monthlyBudget=4000&mediaSpendFraction=0.70&companyName=Eniro+Sverige+AB&address=Gustav+III%3As+Boulevard+40%2C+169+73+SOLNA&targetUrl=http%3A%2F%2Fwww.enirogroup.com&startDate=2013-12-15&endDate=&mayKeepExistingData=true&systemId=DEMO&customerId=765432&userId=demo20&bingBlacklist=false&splAccountId=12345&savedFormId='
```

== Minimal curl request to get xml: ==

```
curl 'http://web2.test.media.eniro/mcconfig/order' --data 'country=SE&monthlyBudget=4000&mediaSpendFraction=0.7&packageLabel=SMB_BASIC&currency=SEK&startDate=2013-12-15&endDate=&systemId=DEMO&customerId=765432&userId=demo20&splAccountId=12345&companyDisplayName=Eniro+Sverige+AB&firstMonthBudgetType=FULL&businessPhone=&includeGoogleAnalyticsTags=on&networks=google&networks=bing&locations%5B0%5D.language=sv&locations%5B0%5D.name=Eniro+Sverige+AB&locations%5B0%5D.landingUrl=http%3A%2F%2Fwww.enirogroup.com&locations%5B0%5D.requestedDisplayUrl=www.enirogroup.com&locations%5B0%5D.address.country=se&locations%5B0%5D.radius=50&location.searchAddress=Gustav+III%3As+Boulevard+40%2C+169+73+SOLNA&locations%5B0%5D.address.lon=18.01671410&locations%5B0%5D.address.lat=59.37264252&locations%5B0%5D.categoryIds=SE2200734'
```
