# Loading a Font

To load a font using the **Shaughnessy CDN**, create a `<link>` to the css stylesheet for the font you'd like to use.

–––––

For example, to load the font "[Wayfinder](https://craftwork.design/downloads/wayfinder/)" by the [Craftwork Design Company](https://craftwork.design/) & [Connary Fagen](https://craftwork.design/author/connary-fagen/), create a `<link>` like this:

{% code overflow="wrap" %}
```html
<link href="https://cdn.emmetts.dev/fonts/wayfinder/stylesheet.css" rel="stylesheet" type="text/css" />
```
{% endcode %}

Then, use the font like this:

<pre class="language-css"><code class="lang-css"><strong>&#x3C;style>
</strong><strong>    p {
</strong>        font-family: "Wayfinder CF";
        font-size: 50px;
    }
&#x3C;/style></code></pre>

Again, for the font "[Anti-Design](https://craftwork.design/downloads/anti-design/)" by the [Craftwork Design Company](https://craftwork.design/) & [Endeavor Studio](https://craftwork.design/author/endeavour-studio/), implement the CDN like this:

```html
<head>
    
    <!-- CDN IMPLEMENTATION -->
    <link href="https://cdn.emmetts.dev/fonts/anti-design/stylesheet.css" rel="stylesheet" type="text/css" />
    
    <style>
        p {
            font-family: "Anti Design Endeavour";
            font-size: 50px;
        }
    </style>
    <!-- CDN IMPLEMENTATION -->

</head>
```
