# anypage
On-demand web pages defined by JSON in the URL

## The URL is the content.

The page is described by a JSON object with these attributes:

```{ "h1":"This is the title", "h2":"This is the subtitle", "body":"The quick brown fox jumped over the lazy dog, the quick brown fox jumped over the lazy dog.", "footer":"This is the footer" }```

Encode the JSON as base64 and append to the URL.
