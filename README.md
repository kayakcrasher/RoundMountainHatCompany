# Round Mountain Hat Company

Responsive storefront for Hats, Clothing, and Accessories. Inspired by the outdoor retail structure of American Fetcher, with original branding and illustrations.

## Run locally (including Termux)

```sh
pkg install git python
 git clone https://github.com/kayakcrasher/RoundMountainHatCompany.git
cd RoundMountainHatCompany
python -m http.server 8080
```

Open http://localhost:8080. If you already cloned it, run `git pull` inside the repository instead.

## Connect Square

Edit `catalog.js` with your real products, prices, sizes, images, and each product's Square hosted checkout link in `squarePaymentUrl`. Optionally set `STORE_CONFIG.squareStoreUrl` to your Square Online store URL.

The Square link appears in the product dialog when configured. Square handles the actual checkout and final variation/quantity selection. The preview bag does not transfer to Square. This version does not synchronize Square inventory or create a combined cart checkout. Those features require a server integration and private Square credentials. Never put access tokens in these public files.

All current products, illustrations, and prices are sample content. Replace them before opening orders. The banner photograph shows the Highway 65 scenic overlook south of Marshall, Arkansas. Photo: Brandonrush, “Lower Boston Mountains near Marshall, AR,” Wikimedia Commons, CC0 public domain. Source: https://commons.wikimedia.org/wiki/File:Lower_Boston_Mountains_near_Marshall,_AR.jpg

## Hosting

Serve this folder with any static host. For GitHub Pages, select Settings → Pages → Deploy from a branch → main → / (root). No build or npm installation is needed.
