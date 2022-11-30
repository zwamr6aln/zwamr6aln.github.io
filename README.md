
これは仮のGitHubPagesです。

[GitHub link](https://github.com/zwamr6aln/zwamr6aln.github.io)

[Pages link](https://zwamr6aln.github.io)

***

[html css](html_css)

[markdown ssg](markdown_ssg)

***

[sitemap.xml](sitemap.xml)

***

[testPlainPages](https://zwamr6aln.github.io/testPlainPages/)

***

[AppPRPages](https://zwamr6aln.github.io/AppPRPages/)


Jekyll メモ
--------------------
jekyll new PATH

jekyll new PATH --blank

jekyll build

jekyll clean

bundle exec jekyll serve

### markdownファイルにはfront-matterが必要
```
---
title: TITLE
description: PLACEHOLDER
layout: post
published: false
lang: ja
---
```

### \_config.yml
```
defaults:
  -
    scope:
      path: "" # an empty string here means all files in the project
    values:
      layout: "default"
```

```
plugins:
  - jekyll-seo-tag
  - jekyll-sitemap
```

### default.html
```
<html lang="{{ page.lang | default: site.lang | default: "en" }}">
```

```
{%- seo -%}
```

```
<body>
{{ content }}
</body>
```

#### jekyll-seo-tag
これでtitleとdescriptionは設定される
```
{%- seo -%}
```
