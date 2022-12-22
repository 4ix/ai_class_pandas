## 2022-12-22(목)
1. folium 라이브러리 (지도 활용)

2. ★ 데이터 사전 처리 ★
- 1. 누락 데이터 처리
- 2. 단위환산
- 3. 치환 후 누락 데이터 처리, 다른 값으로 대체
- 4. 중복 데이터 처리
- 5. 데이터 타입을 변환 시킴
- 6. 숫자형, 문자형, 범주형으로 변경
- 7. 문자형과 범주형은 dummy 변수로 변환
- 8. 시계열 데이터 있으면 처리

3. 범주형(카테고리) 데이터 처리
- 구간 분할
- 더미 변수

4. 정규화
5. 시계열 데이터

6. 20221222_part5
- 데이터 전처리 연습


## 2022-12-21(수)
1. 20221221_part4
- matplotlib를 활용한 그래프 그리기 연습

## 2022-12-20(화)
1. 20221220_part2
- 데이터프레임을 엑셀로 저장. 
-> writer = pd.ExcelWriter('./data/df_sample_2.xlsx')

2. 20221220_part3

3. numpy

4. 20221220_part4
- matplotlib 사용법 연습

## 2022-12-19(월)
1. pandas 라이브러리 사용방법 연습

2. student_score
- 시리즈 생성 -> pd.Series(리스트 or 딕셔너리{키:값, })
-             -> 딕셔너리의 키가 인덱스가 됨
- 데이터프레임 -> pd.DataFrame(이차원리스트 or 딕셔너리{키:[값,...], })
-              -> 딕셔너리의 키가 컬럼명이 됨
- df(sr).index = [ 인덱스명, ....]
- df.colums = [ 컬럼명, ... ]
- 데이터프레임 -> 특정 컬럼을 인덱스로 설정 : df.set_index(컬럼, inplace = True)
-              -> 컬럼 추출: df.컬럼명 or df['컬럼명']
-              -> ★ 인덱스 추출: df.loc['인덱스명'], df.iloc[0]
-              -> 각 원소 추출: df.loc['인덱스명', '컬럼명'], df.iloc[인덱스 숫자, 컬럼 숫자]
-              -> df.reset_index(): 인덱스를 컬럼으로
-              -> df.reset_index(새로운 인덱스 배열, fill_value=0)
-              -> df.sort_index(인덱스명, ascending=True): 인덱스로 정렬
-              -> df.sort_values(by='컬럼명', ascending=True): 컬럼의 값으로 정렬
-              -> df.T, df.transpose(): 전치 행렬

3. 데이터 입출력

4. pandas_hw1
- seborn의 mpg 데이터셋 활용하여 자료 슬라이스 연습