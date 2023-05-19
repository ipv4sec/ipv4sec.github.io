---
title: "开发Hugo主题笔记"
date: 2023-04-26T23:04:02+08:00
draft: true
---

Hugo博客`config.json`配置
```json
{
  "title": "愿",
  "theme": "ahri",
  "disableKinds": [
    "taxonomy",
    "term",
    "sitemap",
    "section",
    "RSS",
    "404"
  ],
  "uglyurls": true,
  "permalinks": {
    "/": "/:filename"
  }
}
```


先执行 `hugo new theme ahri`
```
├─layouts
│  ├─partials
│  └─_default
└─static
```

1. `partials/ahri.html`组件
2. `_default/index.html`首页, `_default/single.html`单页, 内容`{{ partial "ahri.html" . }}`
3. `theme.toml`

```
name = "ahri"
min_version = "0.41.0"
description = "ahri theme description"
```


1. `<title>{{ .Site.Title }} {{ if .IsPage }} - {{.Title}} {{end}}</title>`
2. `<link rel="preload" href="assets/quicksand-v30-latin-regular.woff2" as="font" type="font/woff2" crossorigin>`

```
{{ if .IsHome }}
    <h1>所有文章:</h1>
    <section class="articles">
        <nav>
            <ol class="list-of-pages">
                {{  range .Pages }}
                <li><a href="{{.Permalink}}">[{{.Date.Format "2006/01/02" }}] {{.Title}}</a></li>
                {{  end  }}
            </ol>
        </nav>
    </section>
{{end}}
```

```
{{ if .IsPage }}
    <h1>{{.Title}}</h1>
    <section class="content">
        <div>
            {{.Content}}
        </div>
    </section>
{{end}}
```