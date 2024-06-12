# AI CPA

> XBRL(eXtensible Business Reporting Language) Generator
>
> AI기술을 활용한 확장성 경영보고언어 생성기

**롯데이노베이트 멤버스IS팀 권기정**

## 시장조사 및 배경

1. XBRL이란 무엇인가?

   - XBRL이란 차세대 인터넷 언어인 XML(eXtensible Markup Language)을 기반으로 **복잡한 기업정보를 효율적으로 생성/교환/비교**할 수 있도록 만든 기업보고용 국제 표준화 언어
   - 기업의 공시정보(Fact)에 표준이름(Tag)을 붙여서 문서를 작성하는 제도
   - 기업은 감독기관이 제시한 Taxonomy내의 약속된 표준이름을 사용하여 작성

   ![image](https://github.com/gijeogiya/4CPA/assets/97646078/0003c64e-e559-44e6-8a3c-26e18f3b331d)


2. 대한민국에서의 XBRL **정책/시장 현황**

   - **2023년 하반기**부터 금융당국이 **자산총액 2조 원 이상 상장회사**를 시작으로 순차적으로 주석을 포함한 재무제표 전반에 대한 **XBRL 공시 의무화**를 추진함에 따라 금융•회계업계는 관련 전문가 자문 서비스 수요가 증가할 것으로 전망

   ![image](https://github.com/gijeogiya/4CPA/assets/97646078/79b17c32-32f9-4643-81ce-3678a68022c6)


3. 대한민국에서의 XBRL **고객 동향**

   - 대한민국 회계 시장 내 전문가 부족
   - 롯데지주, 롯데이노베이트를 포함한 대부분의 롯데계열 상장사 또한 XBRL 공시 의무 대상으로 지난 2023년 하반기부터 XBRL을 활용하여 공시

   ![image](https://github.com/gijeogiya/4CPA/assets/97646078/69cf852f-b9e4-407e-a999-f6d5b6f4fd0f)


   

4. 사업 상황
   - 금융감독원이 주도하여 XBRL 생성 툴을 배포
   - 회계법인의 용역 사업을 통해 XBRL 작성(주석 등)
   - 현재 AI를 활용한 XBRL 서비스 및 오픈소스는 없는 것으로 확인됨



## AI기술을 활용한 XBRL 생성기 아이디어

1. XBRL 생성기 모델링

   - INPUT: 기업의 공시정보(Fact)가 기입된 엑셀 형식의 표
   - OUTPUT: 기업의 공시정보(Fact)에 표준이름(Tag)가 매핑된 XBRL 파일

   ![image](https://github.com/gijeogiya/4CPA/assets/97646078/0003c64e-e559-44e6-8a3c-26e18f3b331d)

2. AI 학습 방안

   - 대한민국 Open Dart(https://opendart.fss.or.kr/)에 공시된 2조원 이상 자산 기업이 공시한 공시정보(Fact)와 XBRL 데이터(Fact, Tag)를 활용
   - 미국 전자공시시스템(https://www.sec.gov/)에 공시된 공시정보(Fact)와 XBRL 데이터(Fact, Tag)를 활용
   - 추후 롯데 고객사 XBRL 작성에 활용된 Rough한 공시정보(Fact)와 결과물인 XBRL 데이터(Fact, Tag)를 활용
  ![image](https://github.com/gijeogiya/4CPA/assets/97646078/25b74cdc-67f3-4dbe-9bed-24220d8f90dc)


3. 생성기 검증 방안

   - Dart 제공 뷰어를 활용한 적합도 판정 (현재 %단위로 제공 중)
   - 실제 회계사(전문가)가 작성한 XBRL 결과물과의 비교/검증

## 기대효과 및 리스크

1. 1차 기대효과 (사내 적용)
   - 롯데이노베이트의 회계업무 개선을 통한 성과 창출 

2. 2차 기대효과 (롯데 그룹사 적용)
   - 롯데그룹의 재무정보의 통일성있는 재무정보의 호환성, 경제성, 투명성 향상을 통한 성과 창출
3. 3차 기대효과 (SaaS 형태로 국내외 회계법인 등에 공급)
   - SaaS 판매를 통한 영업이익 창출
   - AI기술을 활용한 회계/감사 시장의 새로운 패러다임으로 혁신하는 기업으로 등극
4. 리스크
   - 금융감독원의 규제
     - 현재 금융감독원이 개발/배포하는 XBRL툴은 매우 폐쇄적
     - 하지만 XBRL이 추구하는 것이 호환성, 경제성, 투명성인 만큼 미래에 IT기술과 결합될 가능성이 큼
