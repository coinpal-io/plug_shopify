# How to start accepting crypto on Shopify

## Step 1: Go to your Shopify "Apps", click "Develop Apps" and "Create an App". Enter the App name and the developer's email

![](./images/shopify-1.png)

## Step 2: In Configuration tab, choose "Admin API integration". Give a "Read and Write" permission to Orders and Draft orders and click "Save"

![](./images/shopify-2.png)

## Step 3: Go to the API credentials tab and press "install app". Click "Reveal token once" in the module of Admin API access token

![](./images/shopify-3.png)

![](./images/shopify-4.png)

## Step 4: Go to your [CoinPal Account](https://portal.coinpal.io/#/admin/myAccount/Business) > My Account > My Store > choose/add store & click "Configuration" > click"Shopify" and fill the fields using the info from the Shopify API credentials tab (access token)

![](./images/shopify-51.png)

## Step 5: Click "Connect to Shopify"

![](./images/shopify-52.png)

## Step 6: Contact the administrator to obtain the distribution address
    Contact info:
    
    Email: tech@coinpal.io
    
    Telegram: @carter_crypto
    
    Click Install
 
![](./images/shopify-61.png)



## Step 7: Add Coinpal application in the custom template

![](./images/shopify-62.png)

![](./images/shopify-63.png)

![](./images/shopify-64.png)

![](./images/shopify-65.png)

![](./images/shopify-66.png)

## Step 8: Go to Shopify Settings > Payment Providers > Manual Payment Methods. Add a Custom payment method, ensure the Custom payment method name is the same as the one you set in the CoinPal > My Account  > My Store > Payment method name.Then activate it.

![](./images/shopify-91.png)

![](./images/shopify-9.png)

## Step 9: Go to Shopify Settings>Notifications>Order confirmation

![](./images/shopify-10.png)

    Click "Edit code"
    
![](./images/shopify-11.png)

    Replace the "Thank you for your purchase!" with the following code
     {% if financial_status=='paid' %}
        Thank you for your purchase!
     {% else %}
        Thank you for your order!
     {% endif %}
    
![](./images/shopify-12.png)

    Replace the "We're getting your order ready to be shipped. We will notify you when it has been sent." with the following code
     {% if financial_status=='paid' %}
        We're getting your order ready to be shipped. We will notify you when it has been sent.
     {% else %}
        You can continue to pay by clicking &quot;View your order&quot; below
     {% endif %}
     
![](./images/shopify-13.png)
