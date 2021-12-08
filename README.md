# growcommerce-demo

A demo app installed on [growcommerce.app](https://www.growcommerce.app).

This source code is used in Goaddon's introduction video series. It is a MVP in the truest sense of the word, put together with only a few days of work. Before you decide to fork this project into production, please note that a lot of optimization is due.

This repository uses the Javascript library [EasyQRCodeJS](https://github.com/ushelp/EasyQRCodeJS). It is available through the jsdelivr CDN at:

```
https://cdn.jsdelivr.net/npm/easyqrcodejs@4.4.7/dist/easy.qrcode.min.js
```

This URL can be registered on your Goaddon account under [GOEXPLORE > ASSETS](https://goaddon.com/en/addons/5bb227d283c3360abe01e036/manage#page=assets).

The repository also needs access to two secrets from the Gofetch addon. The secrets can be created from your Goaddon account under [GOEXPLORE > SECRETS](https://goaddon.com/en/addons/5bb227d283c3360abe01e036/manage#page=secrets), and in both cases you need to copy the encoded version.

- Your `gofetch_shop_api_token` can be found in [GOFETCH > SHOP API](https://goaddon.com/en/addons/5b9ff6463ab42f43522b30cf/manage#page=shop_api)
- Your `gofetch_webhook_token` can be found in [GOFETCH > WEBHOOKS](https://goaddon.com/en/addons/5b9ff6463ab42f43522b30cf/manage#page=webhooks)

While you are on [GOFETCH > WEBHOOKS](https://goaddon.com/en/addons/5b9ff6463ab42f43522b30cf/manage#page=webhooks) you should register your webhook address, which for this repository is:

```
https://www.example.com/gofetch_events
```

where you should replace `https://www.example.com/` with the URL of your own website.

The repository communicates with the shipping platform [Shipmondo](https://shipmondo.com/). To enable the communication with their API you should create an account there and generate an API token. This token should be saved in [GOEXPLORE > SECRETS](https://goaddon.com/en/addons/5bb227d283c3360abe01e036/manage#page=secrets) as `shipmondo_api_token`.