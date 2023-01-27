# markdown_20230127
마크다운 설명

### 11. 표 
|번호|아이디|이름|레벨|이메일|등록일|
|:--------||:--------||:--------||--------:||:------------------||:-------------:|
|1|dia|이상무|1|dia@naver.com|2023-01-27|

### 10. 인라인
문단 중간에 `CODE` 를 넣을 수 있습니다.(고정 폭 폰트를 표시해야 할 때 사용)  
예를들어 `return render(request, 'pybo/question_detail.html', context)` 처럼

### 9. 강조
Spring을 만끽하세요.  
**Spring**을 만끽하세요.

### 8. 이미지 넣기
![파이참](https://github.com/ASHyeon/markdown_20230127/blob/main/doc/image.png "머였더라")

### 7. 하이퍼 링크
[e클래스](https://cafe.daum.net/pcwk "e클래스의 cafe입니다.")

### 6. 가로라인
---
***
----------

### 5. 코드블록
```
def index(request):

    # list order create_date desc
    question_list = Question.objects.order_by('-create_date')  # order_by('-필드') desc, asc order_by('필드')
    # question_list = Question.objects.filter(id=99)
    context = {'question_list': question_list}

    return render(request, 'pybo/question_list.html', context)
```

### 4. 목록
1. 아이템 1  
2. 아이템 2  
  9. 단계 하위 아이템  
    3. 단계 하위 아이템  
9. 아이템 3

- 아이템 1  
+ 아이템 2  
  - 1단계 하위 아이템  
    * 2단계 하위 아이템  
      - 3단계 하위 아이템

순서없는 목록  
* 목록이름
- 목록
+ 목록

순서있는 목록  
1. 목록이름
2. 목록
3. 목록목록

### 3. 인용문
> 여기에 인용할 내용을 넣으면 됩니다  
> 빈 줄이 없으면 자동으로 인용 상자에 포함이 됩니다.

### 2. 헤더
# 헤더1
## 헤더2
### 헤더3
#### 헤더4
##### 헤더5


### 1. 문단 구분을 위한 개행.
문단을 작성합니다.(개행 공백 두개)->  
겨울이 가고 봄이 옵니다.
