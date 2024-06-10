# 생성형 AI를 활용한 블로그 콘텐츠 자동화 솔루션

## 개요
이 프로젝트는 ChatGPT-4를 활용하여 고품질의 블로그 콘텐츠를 자동으로 생성하고, 이를 블로그에 자동으로 포스팅하는 시스템을 개발하는 것을 목표로 합니다. 이 솔루션은 특히 지하철 관련 정보 제공에 최적화되어 있으며, 실시간으로 데이터를 수집하고 분석하여 최신 정보를 제공합니다.

## 주요 기능
- **자동화된 글쓰기**: AI 기반으로 블로그 글을 자동으로 작성합니다.
- **SEO 최적화**: 검색 엔진 최적화를 통해 더 많은 트래픽을 유도합니다.
- **비용 절감**: 기존 브랜딩 블로그 관리 비용보다 훨씬 저렴하게 관리할 수 있습니다.
- **편리한 관리**: 블로그 관리가 쉬워져 하루 한 번의 글쓰기도 문제 없습니다.

## 장점
- **시간 절약**: 자동으로 매일 새로운 글이 올라갑니다.
- **효과적인 마케팅**: 블로그를 마케팅 홍보용으로 최적화합니다.
- **브랜딩 강화**: 브랜드 블로그 담당자를 위한 손쉬운 콘텐츠 생성 도우미입니다.

## 설치와 사용 방법
1. [최신 버전 다운로드](https://github.com/your-repo/releases)
2. `make start`로 Docker 실행
3. 자세한 설치 및 사용 방법은 [식탁보 홈페이지](https://github.com/your-repo)에서 확인하세요.

## 개발 환경
- **빌드 환경**
  - Visual Studio 2022 이상
  - .NET 8.0 SDK
  - .NET Framework 4.8 SDK
- **테스트 환경**
  - Windows 10 1909 이상
  - 지원되는 SKU: Pro, Edu, Enterprise
  - Windows Sandbox를 실행할 수 있는 환경

## 의존성
- `black==22.10.0`
- `fastapi==0.87.0`
- `mypy-extensions==0.4.3`
- `pydantic==1.10.2`
- `requests==2.28.1`
- `urllib3==1.26.12`
- `uvicorn==0.19.0`
- `python-dotenv==0.21.0`
- `pandas==1.5.2`
- `cryptography==39.0.2`
---




## 데이터/요구 사항
- **데이터 수집 및 분석**: 네이버 뉴스 크롤링, 연관성 높은 기사 필터링, 프롬프트에 넘김
- **Knowledge Generation**: 프롬프트 엔지니어링 선정
- **Knowledge Injection**: 데이터를 넣고 프롬프트 처리
  - Retrieval
  - Template
  - Chaining

## 스폰서
GitHub Sponsorship을 통해 후원해주시면 프로젝트 진행에 큰 도움이 됩니다. [프로젝트 후원하러 가기](https://github.com/sponsors/your-repo)

## 저작권 정보
- Tablecloth Icon by Icons8
- Spork Icon by Freepik Flaticon
- Sponge Icon by Freepik Flaticon

---

### Dockerfile/develop
- makefile
- make start - docker 실행
---
### workflow 
| 파일        | 역할                                                                                           |
|------------|------------------------------------------------------------------------------------------------|
| main.py    | 프로그램의 주 진입점으로, 각 운영사의 공지사항을 가져오는 함수들을 호출하고, 역 정보 변동을 확인하는 함수를 호출 |
| utils.py   | 공지사항을 가져오고 Slack에 전송하는 함수들이 정의된 파일                                      |

