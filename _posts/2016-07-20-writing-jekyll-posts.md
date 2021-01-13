---
title: "Layout: Post with Table of Contents"
header:
  overlay_image: assets/images/sky.jpg
categories:
  - Layout
---

첫번째 줄

컨텐츠! 시작!

## link

- [Twitter Cards](https://dev.twitter.com/cards/overview)
- [custom sidebars](https://mmistakes.github.io/minimal-mistakes/docs/layouts/#sidebars)

## notice

notice
{: .notice}

notice--info
{: .notice--info}

notice--warning
{: .notice--warning}

notice--danger
{: .notice--danger}

## button

[button]({{ "/docs/quick-start-guide/" | relative_url }}){: .btn}

[button]({{ "/docs/quick-start-guide/" | relative_url }}){: .btn .btn--info}

[button]({{ "/docs/quick-start-guide/" | relative_url }}){: .btn .btn--success}

[button]({{ "/docs/quick-start-guide/" | relative_url }}){: .btn .btn--warning}

[button]({{ "/docs/quick-start-guide/" | relative_url }}){: .btn .btn--danger}

[button]({{ "/docs/quick-start-guide/" | relative_url }}){: .btn .btn--danger .btn--large}

## code block

```yaml
---
toc: true
---

```

```sh
$ sh
```

```css
.css {
  x: y;
}
```

```html
<a>html</a>
```

```js
console.log("js");
```

## test

test

<!-- <iframe id="iframe" class="iframe" src="https://htmlpreview.github.io/?https://github.com/imjhua/animation/blob/master/linear-gradient/index.html"></iframe> -->

## HTML Elements

Below is just about everything you'll need to style in the theme. Check the source code to see the many embedded elements within paragraphs.

## Body text

![Smithsonian Image]({{ site.url }}{{ site.baseurl }}/assets/images/sky.jpg)
{: .image-right}

## Tables

| Header1 | Header2 | Header3 |
| :------ | :-----: | ------: |
| cell1   |  cell2  |   cell3 |
| cell4   |  cell5  |   cell6 |

|----
| cell1 | cell2 | cell3 |
| cell4 | cell5 | cell6 |
|=====
| Foot1 | Foot2 | Foot3
{: rules="groups"}
