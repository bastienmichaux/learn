# Html

## Document character set

```html
<meta charset="utf-8">
```

When a HTML document is downloaded, the browser first try to determine the character set from the server's `Content-Type` HTTP response header. The browser generally prefers this character set to the one specified in the document ($TODO check). If you cannot control the headers your server sends, declare the character set in the HTML document.

See [Google's XSS vulnerability](http://shiflett.org/blog/2005/googles-xss-vulnerability)

## Anchors

### "email" anchor

```html
<a href="mailto:foo@bar.be">My email</a>
```
