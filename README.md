# Sub-Store
> This project is still under active development.

![Icon](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F9c8f07d1-7290-4caf-8e63-941d7e2edc58%2Ffavicon.png?table=block&id=62595869-94d3-4c11-a4ce-d5c406264b46&width=250&userId=187ae477-568a-42e3-85f0-ad2f29911433&cache=v2)

Subscription manager for QX, Loon and Surge.

[Doc](https://www.notion.so/Sub-Store-6259586994d34c11a4ced5c406264b46) [文档](https://www.notion.so/Sub-Store-6259586994d34c11a4ced5c406264b46)


Core functionalities:
1. Conversion among various formats.
2. Subscription formatting.
3. Collect multiple subscriptions in one URL.
## 1. Subscription Conversion
### Supported Input Formats
- [x] SS URI
- [x] SSR URI
- [x] SSD URI
- [x] V2RayN URI
- [x] QX (SS, SSR, VMess, Trojan, HTTP)
- [x] Loon (SS, SSR, VMess, Trojan, HTTP)
- [x] Surge (SS, VMess, Trojan, HTTP)
- [x] Clash (SS, SSR, VMess, Trojan, HTTP)

### Supported Target Platforms
- [x] QX
- [x] Loon
- [x] Surge

## 2. Subscription Formatting
### Filtering
- [x] **Keyword filter**
- [x] **Discard keywords filter**
- [x] **Regex filter**
- [x] **Discard regex filter**
- [x] **Region filter**
- [x] **Type filter**
- [x] **Useless proxies filter**
- [x] **Script filter**

### Proxy Operations
- [x] **Set property operator**: set some proxy properties such as `udp`,`tfo`, `skip-cert-verify` etc.
- [x] **Flag operator**: add flags or remove flags for proxies.
- [x] **Sort operator**: sort proxies by name.
- [x] **Keyword sort operator**: sort proxies by keywords (fallback to normal sort).
- [x] **Keyword rename operator**: replace by keywords in proxy names.
- [x] **Keyword delete operator**: delete by keywords in proxy names.
- [x] **Regex rename operator**: replace by regex in proxy names.
- [x] **Regex delete operator**: delete by regex in proxy names.
- [x] **Script operator**: modify proxy by script.

### Development
Go to `backend` and `web` directories, install node dependencies:
```
npm install
```

1. In `backend`, run the backend server on http://localhost:3000

```
node sub-store.js
```

2. In`web`, start the vue-cli server
```
npm start
```

## LICENSE
This project is under the GPL V3 LICENSE.

## Acknowledgements
Special thanks to @KOP-XIAO for his awesome resource-parser. Please give a [star](https://github.com/KOP-XIAO/QuantumultX) for his great work!
