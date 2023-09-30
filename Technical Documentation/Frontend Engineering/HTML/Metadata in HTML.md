The [head](https://developer.mozilla.org/en-US/docs/Glossary/Head) of an HTML document is the part that is not displayed in the web browser when the page is loaded. It contains information such as the page [`<title>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title), links to [CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS) (if you choose to style your HTML content with CSS), links to custom favicons, and other metadata (data about the HTML, such as the author, and important keywords that describe the document). Web browsers use information contained in the [head](https://developer.mozilla.org/en-US/docs/Glossary/Head) to render the HTML document correctly.

#### Adding a title
The [`<title>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title) element is metadata that represents the title of the overall HTML document (not the document's content.)

#### Metadata: the <meta> element
Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document — the [`<meta>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta) element.
```html
<meta charset="utf-8" />
```
Many `<meta>` elements include `name` and `content` attributes:

- `name` specifies the type of meta element it is; what type of information it contains.
- `content` specifies the actual meta content.
```html
<meta name="author" content="Chris Mills" />
<meta
  name="description"
  content="The MDN Web Docs Learning Area aims to provide
complete beginners to the Web with all they need to know to get
started with developing websites and applications." />
```
**Note:** Many `<meta>` features just aren't used anymore. For example, the keyword `<meta>` element (`<meta name="keywords" content="fill, in, your, keywords, here">`) — which is supposed to provide keywords for search engines to determine relevance of that page for different search terms — is ignored by search engines, because spammers were just filling the keyword list with hundreds of keywords, biasing results.
[Open Graph Data](https://ogp.me/) is a metadata protocol that Facebook invented to provide richer metadata for websites. In the MDN Web Docs sourcecode, you'll find this:
```html
<meta
  property="og:image"
  content="https://developer.mozilla.org/mdn-social-share.png" />
<meta
  property="og:description"
  content="The Mozilla Developer Network (MDN) provides
information about Open Web technologies including HTML, CSS, and APIs for both websites
and HTML Apps." />
<meta property="og:title" content="Mozilla Developer Network" />
```
One effect of this is that when you link to MDN Web Docs on Facebook, the link appears along with an image and description: a richer experience for users.
Twitter also has its own similar proprietary metadata called [Twitter Cards](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards), which has a similar effect when the site's URL is displayed on twitter.com. For example:
```html
<meta name="twitter:title" content="Mozilla Developer Network" />
```

#### Adding custom icons to your site
