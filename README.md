# exchange-rates-challenge
Technical Challenges to help learn

Requirements, Rules, Guide:
1. No cheating - it doesn't benefit you.
2. Let's have fun, don't take it too seriously. Aim is to learn and to push yourself.
3. Each challenge will build upon the previous one.
4. You'll need have a GitHub account.
5. We will start slow/small and will build up as we go along.
6. No time limit will be applied - but maybe we should have some form of agreement - maybe we DO set time.
7. Use the slack channels for help - we will support each other.

Challenge Business Brief:
Build a service that will expose a way to convert currencies. For example convert 10.99 GBP to AED. 
For the sake of simplicity we will limit the number of currencies to AED, EUR, GBP, INR, PKR and USD. 


Challenges Overview

1. Build an exchange rate API, only GET method required. This GET method should look like /api/v1/{FROM_CURRENCY/{TO_CURRENCY}/

{AMOUNT}. The /api endpoint should be the context root. The API will return the following JSON:

{
	"from_currency" : AED,
	"to_currency": GBP,
	"from_amount: 10.00,
	"to_amount": 2.07,
	"exchange_rate": 0.21
}

The actual exchange rate will be obtained from providers like currencylayer.com (you'll need to maintain the keys for the 

providers).


Rules and expected result:
1. You cannot use Spring (unless if you haven't used it before)
2. You can use whatever language you like even Java.
3. You must provide your GitHub repo README which must include: design diagram and steps on how to run.
4. The runnable code must be available as a release from GitHub.
5. The name of your deployable/executable should be in this format:  exchange-rate-firstname.[jar, exe, bat etc]
6. You should be able to run (a provided) set of JMeter tests that all pass against your GET API.


---

2. Create a travis CI build pipeline for your code. The pipeline should checkout the code, run the tests (as well as JMeter), 

build the package and create a release to github.

---

3. Now that you have a pipeline, extend it to include the creation of a docker image. Once a package has been created its docker 

image should be pushed to a docker registry (prefer dockerhub).

---
4. Extend the code base to create a java client. This client will allow access to your service without having to do any plumbing. 

The client api (first version) should look something like (Java):

ExchangeRateResponse response = ExchangeRateClient().withHost(...).withPort(...).fromCurrency(...).toCurrency(...).amount

(...).call(); 


---
5. For the client you should also create the travis job, pipeline, docker etc.

---
6. 


OAuth

API Testing (CDC)

Cloud deployment (Google/AWS)

RSocket

Serverless

NoSQL

Blockchain

Mobile App   
