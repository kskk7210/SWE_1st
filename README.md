# 초보자를 위한 Markdown 사용법


## Markdown 이란?
Markdown이란 일반 텍스트 문서에 서식 요소를 추가하여 사용할 수 있는 경량 마크업 언어를 뜻한다. [^경량 마크업 언어]
[^경량 마크업 언어]: 태그 등을 통해 문서나 데이터 구조를 명기하는 언어를 마크업이라 하며 보다 경량화된 Markdown과 같은 언어를 경량 마크업 언어라고 한다.


## Markdown의 장점 및 사용 이유

### Markdown의 장점
- 쉬운 방법으로 문서의 작성이나 제작이 가능하다.
- Markdown 구문을 배우는 데에는 오래 걸리지 않으며 사용 방법을 익힌 후에는 거의 모든 곳에서 Markdown을 사용하여 문서 작성이 가능하다.

### Markdown의 사용이유
- 웹사이트나 문서, 이메일 등 **사용 범위가 넓다**.
- 운영체제를 실행하는 모든 장치에서 Markdown 형식의 텍스트를 만들 수 있다는 점에서 **플랫폼에 독립적**이다.
- Markdown 형식의 텍스트가 포함된 파일은 **거의 모든 프로그램을 사용**하여 열 수 있으며, 사용 중인 응용 프로그램이 **중지되어도** 텍스트 편집이 가능한 응용프로그램을 사용하여 Markdown 형식의 **텍스트를 읽을 수 있다**.
- Reddit이나 GitHub 같은 웹사이트에서 Markdown을 지원하며 많은 웹기반 프로그램이 이를 지원하기에 **모든 곳에서 사용**할 수 있다.


## Markdown의 기본 구문(Basic Syntax)
1. Header 작성
2. 단락 및 줄바꿈
3. 강조
4. 인용구
5. 목록
6. 코드블럭 및 링크, 이미지

### 1. Header 작성

1. \# 을 이용하여 작성할 수 있다.
2. \# 의 수가 많아질수록 글자의 스케일은 작아진다.

        # Header
        ## Header
        ### Header
이런 식으로 입력하면 렌더링 결과 아래와 같아진다.
 # Header
 ## Header
 ### Header

### 2. 단락 및 줄바꿈
1. 단락의 경우 빈 줄(단락과 단락 사이 아무것도 쓰이지 않은 줄)을 사용하여 구분 지을 수 있다.
2. 줄바꿈은 문장의 끝에 두개 이상의 공백을 입력하거나 문장 끝에 \<br\>를 입력해준다.
        
        I think this is a way to divide paragraphs. 
        
        I divided the paragraph by putting an empty line between the sentence above and this sentence.  
        Avoid using spaces or tabs at this time.<br>
        The implementation results are as follows.  
단락을 구분 지을 때는 문장 앞에 공백이나 탭을 사용하지 않아야함에 주의하며 위 방식대로 렌더링하면 아래와 같은 결과를 얻게 된다.

I think this is a way to divide paragraphs. 

I divided the paragraph by putting an empty line between the sentence above and this sentence.  
Avoid using spaces or tabs at this time.<br>
The implementation results are as follows.  

### 3. 강조 (Emphasis)  
1. 강조에는 볼드체(굵게)와 이탤릭체(기울임체)를 이용하는 방식이 있다.
2. 볼드와 이탤릭을 한번에 사용하는 방법도 있다.
        
        볼드체(Bold)의 경우 **Bold** 이런 식으로 앞뒤에 두개씩 붙여준다
        이탤릭체(Italic)의 경우 *Italic* 이런 식으로 앞뒤에 하나씩 붙여준다.
        두 강조방법을 한 번에 사용한다면 ***Bold Italic*** 과 같이 앞뒤로 세개를 붙여준다.
강조의 방식을 렌더링한 결과는 아래와 같다.

**Bold**  
*Italic*  
***Bold Italic***  

### 4. 인용구 (Quotation)  
1. 인용구를 표시하기 위해서는 > 기호가 사용된다.
2. 문장 앞에 >  배치하는 것에 따라 여러 문장이나 단락의 인용을 표시하거나 인용구 속에 인용구를 하나 더 표시하는 것이 가능하다.
3. 인용구 안에 여러 강조 표현같은 것들도 사용 가능하다.


        >This is a quote.
        >
        >이것은 **인용문**입니다.
        >>This is a nested quote.
        >
        > - 위는 중첩 인용문을 표시한 것입니다.
아래에는 인용구를 표시하는 것에 관한 렌더링 결과이다.

>This is a quote.
>
>이것은 **인용문**입니다.
>>This is a nested quote.  
>
> - 위는 중첩 인용문을 표시한 것입니다.  

### 5. 목록 (List)  
1. 숫자와 마침표를 사용하여 나타내는 방법의 경우 숫자는 꼭 1로 시작해야하지만 그 다음 숫자부터는 상관이 없다. 1로 시작한 이상 다음에 오는 숫자 상관없이 1, 2, 3, 4, ... 순서로 정렬된다.

        1. first 첫번째
        2. second 두번째
        3. third 세번째
        5. 4st 숫자는 5이지만 순서는 네번째
        8. 5st 숫자는 8이지만 순서는 다섯번째
        

2. /- (하이픈), * 이나 + 표시를 사용하여 목록을  표현할 수도 있다.
        
        - 목록을 나타낼 때 - 사용하는 방법
        * 목록을 나타낼 때 * 사용하는 방법
        + 목록을 나타낼 때 + 사용하는 방법
        
3. 목록 또한 중첩되게 만들 수 있으며 인용구도 표현도 가능하다.
        
        - 새로운 목록
        
            - 탭을 사용하여 중첩된 목록 생성  
                
        - 그 다음 목록
         
            목록 사이 문장을 넣을 때는 탭이나 공백 네 칸  
            
        - 인용구를 위한 목록  
        
            >인용구 목록
            
        - 인용구 생성 시에도 공백이 필요
                        
아래에는 목록을 표현하는 위 세가지 방식에 대한 렌더링 결과를 전부 보여주는 것이다.

1. first 첫번째  
2. secoun 두번째  
3. third 세번째  
5. 4st 숫자는 5이지만 순서는 네번째  
8. 5st 숫자는 8이지만 순서는 다섯번째  

- 목록을 나타낼 때 - 사용하는 방법  
* 목록을 나타낼 때 * 사용하는 방법  
+ 목록을 나타낼 때 + 사용하는 방법  

- 새로운 목록
 
    -탭을 사용하여 중첩된 목록 생성  
        
- 그 다음 목록  

    목록 사이 문장을 넣을 때는 탭이나 공백 네 칸  
    
- 인용구를 위한 목록  

    >인용구 목록  
    
- 인용구 생성 시에도 공백이 필요  

