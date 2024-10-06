---
title: 🎓전북대학교 입학
summary: 2020년 전북대학교 입학에 대한 블로그 글입니다.(with SEO)
date: 2020-03-01
authors:
  - 유승현
tags:
  - 전북대학교
  - 유승현
  - 입학
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/ko/%EC%82%AC%EC%A7%84/%ED%97%A4%EB%93%9C%ED%8F%B0%EC%9D%84-%EC%93%B4-%EC%98%81%EB%A6%AC%ED%95%9C-%EC%8B%AD-%EB%8C%80-%EC%86%8C%EB%85%80%EA%B0%80-%EB%8B%A4%EB%A5%B8-%ED%95%99%EC%83%9D%EB%93%A4%EC%9D%98-%EB%B0%B0%EA%B2%BD%EC%97%90-%EB%8C%80%ED%95%9C-%EC%84%B8%EB%AF%B8%EB%82%98%EB%A5%BC-%EC%A4%80%EB%B9%84%ED%95%98%EB%8A%94-%EB%8F%99%EC%95%88-%EC%B1%85%EC%83%81%EC%97%90%EC%84%9C-%EB%A9%94%EB%AA%A8%EB%A5%BC-%ED%95%98%EA%B3%A0-%EC%9E%88%EB%8B%A4-zjnHrnc72ro)'
---

Easily manage your projects - create ideation mind maps, Gantt charts, todo lists, and more!

## Ideation

Hugo Blox supports a Markdown extension for mindmaps.

Simply insert a Markdown code block labelled as `markmap` and optionally set the height of the mindmap as shown in the example below.

Mindmaps can be created by simply writing the items as a Markdown list within the `markmap` code block, indenting each item to create as many sub-levels as you need:

<div class="highlight">
<pre class="chroma">
<code>
```markmap {height="200px"}
- Hugo Modules
  - Hugo Blox
  - blox-plugins-netlify
  - blox-plugins-netlify-cms
  - blox-plugins-reveal
```
</code>
</pre>
</div>

renders as

```markmap {height="200px"}
- Hugo Modules
  - Hugo Blox
  - blox-plugins-netlify
  - blox-plugins-netlify-cms
  - blox-plugins-reveal
```

## Diagrams

Hugo Blox supports the _Mermaid_ Markdown extension for diagrams.

An example **Gantt diagram**:

    ```mermaid
    gantt
    section Section
    Completed :done,    des1, 2014-01-06,2014-01-08
    Active        :active,  des2, 2014-01-07, 3d
    Parallel 1   :         des3, after des1, 1d
    Parallel 2   :         des4, after des1, 1d
    Parallel 3   :         des5, after des3, 1d
    Parallel 4   :         des6, after des4, 1d
    ```

renders as

```mermaid
gantt
section Section
Completed :done,    des1, 2014-01-06,2014-01-08
Active        :active,  des2, 2014-01-07, 3d
Parallel 1   :         des3, after des1, 1d
Parallel 2   :         des4, after des1, 1d
Parallel 3   :         des5, after des3, 1d
Parallel 4   :         des6, after des4, 1d
```

## Todo lists

You can even write your todo lists in Markdown too:

```markdown
- [x] Write math example
  - [x] Write diagram example
- [ ] Do something else
```

renders as

- [x] Write math example
  - [x] Write diagram example
- [ ] Do something else

## Did you find this page helpful? Consider sharing it 🙌
