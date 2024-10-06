---
title: 'postgresql에 대한 학습'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Yoo-SH

# Author notes (optional)
author_notes:

date: '2013-07-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-10-06T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Hugo Blox Builder Conference*
publication_short: In *ICW*

abstract: 'PostgreSQL은 오픈 소스 관계형 데이터베이스 관리 시스템(RDBMS)으로, 다른 SQL 데이터베이스들과 비교할 때 다양한 장점과 차별화된 특징을 갖고 있습니다. 그럼에도 불구하고 몇 가지 단점도 존재하는데, 이를 고려해 PostgreSQL의 장단점과 다른 SQL 데이터베이스들과의 차이점을 중심으로 논의해 보겠습니다.

[PostgreSQL의 장점]

<오픈 소스이자 자유로운 사용>
PostgreSQL은 오픈 소스로 제공되며, 라이선스 비용 없이 사용 가능합니다. 이는 기업이나 개발자에게 비용 절감의 이점을 제공합니다. 뿐만 아니라, 오픈 소스이기 때문에 커뮤니티가 활발하게 참여하여 지속적으로 개선하고, 새로운 기능들을 추가합니다.


<확장성(Extensibility)>
PostgreSQL은 매우 확장성이 높은 시스템으로, 사용자 정의 함수를 작성하거나 새로운 데이터 타입, 인덱스 방법, 언어 확장을 추가할 수 있습니다. 예를 들어, 확장 모듈을 통해 JSON, XML, Hstore 같은 비구조화 데이터를 저장하고 관리할 수 있습니다. 이는 MongoDB와 같은 NoSQL 시스템과의 경계를 넘나드는 기능성을 제공합니다.


<ACID 지원과 강력한 트랜잭션 관리>
PostgreSQL은 트랜잭션의 원자성(Atomicity), 일관성(Consistency), 격리성(Isolation), 지속성(Durability)을 보장하는 ACID 특성을 완벽하게 준수합니다. 이로 인해 데이터 무결성과 안정성을 요구하는 시스템에 매우 적합합니다. 다수의 사용자와 복잡한 트랜잭션을 동시에 처리해야 하는 대규모 응용 프로그램에서 특히 유용합니다.


<SQL 표준의 높은 준수율>
PostgreSQL은 SQL 표준을 준수하는 측면에서 타의 추종을 불허합니다. SQL/JSON 기능부터 다양한 집합 연산과 복합 데이터 타입에 이르기까지, PostgreSQL은 최신 SQL 표준을 지속적으로 반영하고 확장합니다. 다른 데이터베이스들이 종종 자사 고유의 확장을 사용하여 표준에서 벗어나는 경우가 많지만, PostgreSQL은 가능한 한 표준을 유지하려고 합니다.


<풍부한 데이터 타입 지원>
PostgreSQL은 다른 RDBMS에 비해 많은 데이터 타입을 기본적으로 지원합니다. 숫자, 문자, 날짜와 같은 일반적인 데이터 타입 외에도, JSON, 배열, 범위 데이터 타입 등 복잡한 구조의 데이터 타입을 저장할 수 있는 기능을 제공합니다. 이 때문에 구조화된 데이터와 비구조화된 데이터를 동시에 다루어야 하는 현대의 애플리케이션 환경에서 더욱 유리합니다.



<다양한 인덱싱 방법 제공>
PostgreSQL은 B-tree, Hash, GIN(Generalized Inverted Index), GIST(Generalized Search Tree), SP-GiST 등 다양한 인덱스 구조를 제공합니다. 이 덕분에 다양한 검색 요구사항에 맞춰 성능을 최적화할 수 있으며, 복잡한 쿼리 성능을 향상시킬 수 있습니다. 특히, GIN 인덱스는 대규모 텍스트 데이터나 JSONB 필드를 검색하는 데 유용합니다.



<다중 버전 동시성 제어(MVCC)>
PostgreSQL은 다중 버전 동시성 제어(MVCC)를 통해 트랜잭션 간의 충돌을 최소화하면서도 높은 성능을 유지합니다. 이는 데이터베이스가 여러 사용자가 동시에 데이터를 읽거나 쓸 때, 각 트랜잭션이 고유한 데이터 스냅샷을 가지도록 하여 트랜잭션 격리 수준을 높이는 데 기여합니다.



<NoSQL 기능 통합>
PostgreSQL은 관계형 데이터베이스이면서도 NoSQL의 특성을 통합한 하이브리드 시스템입니다. 예를 들어, JSON과 JSONB 데이터 타입을 통해 문서 지향 데이터 모델링이 가능하며, 비정형 데이터를 처리할 수 있습니다. 이를 통해 MongoDB와 같은 전통적인 NoSQL 데이터베이스의 기능을 일부 흡수합니다.



