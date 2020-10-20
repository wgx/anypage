# ☁️📄 [Anypage](https://wgx.github.io/anypage/)

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

Why should those other CMSs get all the fancy toys? Anypage has got a [WYSIWYG editor](https://wgx.github.io/anypage/editor) now.
