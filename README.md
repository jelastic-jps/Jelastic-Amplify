# NGINX Amplify Add-On

**NGINX Amplify** is monitoring tool that provides comprehensive analytics, troubleshooting, customizable alerts and appropriate recommendations to improve PHP applications performance.

With NGINX Amplify, you can monitor your application and proactively identify problems before they affect your users - namely, it allows to:
* **analyze configurations** to get recommendations on possible improvements
* **aggregate metrics** on CPU usage, traffic, HTTP errors, etc
* **get alerts** if something goes wrong with the application delivery
* **plan capacities**, required for your application

> **Note:** This add-on can be applied only to the environments with NGINX-PHP application server.

For more information about [Jelastic Add-Ons](https://github.com/jelastic-jps/jpswiki/wiki/Jelastic-Addons) and their usage, refer to the linked guide.

## How to Install NGINX Amplify Add-On

Before installing the NGINX Amplify add-on, you need to create an account at official Amplify [website](https://amplify.nginx.com/signup/) and get your own **API Key** (from the either start page or account settings) for the proper monitoring integration.

![Amplify Account Settings](/images/amplify-account-settings.png)

Then copy the link to _**manifest.json**_ from the repository file list above, enter your Jelastic dashboard and [import](https://docs.jelastic.com/environment-import) the copied URL.

![NGINX Amplify Install](/images/nginx-amplify-install.png)

> **Tip:** Alternatively, you can locate and install this add-on from [Jelastic Marketplace](https://docs.jelastic.com/marketplace#add-ons).

In the installation dialog box, provide the following details and click **Install**:
* _**API key**_ - your Amplify account API key
* _**Environment name**_ - an environment the Amplify add-on should be applied to
* _**Nodes**_ - NGINX-PHP application server should be chosen (is fetched automatically upon selecting the environment)

When the installation is completed, return to your Amplify dashboard and wait a minute for the data on your NGINX instance to be collected and visualized.

![NGINX Amplify Monitoring](/images/nginx-amplify-monitoring.png)

Now, at Amplify dashboard, you are able to monitor your server and proactively detect & fix issues, related to running and scaling NGINX-based PHP applications. To find more information on Amplify usage and its capabilities, refer to the [official documentation](https://amplify.nginx.com/docs/guide-introduction.html).
