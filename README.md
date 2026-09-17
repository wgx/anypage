# ☁️📄 [Anypage](https://wgx.github.io/anypage/)

## V 0.2.0 - September 2026 Update!

On-demand web pages defined by JSON in the URL

## The URL is the content.

The page is described by a JSON object with these attributes:

```json
{
  "h1":"This is the title",
  "h2":"This is the subtitle",
  "body":"The quick brown fox jumped over the lazy dog, the quick brown fox jumped over the lazy dog.",
  "footer":"This is the footer"
}
```

Encode the JSON as base64 and append to the URL, [like this](https://wgx.github.io/anypage/?eyJoMSI6IlRoaXMgaXMgdGhlIHRpdGxlIiwiaDIiOiJUaGlzIGlzIHRoZSBzdWJ0aXRsZSIsImJvZHkiOiJUaGUgcXVpY2sgYnJvd24gZm94IGp1bXBlZCBvdmVyIHRoZSBsYXp5IGRvZywgdGhlIHF1aWNrIGJyb3duIGZveCBqdW1wZWQgb3ZlciB0aGUgbGF6eSBkb2cuIiwiZm9vdGVyIjoiVGhpcyBpcyB0aGUgZm9vdGVyIn0=).

## ✏️ [Editor](https://wgx.github.io/anypage/editor)

Why should those other (real) CMSs get all the fancy toys? Anypage has got an [editor](https://wgx.github.io/anypage/editor) now.

## Limits and privacy

The content is encoded in the URL as UTF-8 JSON followed by Base64. Base64 is an encoding, not encryption: anyone with the link can decode the content, and the URL may be stored in browser history, server logs, referrer data, or link previews.

URLs have practical length limits. Large pages may fail in browsers, proxies, QR codes, or sharing services, so Anypage is intended for short text rather than documents or secrets. Invalid or corrupted payloads are rejected and shown as an error instead of being rendered.

Custom content is rendered as text. HTML, scripts, and event-handler markup in the JSON are displayed literally and are not interpreted.

## Development notes

The viewer and editor are static HTML pages. Tailwind CSS, Google Fonts, and QRious are loaded from CDNs; QRious is pinned with Subresource Integrity. A production deployment should consider self-hosting these assets and adding a Content Security Policy.

## 💵 Chuck a tip my way

[Buy me a coffee](https://ko-fi.com/wllgrnt)
