# Filemoon Extractor API

> **NOTE:** The source code for this project is contained in a **Private Repository**.

## 🔴 Live Demo
**Developing Site:** [https://filemoon-extractor.netlify.app/](https://filemoon-extractor.netlify.app/)

---

## ⚡ API Documentation

### Get Video Information
Extracts video sources and metadata from a Filemoon URL.

**Endpoint:**
`GET /api/url`

**Query Parameters:**
- `url` (required): The Filemoon URL to bypass (e.g., `https://bysezoxexe.com/e/...`)

**Example Request:**
```http
GET https://filemoon-extractor.netlify.app/api/url?url=https://bysezoxexe.com/e/ohbcoeb7m57l
```

**Example Response:**
```json
{
  "success": true,
  "data": {
    "title": "Video Title",
    "image": "https://poster-image-url.jpg",
    "duration": 1234,
    "sources": [
      {
        "file": "https://m3u8-url.com/playlist.m3u8",
        "type": "hls",
        "label": "Auto"
      }
    ],
    "tracks": []
  },
  "debug": {
    "executionTime": "120ms"
  }
}
```

---

## 👨‍💻 Creator Info

```json
{
  "creator": "Kawdhitha Nirmal",
  "CodeXSL": "Developer",
  "contact": "https://github.com/codexsldev"
}
```

&copy; 2026 CodeXsl Dev. All rights reserved.
