# 📦 QR Code Generator API

Generate high-performance QR codes via a simple RESTful API. Deployed serverlessly on Vercel for blazing-fast response times.

## 🚀 Live Demo

Explore the API live at [qrsapi.vercel.app][qrsapi-url]

📘 API Documentation

🔗 Base URL

`https://qrsapi.vercel.app`

---

### Build with

[![JavaScript][js]][js-docs]
[![Node.js][node]][node-docs]
[![Tailwind CSS][tailwind]][tailwind-docs]
[![Vercel][vercel]][vercel-docs]

---

### 📥 GET /api/qr/generate

Generate a QR code via query parameters.

Example:

```
GET https://qrsapi.vercel.app/api/qr/generate?text=Hello%20World&size=200&margin=1&format=png
```
```html
<img src="https://qrsapi.vercel.app/api/qr/generate?text=Hello%20World&size=200&margin=1&format=png" alt="QR Code" />
```
Preview:

[![Preview][qrsapi-img]][qrsapi-url]

**Query Parameters:**

| Parameter |  Type  | Description |
| --------- | ------ | ----------- |
| text      | string | Text to encode in QR |
| size      | number | Size in pixels (default: 200) |
|  format   | string | png or svg|
| margin    | number | size in pixel (default: 1)|
---

### 📤 POST /api/qr/generate

Generate a QR code with custom options via JSON payload.

Headers:

```
Content-Type: application/json
```

Body Example:

```json
{
  "text": "Hello World",
  "size": 200,
  "margin": 1,
  "format": "png",
  "color": "#FF0000",
  "background": "#FFFFFF"
}
```

---

### 📊 GET /api/qr/info

Returns API usage information and metadata.

---

### ❤️ GET /health

Health check endpoint to verify server status.

---

### 🛠 Tech Stack

-   Serverless Functions (Vercel)
-   Node.js
-   QR Code generation library

📄 License

[![License][mit]][mit-license]

---

👀 Readme

[![README][readme]][repo]

---

Made by [Nine12](https://fqnlst.vercel.app) for QRsAPI

[mit]: https://img.shields.io/badge/License-MIT-2ea44f?logo=github&logoColor=white&style=for-the-badge
[js]: https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=000&style=for-the-badge
[node]: https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=fff&style=for-the-badge
[tailwind]: https://img.shields.io/badge/Tailwind_CSS-06B6D4?logo=tailwindcss&logoColor=fff&style=for-the-badge
[vercel]: https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white&style=for-the-badge
[readme]: https://img.shields.io/badge/README-md-blue?style=for-the-badge&logo=markdown&logoColor=white
[qrsapi-img]: https://qrsapi.vercel.app/api/qr/generate?text=Hello%20World&size=200&margin=1&format=png

[repo]: ./README.md
[js-docs]: https://developer.mozilla.org/en-US/docs/Web/JavaScript
[node-docs]: https://nodejs.org
[tailwind-docs]: https://tailwindcss.com
[vercel-docs]: https://vercel.com/docs
[mit-license]: https://opensource.org/licenses/MIT
[qrsapi-url]: https://qrsapi.vercel.app



