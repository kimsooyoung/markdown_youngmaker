# markdown_youngmaker - markdown 다루기

<p align="center">
    <img src="https://user-images.githubusercontent.com/12381733/157016126-a57bf232-f63e-4046-979f-62a0626fc8ba.png" height="100">
</p>


> github의 issue를 등록하는 등 개발 문서를 다룰 시 많이 markdown이라는 문법을 많이 사용합니다.
> 
> 
> 이 노션에서는 **가장 기본적이고 많이 사용되는 최소한의 markdown 문법을 학습**하며, 학습 이후 실제 github Issue를 작성하는 실습도 진행해보고자 합니다.
> 

# 1. Header

---

샾(#) 기호의 개수를 통해 글자 크기를 조절 가능합니다. 

서로 다른 글자 크기를 통해 대제목, 소제목과 같은 제목 분류가 가능합니다.

<aside>
💡 띄어쓰기 없이 가장 앞부분에 # 기호를 붙여 사용 가능합니다.

</aside>

<aside>
💡 지금 보고계신 이 Notion도 Markdown을 지원하기 때문에 페이지 내에서 실습이 가능합니다.

</aside>

- 예시

```xml
# H1 태그
## H2 태그
### H3 태그
#### H4 태그
##### H5 태그
###### H6 태그
최대 6개까지 가능합니다.
```

- 결과

<aside>
💡 Notion에서는 최대 3개까지 가능하며, 아래와 같은 결과를 얻으실 수 있습니다.

</aside>

# H1

## H2

### H3

# 2. 볼드, 기울임, 단어 강조

---

**이 글자**처럼 특정 부분을 진하게 강조하고 싶다면 글자 좌,우로 *** (별) 기호를 2개씩** 붙여주시면 됩니다.

- 예시

```
**강조!!**
```

- 결과

**강조!!**

*이 글자*처럼 특정 부분을 기울이고 싶다면 글자 좌,우로 *** (별) 기호를 1개씩** 붙여주시면 됩니다.

- 예시

```
*기울임!!*
```

- 결과

*기울임!!*

`이 글자` 처럼 특정 단어를 강조하고 싶다면 글자 좌,우로 **` (숫자 1 옆의 기호)를 1개씩** 붙여주시면 됩니다.

- 예시

```
`단어 강조!`
```

- 결과

`단어 강조!`

<aside>
💡 아래와 같이 설명 중 코드상의 변수 이름이나 특정 함수를 일컬을 때 많이 사용합니다.


<p align="center">
    <img src="https://user-images.githubusercontent.com/12381733/157016115-84a8aaf8-4e85-49c9-aaa0-cdd4763aff44.png" height="200">
</p>

</aside>

# 3. 코드 단락

---

```python
import json
import pprint

# Code starts from here
if __name__ == '__main__':
  print("Hello, Mrs. Sinnara!")
```

위와 같이 작성한 코드를 띄어쓰기에 맞추어, 색상을 입혀 공유하고 싶은 경우가 많습니다.

이러한 경우, 코드의 상,하단에 **` (숫자 1 옆의 기호)를 3개씩** 붙이게 되면 해당 범위내의 텍스트를 코드로 간주하여 포매팅이 가능합니다. 

- 예시

#include <iosteam>

using namespace std;

int main(){
	return 0;
}


- 결과

```python
#include <iosteam>

using namespace std;

int main(){
	return 0;
}
```

C++의 경우 `int`, `#include`와 같은 단어가 다른 색을 보이고, 파이썬의 경우 `import`, `self` 와 같은 단어가 다른 색을 보이면 좋겠지요?

이러한 경우 첫번째 단락기호 ``` 다음에 사용하는 프로그래밍 언어 이름을 적어주시면 됩니다. 

- 예시 - python3

```
```**python3**
# Python code to demonstrate naive method
# to compute factorial
n = 23
fact = 1
  
for i in range(1,n+1):
    fact = fact * i
      
print ("The factorial of 23 is : ",end="")
print (fact)
```

- 결과

```python
# Python code to demonstrate naive method
# to compute factorial
n = 23
fact = 1
  
for i in range(1,n+1):
    fact = fact * i
      
print ("The factorial of 23 is : ",end="")
print (fact)
```

# 4. 그림 추가

---

Github Issue를 기준으로, 그림 삽입은 정말 쉽습니다. 

단순히 그림을 복사하신 뒤 붙여넣기 하시면 자동으로 해당 이미지의 링크와 함께 해당 문서 내에 추가됩니다.

<p align="center">
    <img src="https://user-images.githubusercontent.com/12381733/157016118-4839f1a3-6d9a-44db-b957-350050020ab0.png" height="150">
</p>

이렇게 복사된 이미지를 Write 탭에 붙여넣기 하시면 자동으로 업로드 되며 Preview 탭에서 확인이 가능합니다.


<p align="center">
    <img src="https://user-images.githubusercontent.com/12381733/157016120-7255c84f-3ac7-4d09-91e0-dd8822a2d32a.png" height="210">
</p>

# 5. 링크 삽입

---

[링크](http://www.google.com) <= 이렇게 글자 내 링크를 삽입하는 방법은 다음과 같습니다.

- 예시

```python
[보여질 글자](링크될 웹주소)

[네이버](www.naver.com)
```

- 결과

[네이버](http://www.naver.com)

# 실습해보기

---


[이 링크](https://github.com/kimsooyoung/markdown_youngmaker/issues/new/choose)로 접속하셔서 직접 여러분만의 Markdown을 작성해 보시기 바랍니다. 

우측 `Get Started` 를 클릭하신 뒤, 제가 미리 만들어 둔 포멧을 사용하셔서 연습해보시고, 추가 질 문이 있다면 질문도 남겨주세요. 확인 후 comment로 답변을 달아드리겠습니다.

<p align="center">
    <img src="https://user-images.githubusercontent.com/12381733/157016122-3c645c22-94fa-4364-b302-d879bb4adf10.png" height="100">
</p>

Write 탭에서 Markdown을 작성하신 뒤, 그 옆의 Preview를 통해 미리보기를 할 수 있습니다.

원하는 결과를 얻기 위해 여러 차례 Preview 확인은 필수입니다. 😊

<p align="center">
    <img src="https://user-images.githubusercontent.com/12381733/157016124-494b0c00-2f41-4be1-b8f0-fcd62e98b381.png" height="250">
</p>


# 마치며

---

모르는 문제가 있을 때, 단순히 풀어달라 하기보다. 어디서 막혔는지, 왜 풀리지 않는다 생각하는지, 시도해 본 것은 무엇인지 이러한 정보를 함께 전달한다면, 질문을 받아주기도 훨씬 용이하고, 친절하게 알려주소 싶은 마음도 뿜뿜합니다.

이 글을 읽으시는 분들 모두 기본 Markdown을 통해 더 훌륭한 개발자로 성장하시기를 기원합니다. 🙏🙏🙏
