# Loading a Font

To load a font using the **Shaughnessy CDN**, create a `<link>` to the css stylesheet for the font you'd like to use.

–––––

For example, to load the font "[Wayfinder](https://craftwork.design/downloads/wayfinder/)" from the [Craftwork Design Company](https://craftwork.design/) & [Connary Fagen](https://craftwork.design/author/connary-fagen/), create a `<link>` like this:

{% code overflow="wrap" %}
```html
<link href="https://cdn.emmetts.dev/fonts/wayfinder/stylesheet.css" rel="stylesheet" type="text/css" />
```
{% endcode %}

Then, use the font like this:

<pre class="language-css"><code class="lang-css">p {
<strong>    font-family: "Wayfinder CF";
</strong>    font-size: 50px;
}</code></pre>
