## Challenges
https://github.com/imamchishty/exchange-rates-challenge/wiki

## External Resources
To solve challance we need exchange rate of source to target currency.
To get exchange rates following API can be used
https://free.currencyconverterapi.com/api/v6/convert?q=AED_INR&compact=y

This url returns following JSON response
{
  AED_INR: {
  val: 19.73307
  }
}

verbose mode of the same API is:
https://free.currencyconverterapi.com/api/v6/convert?q=AED_INR

Which returns following JSON
{
	query: {
		count: 1
		},
		results: {
			AED_INR: {
				id: "AED_INR",
				fr: "AED",
				to: "INR",
				val: 19.73307
			}
		}
}
## Participants

| Name | Framework/Language Used | Currency Service Repo | CI | Cloud Deployment |
|------|-------------------------|-----------------------|---------------|---------------|
|Imam Chishty | Golang | https://github.com/imamchishty/exchange-rates | [Circle CI]() | TBD | 

