# stock-predictor
Stock price prediction - simple model, deployed to server.

While it was running on an EC2 AWS instance, the command to query for stock forecasts was:

```
curl \
--header "Content-Type: application/json" \
--request POST \
--data '{"ticker":"MSFT", "days":7}' \
http://52.32.189.64:8000/predict
```


I also deployed the stock predictor on another server, that should still be online (2023-01-31):

```
curl \
--header "Content-Type: application/json" \
--request POST \
--data '{"ticker":"MSFT", "days":7}' \
http://5.189.182.28:8000/predict
```
