# CORSflare for Pandora
CORSflare, a lightweight JavaScript CORS Reverse Proxy designed to run in a Cloudflare Worker, configured to proxy Pandora APIs.

## Purpose
You'll need to use this (or an alternative) to use Epimetheus on the Web.

## How to install
To setup CORSflare within a Cloudflare Worker, follow these steps:
* **Download the latest CORSflare for Pandora version** from the CORSflare for Pandora GitHub page: you'll only need the `CORSflare.js` JavaScript file.
* **Login to Cloudflare**. If you don't have an account, create one: it's free 
and the basic plan will arguably be enough for most common scenarios, as it will grant 100.000 requests per day.
* **Navigate to the *Workers* section** using the top-level menu.
* **Create a new worker**. If it's the first time you do that, you'll also be asked to choose a subdomain, such as `domainName.workers.dev`.
The subdomain name will be appended to the worker's name to form the worker's FQDN, such as `workerName.domainName.workers.dev`.
* **Paste the CORSflare.js source code within the worker code**.

## Credits
CORSflare for Pandora is strongly based upon the following projects:
* [CORSflare](https://github.com/Darkseal/CORSflare) by [Darkseal](https://github.com/Darkseal) (MIT License)
* [worker-proxy](https://github.com/Berkeley-Reject/workers-proxy/) by [Berkeley-Reject](https://github.com/Berkeley-Reject) (MIT License)
* [cloudflare-cors-anywhere](https://github.com/Zibri/cloudflare-cors-anywhere) by [Zibri](https://github.com/Zibri) (MIT License)
