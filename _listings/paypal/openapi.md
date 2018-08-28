swagger: "2.0"
x-collection-name: PayPal
x-complete: 1
info:
  title: PayPal (Sandbox)
  description: bring-payments-to-apps-mobile-and-social-with-adaptive-payments-bsandbox-api-b
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