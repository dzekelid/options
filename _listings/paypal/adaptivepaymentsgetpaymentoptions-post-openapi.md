---
swagger: "2.0"
x-collection-name: PayPal
x-complete: 0
info:
  title: Paypal Get Payment Options
  description: You use the GetPaymentOptions API operation to retrieve the payment
    options passed with the SetPaymentOptionsRequest.
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptivePayments/GetPaymentOptions:
    post:
      summary: Get Payment Options
      description: You use the GetPaymentOptions API operation to retrieve the payment
        options passed with the SetPaymentOptionsRequest.
      operationId: AdaptivePayments.GetPaymentOptions.post
      x-api-path-slug: adaptivepaymentsgetpaymentoptions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/SetPaymentOptions:
    post:
      summary: Set Payment Options
      description: "You use the SetPaymentOptions API operation to specify settings
        for a payment of the actionType CREATE. \n\t\t\t\t\tThis actionType is specified
        in the PayRequest message."
      operationId: AdaptivePayments.SetPaymentOptions.post
      x-api-path-slug: adaptivepaymentssetpaymentoptions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---