<리플리케이션 및 고가용성>
PostgreSQL은 스트리밍 리플리케이션과 논리 리플리케이션을 지원하여 데이터베이스의 고가용성을 보장합니다. 이를 통해 마스터-슬레이브 리플리케이션 구조를 구축할 수 있으며, 장애 복구 및 데이터 백업에도 유리한 구조를 제공합니다.



[PostgreSQL의 단점]


<초기 설정 및 학습 곡선>
PostgreSQL은 기능이 풍부한 만큼 설정과 최적화가 복잡할 수 있습니다. 기본적인 사용은 쉽지만, 대규모 시스템에서 성능을 최적화하거나 특정 기능을 활용하려면 많은 학습이 필요합니다. 특히, 확장성 있는 환경에서 최적의 성능을 유지하기 위해서는 상당한 경험과 지식이 요구됩니다.


<복잡한 확장성 문제>
수평적 확장(샤딩)을 기본적으로 지원하지 않기 때문에, 대규모 데이터베이스에서 성능을 확장하는 것이 어려울 수 있습니다. 반면, MongoDB나 Cassandra 같은 NoSQL 데이터베이스는 샤딩 기능을 기본적으로 제공하여 데이터를 쉽게 분산 처리할 수 있습니다. PostgreSQL의 경우 이러한 수평 확장은 외부 도구나 설정이 필요합니다.



<비교적 느린 쓰기 성능>
PostgreSQL은 복잡한 트랜잭션을 처리하는 데 강력하지만, 그로 인해 많은 쓰기 작업에서 MySQL 같은 다른 데이터베이스보다 느릴 수 있습니다. 이는 고성능 쓰기 작업이 필요한 애플리케이션에는 부적합할 수 있습니다. 트랜잭션의 무결성을 보장하기 위해 다양한 보호 장치와 검사 과정을 거치기 때문에 일부 경우 쓰기 성능이 제한됩니다.



<상대적으로 작은 커뮤니티와 지원>
MySQL과 같은 데이터베이스에 비하면 PostgreSQL의 커뮤니티 크기는 상대적으로 작을 수 있습니다. 이는 상업적인 지원이 부족하거나 특정 문제가 발생했을 때 해결하기 어려울 수 있다는 단점으로 작용할 수 있습니다. 물론, PostgreSQL도 활성화된 커뮤니티와 다양한 온라인 리소스를 제공하지만, 상업적인 지원을 찾는 기업에는 불리할 수 있습니다.



<수직적 확장 비용>
PostgreSQL은 메모리와 CPU 자원에 대한 요구사항이 높을 수 있습니다. 이는 트랜잭션 처리에 있어 고성능을 유지하기 위한 구조적인 특성 때문인데, 대규모 데이터를 처리할 때는 추가적인 하드웨어 리소스가 필요할 수 있습니다.


주제 3:[다른 SQL 데이터베이스와의 차별화]


<PostgreSQL vs. MySQL>
MySQL은 단순성과 빠른 성능을 제공하는 반면, PostgreSQL은 기능의 풍부함과 표준 준수에 중점을 둡니다. MySQL은 읽기 성능이 뛰어나고 빠르게 시작할 수 있는 반면, PostgreSQL은 복잡한 트랜잭션과 데이터 무결성을 요구하는 애플리케이션에 더 적합합니다. 또한, MySQL은 기본적으로 트랜잭션을 다루는 방식에서 다소 제한적일 수 있지만, PostgreSQL은 완전한 ACID 준수와 MVCC를 통해 더 안정적이고 일관된 트랜잭션 관리를 제공합니다.



<PostgreSQL vs. MariaDB>
MariaDB는 MySQL의 포크(fork)로, MySQL과의 호환성을 유지하면서 성능과 확장성을 개선하려고 합니다. 그러나 PostgreSQL은 MySQL이나 MariaDB와는 다르게 강력한 확장성과 복잡한 데이터 구조를 처리할 수 있는 기능을 제공합니다. 특히 PostgreSQL은 JSON과 같은 비구조화 데이터를 효율적으로 다룰 수 있는 기능이 더욱 뛰어납니다.


<PostgreSQL vs. Oracle DB>
Oracle DB는 상업적으로 지원되는 강력한 데이터베이스 시스템으로, 특히 대규모 엔터프라이즈 환경에서 사용됩니다. PostgreSQL은 Oracle과 비슷한 기능을 제공하지만, 오픈 소스이기 때문에 비용 측면에서 크게 유리합니다. 다만, Oracle은 고성능과 강력한 기술 지원을 제공하지만 PostgreSQL은 커뮤니티 기반의 지원과 일부 복잡한 설정에서 부족할 수 있습니다.'

 
# Summary. An optional shortened abstract.
summary: postsql이 가진 장단점에 얘기하고자 합니다.

tags:
  - Postgresql

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org


# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/ko/%EC%82%AC%EC%A7%84/silver-laptop-computer-on-black-table-WB3ujiKLJwQ)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---
