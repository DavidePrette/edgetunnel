# 🚀 edgetunnel 2.0
![Admin Dashboard](./img.png)

- **Latest edgetunnel Tutorial**: https://www.youtube.com/watch?v=tKe9xUuFODA ***Must watch! Must watch! Must watch!!!***
- **Error 1101 Explanation**: https://www.youtube.com/watch?v=r4uVTEJptdE

- Telegram Group: [@CMLiussss](https://t.me/CMLiussss)

## ⚠️ Disclaimer

This disclaimer applies to the "edgetunnel" project on GitHub (hereinafter referred to as "this project"), project link: https://github.com/cmliu/edgetunnel .

### Purpose
This project is designed and developed solely for educational, research, and security testing purposes. It aims to provide security researchers, academics, and technology enthusiasts with a tool to explore and practice network communication technologies.

### Legality
When downloading and using the code of this project, you must comply with the laws and regulations applicable to you. You are responsible for ensuring that your conduct complies with the legal framework, regulations, and other relevant provisions of your region.

### Disclaimer
1. As the **secondary developer** of this project (hereinafter referred to as the "author"), I **cmliu** emphasize that this project should only be used for legal, ethical, and educational purposes.
2. The author does not endorse, support, or encourage any form of illegal use. If the project is found to be used for any illegal or unethical activities, the author will strongly condemn it.
3. The author is not responsible for any illegal activities conducted by any person or organization using the project code. All consequences arising from the use of this project's code are borne by the user.
4. The author is not responsible for any direct or indirect damages that may be caused by using this project's code.
5. To avoid any unexpected consequences or legal risks, users should delete the code within 24 hours after using this project's code.

By using this project's code, you agree to understand and accept all terms of this disclaimer. If you do not agree with these terms, you should immediately stop using this project.

The author reserves the right to update this disclaimer at any time without notice. The latest version of the disclaimer will be published on this project's GitHub page.

## 🔥 Risk Warning
- Submit false node configurations to subscription services to avoid exposing node configuration information.
- Alternatively, you can choose to deploy the [WorkerVless2sub Subscription Generation Service](https://github.com/cmliu/WorkerVless2sub) yourself, so you can take advantage of the subscription generator's convenience.
   
## 💡 How to Use?
### ⚙️ Workers Deployment Method [Video Tutorial](https://www.youtube.com/watch?v=tKe9xUuFODA&t=191s)

<details>
<summary><code><strong>「 Workers Deployment Text Tutorial 」</strong></code></summary>

1. Deploy CF Worker:
   - Create a new Worker in the CF Worker console.
   - Copy the contents of [worker.js](https://github.com/cmliu/edgetunnel/blob/main/_worker.js) to the Worker editor.
   - In the `Settings` tab on the left, select `Variables` > `Add Variable`.
     Fill in the variable name as **ADMIN**, and the value as your admin password, then click `Save`.

2. Bind KV Namespace:
   - In the `Bindings` tab, select `Add Binding +` > `KV Namespace` > `Add Binding`, then select an existing namespace or create a new namespace to bind.
   - Fill in the variable name as **KV**, then click `Add Binding`.

3. Bind Custom Domain to Workers: 
   - In the workers console `Triggers` tab, click `Add Custom Domain` below.
   - Enter the subdomain that you have transferred to CF's domain name resolution service, for example: `vless.google.com`, then click `Add Custom Domain` and wait for the certificate to take effect.
   - **If you are a beginner, you can now take off directly without looking further down!!!**

4. Access the Admin Panel:
   - Visit `https://vless.google.com/admin` and enter your admin password to log in.

</details>

### 🛠 Pages Upload Deployment Method **Best Recommended!!!** [Video Tutorial](https://www.youtube.com/watch?v=tKe9xUuFODA&t=436s)

<details>
<summary><code><strong>「 Pages Upload File Deployment Text Tutorial 」</strong></code></summary>

1. Deploy CF Pages:
   - Download [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip) file and give it a Star!!!
   - In the CF Pages console, select `Upload Assets`, give your project a name, then click `Create Project`, then upload the [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip) file you downloaded and click `Deploy Site`.
   - After deployment is complete, click `Continue Processing Site`, then select `Settings` > `Environment Variables` > **Production** to define variables > `Add Variable`.
     Fill in the variable name as **ADMIN**, and the value as your admin password, then click `Save`.
   - Return to the `Deployments` tab, click `Create New Deployment` in the lower right corner, re-upload the [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip) file, then click `Save and Deploy`.

2. Bind KV Namespace:
   - In the `Settings` tab, select `Bindings` > `+ Add` > `KV Namespace`, then select an existing namespace or create a new namespace to bind.
   - Fill in the variable name as **KV**, then click `Save` and retry deployment.

3. Bind CNAME Custom Domain to Pages: [Video Tutorial](https://www.youtube.com/watch?v=LeT4jQUh8ok&t=851s)
   - In the Pages console `Custom Domains` tab, click `Set Custom Domain` below.
   - Enter your custom subdomain. Note that you should not use your root domain. For example:
     If the domain you are assigned is `fuck.cloudns.biz`, add the custom domain `lizi.fuck.cloudns.biz`;
   - As required by CF, return to your domain DNS service provider, add a CNAME record `edgetunnel.pages.dev` for the custom domain `lizi`, then click `Activate Domain`.
   - **If you are a beginner, after binding the custom domain to your pages, you can take off directly without looking further down!!!**
   
4. Access the Admin Panel:
   - Visit `https://lizi.fuck.cloudns.biz/admin` and enter your admin password to log in.

</details>

### 🛠 Pages GitHub Deployment Method [Video Tutorial](https://www.youtube.com/watch?v=tKe9xUuFODA&t=317s)

<details>
<summary><code><strong>「 Pages GitHub Deployment Text Tutorial 」</strong></code></summary>

1. Deploy CF Pages:
   - Fork this project on Github first and give it a Star!!!
   - In the CF Pages console, select `Connect to Git`, select the `edgetunnel` project, then click `Start Setup`.
   - On the `Set up builds and deployments` page below, select `Environment Variables (Advanced)` and `Add Variable`
     Fill in the variable name as **ADMIN**, and the value as your admin password, then click `Save and Deploy`.

2. Bind KV Namespace:
   - In the `Settings` tab, select `Bindings` > `+ Add` > `KV Namespace`, then select an existing namespace or create a new namespace to bind.
   - Fill in the variable name as **KV**, then click `Save` and retry deployment.

3. Bind CNAME Custom Domain to Pages: [Video Tutorial](https://www.youtube.com/watch?v=LeT4jQUh8ok&t=851s)
   - In the Pages console `Custom Domains` tab, click `Set Custom Domain` below.
   - Enter your custom subdomain. Note that you should not use your root domain. For example:
     If the domain you are assigned is `fuck.cloudns.biz`, add the custom domain `lizi.fuck.cloudns.biz`;
   - As required by CF, return to your domain DNS service provider, add a CNAME record `edgetunnel.pages.dev` for the custom domain `lizi`, then click `Activate Domain`.
   - **If you are a beginner, after binding the custom domain to your pages, you can take off directly without looking further down!!!**

4. Access the Admin Panel:
   - Visit `https://lizi.fuck.cloudns.biz/admin` and enter your admin password to log in.

</details>

## 🔑 Variable Explanation

| Variable | Example | Required | Notes |
|--------|---------|-|-----|
| ADMIN | `123456` |✅| Admin panel login password |
| KEY | `CMLiussss` |❌| Quick subscription key, visit `/CMLiussss` to quickly access the subscription. |
| HOST | `edt-pages.github.io` |❌| Force fixed disguise domain (supports multiple elements, use `newline` or `,` as separator) |
| UUID | `90cd4a77-141a-43c9-991b-08263cfe9c10` |❌| Force fixed UUID |
| PATH | `/` |❌| Force fixed path |
| PROXYIP | `proxyip.cmliussss.net:443` |❌| Change default built-in PROXYIP |
| URL | `https://cloudflare-error-page-3th.pages.dev` |❌| Homepage reverse proxy disguise (random settings can easily trigger anti-fraud, reverse proxy of blocked websites accelerates domain blocking) |
| GO2SOCKS5  | `blog.cmliussss.com`,`*.ip111.cn`,`*google.com` |❌| After setting `SOCKS5` or `HTTP` variables, you can set a list to force socks5 access (set to `*` to act as global proxy) |

## 🔧 Practical Tips
The nodes deployed by this project can use specified `PROXYIP` or `SOCKS5` through the node PATH (path) method!!!

- Specifying `PROXYIP` Example
   ```url
   /proxyip=proxyip.cmliussss.net
   /?proxyip=proxyip.cmliussss.net
   /proxyip.cmliussss.net (only for domains starting with 'proxyip.')
   ```

- Specifying `SOCKS5` Example
   ```url
   /socks5=user:password@127.0.0.1:1080
   /?socks5=user:password@127.0.0.1:1080
   /socks://dXNlcjpwYXNzd29yZA==@127.0.0.1:1080 (default to activate global SOCKS5)
   /socks5://user:password@127.0.0.1:1080 (default to activate global SOCKS5)
   ```

- Specifying `HTTP Proxy` Example
   ```url
   /http=user:password@127.0.0.1:1080
   /http://user:password@127.0.0.1:8080 (default to activate global SOCKS5)
   ```

## ⭐ Give It a Star
[![Stargazers over time](https://starchart.cc/cmliu/edgetunnel.svg?variant=adaptive)](https://starchart.cc/cmliu/edgetunnel)

## 💻 Compatible Clients
### Windows
   - [v2rayN](https://github.com/2dust/v2rayN)
   - clash.meta（[FlClash](https://github.com/chen08209/FlClash)，[mihomo-party](https://github.com/mihomo-party-org/mihomo-party)，[clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev)，[Clash Nyanpasu](https://github.com/keiko233/clash-nyanpasu)）
### iOS
   - Surge, Rocket
   - sing-box（[SFI](https://sing-box.sagernet.org/zh/clients/apple/)）
### Android
   - clash.meta（[ClashMetaForAndroid](https://github.com/MetaCubeX/ClashMetaForAndroid)，[FlClash](https://github.com/chen08209/FlClash)）
   - sing-box（[SFA](https://github.com/SagerNet/sing-box)）
### MacOS
   - clash.meta（[FlClash](https://github.com/chen08209/FlClash)，[mihomo-party](https://github.com/mihomo-party-org/mihomo-party)）


# 🙏 Special Thanks
### 💖 Sponsorship Support - Providing Cloud Servers to Maintain [Subscription Conversion Service](https://sub.cmliussss.net/)
- [NodeLoc](https://www.nodeloc.com/)
- [Alice](https://url.cmliussss.com/alice)
- [EasyLinks](https://www.vmrack.net?ref_code=5Zk7eNhbgL7)
- [ZMTO(VTEXS)](https://zmto.com/?affid=1532)

### 🛠 Open Source Code References
- [zizifn/edgetunnel](https://github.com/zizifn/edgetunnel)
- [3Kmfi6HP/EDtunnel](https://github.com/6Kmfi6HP/EDtunnel)
- [SHIJS1999/cloudflare-worker-vless-ip](https://github.com/SHIJS1999/cloudflare-worker-vless-ip)
- [Stanley-baby](https://github.com/Stanley-baby)
- [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR/tree/master/Clash/config)
- [Stock God](https://t.me/CF_NAT/38889)
- [Workers/Pages Metrics](https://t.me/zhetengsha/3382)
- [Free Whoring Brother](https://t.me/bestcfipas)
- [Mingyu](https://github.com/ymyuuu/workers-vless)
- [Alexandre Kojève](https://t.me/Enkelte_notif/784)：stallTCP v1.3
- [eooce](https://github.com/eooce/Cloudflare-proxy)
- [Sukka](https://ip.skk.moe/)