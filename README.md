# 🚀 astro Codepen Embed

This [Astro](https://astro.build/) component makes it easy to add and customize a [CodePen.io](https://codepen.io) embed.

Currently it's __very__ early in development.

Pull requests and/or feature requests are very welcome!

## How To Use

In any of your Astro pages, import Astro CodePen Embed and then use the component inside
the `<body>` section of your HTML:

```jsx
---
import { CodePen } from 'astro-codepen-embed'
---

<html lang="en">
	<head>
		// ... 	
	</head>

	<body>
        <CodePen 
            username="sarah11918"
            slug="rNwNEBL"
            title="5-pin Bowling Game"
            tabs="html, default"
            height="300px"
                />
		// ... rest of body
	</body>
</html>
```

## Supported Props

Propname | Type | Description
------------ | ------------- | -------------
user | string | The username of the account. (required)
slug | string | The slug that identifies the pen. (required)
slug | string | The title of the pen. (required)
height | string | The default if not specified is 300px.
tabs | string | Pens on CodePen show HTML, CSS and JavaScript as well as a Result (preview) tab all at once. Embeds show some tabs, while allowing you to click to show other tabs. The default behaviour is to show HTML and result in a 2-pane window, but this can be configured by adding your preferred tabs comma-separated as a string. 

You can find the user and slug strings from the URL of any pen as follows:
 https://codepen.io/{user}/pen/{slug}



## Acknowledgements

Astro SEO is _heavily_ inspired by [Astro SEO](https://github.com/jonasmerlin/astro-seo)
Thanks Jonas! ❤️
