# stock-predictor
Stock price prediction - simple model, deployed to server.

Because I couldn't launch instances via the Fourthbrain AWS account, I deployed the model on another server. To get predictions, use:

```
curl \
--header "Content-Type: application/json" \
--request POST \
--data '{"ticker":"MSFT", "days":7}' \
http://5.189.182.28:8000/predict
```
