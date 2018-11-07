# Task 1: Restful API

## What?
Build an exchange rate API, only GET method required. This GET method should look like `/api/v1/{FROM_CURRENCY/{TO_CURRENCY}/{AMOUNT}`. 
The `/api` endpoint should be the context root. 
The API will return the following JSON:

    {
        "from_currency" : AED,
        "to_currency": GBP,
        "from_amount: 10.00,
        "to_amount": 2.07,
        "exchange_rate": 0.21
    }

The actual exchange rate will be obtained from providers like `currencylayer.com` (you'll need to maintain the keys for the providers).
The exchange rate for the from/to currencies should be maintained for an hour, i.e. update it every 60 mins.

## Rules and expected result:
  You cannot use Spring (unless if you haven't used it before)
2. You can use whatever language you like even Java.
3. You must provide your GitHub repo README which must include: design diagram and steps on how to run.
4. The runnable code must be available as a release from GitHub.
5. The name of your deployable/executable should be in this format:  exchange-rate-firstname.[jar, exe, bat etc]
6. You should be able to run (a provided) set of JMeter tests that all pass against your GET API.
