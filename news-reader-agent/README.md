# News Leader Agent (뉴스 리더 에이전트)

## 🎯 목적 (Goal)
특정 뉴스 주제를 입력받아, 바로 발행 가능한 수준의 뉴스 보고서를 생성합니다.  
Create a publish-ready news report immediately after receiving a specific news topic.

---

## 🤝 협업 에이전트 (Collaborative Agents)

### 1. 🔍 뉴스 헌터 에이전트 (News Hunter Agent)
- Google 검색과 웹사이트 스크래핑을 통해 주제와 관련된 기사를 수집합니다.  
- Afterwards, the agent filters out low‑quality information and scores each article based on credibility and relevance.

### 2. 📝 요약 에이전트 (Summary Agent)
- '뉴스 헌터 에이전트'가 선별한 기사들에서 핵심 주제와 통계 데이터를 추출하여 상세 요약문을 만듭니다.  
- Extracts key topics and statistical data from selected articles to generate detailed summaries.

### 3. ✨ 큐레이터 에이전트 (Curator Agent)
- '요약 에이전트'가 만든 요약본을 바탕으로 주요 기사, 속보, 편집자 분석, 관련 읽을거리, 정확한 인용 정보를 포함한 최종 보고서를 완성합니다.  
- Builds the final report including major articles, breaking news, editorial insights, additional reading, and accurate citations.

---

# 📘 전체 프로세스 다이어그램 (Overall Workflow Diagram)

```
📰 뉴스 주제 (News Topic)
        ↓
🔍 뉴스 헌터 에이전트 (News Hunter Agent)
        ├── ⭐ 기사 선별 (Article Selection)
        │         ↓
        │     📝 요약 에이전트 (Summary Agent)
        │         ↓
        │     ✨ 큐레이터 에이전트 (Curator Agent)
        │         ↓
        │     📄 보고서 작성 (Report Writing)
        │         ↓
        │     🎯 최종 보고서 (Final Report)
        │
        └── 🔎 구글 조사 (Google Research)
                   ↓
            🌐 웹 스크래핑 (Web Scraping)
```
