# Scraping-Crawling

크롤링 + 스크래핑(beautiful soap, selenium)

-----

## Day 1 (2021-09-29)

- 네이버 개발자 센터 로그인
- 네이버 검색 API 학습(웹문서, 지식in, 블로그, 책, 영화, 쇼핑, 뉴스)

-----

## Day 2 (2021-09-30)

- BeautifulSoup 특징 학습
- HTML 파싱, HTML 태그파싱, HTML 태그검색 학습
- 웹페이지 콘텐츠 가져오기
- 인터넷 웹페이지 

-----

## Day 3 (2021-10-01)

- 웹 페이지 스크래핑(알렉스)
- 음악 순위 차트 스크래핑(벅스)

-----

## Day 4 (2021-10-02)

https://www.data.go.kr/

- 한국환경공단_측정소정보 학습
- 측정소별 실시간 측정정보 조회 학습
- 시도별 실시간 측정정보 조회 학습

## Day 5 (2021-10-06)

- 상가(상권)정보 학습
- 상권조회 학습
  - 지정 상권조회
  - 반경내 상권조회
  - 사각형내 상권조회
  - 행정구역 단위 상권조회
- 상가업소 조회 학습
  - 행정동 단위 상가업소 조회

## Day 6 (2021-10-08)

- 네이버 영화 스크래핑
- 현재 상영작 영화 리뷰 스크래핑
- 네이버 뉴스 기사 

## Day 7 (2021-10-0)

- 네이버 블로그 스크래핑(완성하지 못함)
```
---------------------------------------------------------------------------
AttributeError                            Traceback (most recent call last)
<ipython-input-30-74baf2d99352> in <module>
      1 query = input('검색 질의: ')
----> 2 post_df = get_posts(query)
      3 print('Done')

<ipython-input-29-b62a5e7bc102> in get_posts(query)
     16 
     17     for post in posts:
---> 18         title = post.find('a', {'class':'api_txt_lines total_tit'}).get_text()
     19         date = post.find('span', {'class':'sub_time sub_txt'}).get_text()
     20         blogger = post.find('a', {'class':'sub_txt sub_name'}).get_text()

AttributeError: 'NoneType' object has no attribute 'get_text'
```
