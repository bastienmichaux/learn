# Html

## Document character set

```html
<meta charset="utf-8">
```

When a HTML document is downloaded, the browser first try to determine the character set from the server's `Content-Type` HTTP response header. This character set is generally prefered by the browser to the character set specified in the document. If you cannot control the headers your server sends, declaring the character set in the HTML document is the best option.

See [Google's XSS vulnerability](http://shiflett.org/blog/2005/googles-xss-vulnerability)

## Anchors

### "email" anchor

```html
<a href="mailto:foo@bar.be">My email</a>
```
