## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/tyl811/tyl811/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/tyl811/tyl811/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

<div id="app"></div>
<script src="https://unpkg.com/webamp"></script>
<script>
    const app = document.getElementById("app")
    const webamp = new Webamp();
    webamp.renderWhenReady(app);
</script>

.webamp-desktop {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: -1;
}
Get milkdrop on Galaxy s3 right now!

<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8" />
</head>

<body>
    <div id="app" style="height: 100vh">
        <!-- Webamp will attempt to center itself within this div -->
    </div>
    <script src="https://unpkg.com/webamp@1.5.0/built/webamp.bundle.min.js"></script>
    <script src="https://unpkg.com/butterchurn@2.6.7/lib/butterchurn.min.js"></script>
    <script src="https://unpkg.com/butterchurn-presets@2.4.7/lib/butterchurnPresets.min.js"></script>
    <script>
        const Webamp = window.Webamp;
        new Webamp({
            initialTracks: [{
                metaData: {
                    artist: "DJ Mike Llama",
                    title: "Llama Whippin' Intro"
                },
                // NOTE: Your audio file must be served from the same domain as your HTML
                // file, or served with permissive CORS HTTP headers:
                // https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS
                url: "https://cdn.jsdelivr.net/gh/captbaritone/webamp@43434d82cfe0e37286dbbe0666072dc3190a83bc/mp3/llama-2.91.mp3",
                duration: 5.322286
            }],
            __butterchurnOptions: {
                importButterchurn: () => Promise.resolve(window.butterchurn),
                getPresets: () => {
                    const presets = window.butterchurnPresets.getPresets();
                    return Object.keys(presets).map((name) => {
                        return {
                            name,
                            butterchurnPresetObject: presets[name]
                        };
                    });
                },
                butterchurnOpen: true
            },
            __initialWindowLayout: {
                main: { position: { x: 0, y: 0 } },
                equalizer: { position: { x: 0, y: 116 } },
                playlist: { position: { x: 0, y: 232 }, size: [0, 4] },
                milkdrop: { position: { x: 275, y: 0 }, size: [7, 12] }
            }
        }).renderWhenReady(document.getElementById('app'));
    </script>
</body>

</html>
