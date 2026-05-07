# How to start accepting crypto on Shopify

## Step 1: Go to your Shopify "Apps", click "Apps" and "Develop Apps". 

![](./images/shopify-1.png)

## Step 2: Create Apps.

click "Build apps in Dev Dashboard" and "Create app" and "Create"

![](./images/acc1.png)

![](./images/acc2.png)

![](./images/acc3.png)

click "Create version"

![](./images/acc40.png)

Select the required permissions, then click "Done" and "Release"

![](./images/acc48.png)

![](./images/acc5.png)

![](./images/acc6.png)

![](./images/acc7.png)

Save the "Client ID" and "Secret"; they will be required in Step 4 when connecting Coinpal to Shopify

![](./images/acc8.png)

## Step 3: Install app.

![](./images/acc9.png)

![](./images/acc10.png)

## Step 4: Go to your [CoinPal Account](https://portal.coinpal.io/#/admin/myAccount/Business) > My Account > My Store > choose/add store & click "Configuration" > click"Shopify" and fill the fields using the info from the Shopify API credentials tab (access token)

![](./images/shopify-41.png)

Enter the "Client ID" and "Secret" from Step 3, then click "Connect to Shopify"

![](./images/shopify-42.png)

## Step 5: After a successful connection, please click the "Get Installation Address" button displayed on the page. We will complete the review within 1 to 3 business days. Once approved, the installation address will be displayed.

Contact info:
   
Email: tech@coinpal.io

Telegram: @carter_crypto
    
![](./images/shopify-51.png)

![](./images/shopify-52.png)


## Step 6: Install the Shopify App

Click "Installation link" 

![](./images/shopify-53.png)

Click "Install"
 
![](./images/shopify-61.png)


## Step 7: Add Coinpal application in the custom template

![](./images/shopify-62.png)

![](./images/shopify-63.png)

![](./images/shopify-64.png)

Add application
![](./images/shopify-65.png)

Click to "Save"
![](./images/shopify-66.png)

## Step 8: Go to Shopify Settings > Payment Providers > Manual Payment Methods. Add a Custom payment method, ensure the Custom payment method name is the same as the one you set in the CoinPal > My Account  > My Store > Payment method name.Then activate it.

![](./images/shopify-81.png)

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
        You can continue to pay by clicking "View your order" below.
     {% endif %}
     
![](./images/shopify-13.png)
