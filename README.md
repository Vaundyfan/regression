# regression
금융 하위 부문 주가지수(Co-integration, Co-movement, Structural Break) 분석
본 프로젝트는 2000년~2024년 한국 금융업 주요 하위 부문(은행, 보험, 증권) 주가지수 데이터를 활용하여 시계열 정상성, 공적분, 구조적 변동 분석한 코드 및 결과

1. 개요
분석 대상: 은행(Banks), 보험(Insurance), 증권(Securities) 일일 종가 (DataGuide MK2000 세부지수)

분석 기간: 2000-01-04 ~ 2024-12-31

분석 목적:

금융 섹터 간 장기 동조화(Co-movement), 공적분(Cointegration) 관계 확인

구조적 변동(Structural Break) 탐지 및 이후 동태적 변화 해석

2. 데이터 설명
원본: DataGuide MK2000, FnGuide 주가지수 산출식 기반

사용 변수

금융업종별 지수 (은행, 보험, 증권)

가격 변동성(Volatility), 국고채 3년/10년, 원-달러 환율 등

지수 산출식 요약

It = Mt / Bt × 1000

Mt: t일 시가총액, Bt: 기준 시가총액

기타 상세는 FnGuide 산출식 참조

Statistic	Banks	Insurance	Securities
Count	9128	9128	9128
Mean	4250.19	4803.75	954.57
Std. Dev.	1277.03	2172.10	327.72
Min	911.54	501.25	319.27
Median	4402.38	5529.38	929.29
Max	7518.22	9413.23	2362.10

3. 주요 분석 및 결과
(1) 정상성(Stationarity) 및 료
데이터: DataGuide, FnGuide MK2000 세부지수
