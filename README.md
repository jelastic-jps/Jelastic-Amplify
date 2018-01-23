# NGINX Amplify Add-On

**NGINX Amplify** is a monitoring tool that provides comprehensive analytics of server state, its troubleshooting, customizable alerts on inappropriate metrics changes and corresponding recommendations, helping you to improve performance of your NGINX-based PHP & Ruby applications or load balancer.

With NGINX Amplify, you can monitor your application and proactively identify problems before they affect your users - namely, it  allows to:
* **analyze configurations** to get recommendations on possible improvements
* **aggregate metrics** on CPU usage, traffic, HTTP errors, etc
* **get alerts** if something  goes wrong with the application delivery
* **plan capacities**, required for your application

> **Note:** This add-on can be applied only to the environments with NGINX web server or load balancer.

For more information about [Jelastic Add-Ons](https://github.com/jelastic-jps/jpswiki/wiki/Jelastic-Addons) and their usage, refer to the linked guide.

## How to Install NGINX Amplify Add-On

Before installing the NGINX Amplify add-on, you need to create an account at official Amplify [website](https://amplify.nginx.com/signup/) and get your own **API Key** (from the either start page or account settings) for the proper monitoring integration.

![Amplify Account Settings](/images/amplify-account-settings.png)

If you don’t have an environment with NGINX instance yet, click the _Deploy to Jelastic_ button below to automatically create such, with Amplify add-on being pre-installed to the NGINX-PHP application server. 

[![Deploy](https://github.com/jelastic-jps/git-push-deploy/raw/master/images/deploy-to-jelastic.png)](https://jelastic.com/install-application/?manifest=https://raw.githubusercontent.com/jelastic-jps/nginx-amplify/master/demo-nginx-php-fpm-amplify.jps)

In case you’d like to integrate this add-on into the existing environment, copy the link to _**manifest.jps**_ from the repository file list above, enter your Jelastic dashboard and [import](https://docs.jelastic.com/environment-import) the copied URL.

![NGINX Amplify Install](/images/nginx-amplify-install.png)

> **Tip:** Alternatively, you can locate and install this add-on within [Jelastic Marketplace](https://docs.jelastic.com/marketplace#add-ons).

In the installation dialog box, provide the following details and click on **Install**:
* _**API key**_ - your Amplify account API key
* _**Environment name**_ - an environment the Amplify add-on should be installed to
* _**Nodes**_ - a target environment layer (with either NGINX-based compute node or load balancer) the add-on should be installed to; herewith, all nodes within a layer will be adjusted

When the installation is completed, go to your Amplify dashboard and wait a minute for the data on your NGINX instance(s) to be collected and visualized.

![NGINX Amplify Monitoring](/images/nginx-amplify-monitoring.png)

Now, at Amplify dashboard, you are able to monitor your server and proactively detect & fix issues, related to your NGINX-based PHP & Ruby applications or load balancer running and scaling. To find more information on Amplify usage and its capabilities, refer to the [official documentation](https://amplify.nginx.com/docs/guide-introduction.html).
