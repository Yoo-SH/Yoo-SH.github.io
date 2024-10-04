s---
title: 서버사이드랜더링에 대한 짧은 견해

event: 
event_url: 


summary: SSR(서버사이드 렌더링) 과정에서 겪었던 어려움을 짧게 설명하고자 합니다.
abstract: 'SSR을 구현하면서 어려웠던 점은 클라이언트와 서버 간의 상태 동기화를 적절히 관리하는 것이었던 것 같다. 서버에서 렌더링된 페이지를 클라이언트로 전달하는 과정에서 초기 로딩 속도를 최적화하는 것이 까다로웠고, 특히 SEO 최적화를 위해 콘텐츠를 빠르게 렌더링하면서도 사용자 인터랙션에 대한 반응성을 유지하는 데 고민이 많았던 것 같다. 또한, 서버와 클라이언트 모두에서 발생할 수 있는 오류 처리와 복잡한 빌드 설정 관리도 꾀나 까다로웠던거 같다.'



# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-10-04T13:00:00Z'
date_end: '2024-10-04T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2024-10-04T00:00:00Z'

authors:
  - admin

tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  caption: 'Image credit: [**Unsplash**]()'
  focal_point: Right

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
  - example
---
