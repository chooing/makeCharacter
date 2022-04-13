# make Character
html과 css를 사용하여 캐릭터를 만들었습니다.
https://chooing.github.io/makeCharacter/

# 작업 스케치 및 완성
일러스트로 러프한 캐릭터 초안 제작 후 작업하며 다듬어갔습니다. 
![스케치](https://user-images.githubusercontent.com/96187560/163180423-1164a6ce-08e1-45d1-9712-70ee2742771e.PNG)

완성본
![yojo](https://user-images.githubusercontent.com/96187560/163180000-01c3dd5c-0143-43d2-90c8-9708212383ff.png)

# 사용한 CSS 속성
캐릭터를 제작하며 사용한 속성입니다. 최대한 실무에서 자주 사용하지 않는 속성이나 웹사이트 제작 때 사용량이 적은 것을 위주로 사용해 보고자 했습니다.

## position
각각의 **요소들을 배치**할 때 사용했습니다.<br>
얼굴(.face)를 position: relative로 기준으로 삼아 각 요소들을 붙여가며 캐릭터의 뼈대를 세웠습니다.

## border-radius
각 부위를 표현할 때 가장 자주 사용한 속성입니다.<br> 모서리가 둥근 사각형 동그란 모양, 타원형, 물방울형 등 곡선이 필요한 경우가 다반사였고 모두 border-radius를 사용하여 모양을 잡았습니다.

## ::before, ::after
html의 태그 사용을 줄이고자 가상요소를 사용했습니다.<br> 
- body에 ::before, ::after로 "꽃사슴", "YOJO" 글씨를 넣어 텍스트 요소 대신 사용

- 눈 요소에 ::before로 눈동자를 표현했고 ::after로 눈꺼풀을 표현

- 중심이 되는 뿔 요소에 양옆 가지를 ::before, ::after로 표현

- 귀 요소 위에 ::after요소로 덮어 귀가 반쯤 기울진 것을 표현 

- 여러겹이 겹쳐진 꽃을 표현하기 위해서 ::after로 꽃잎을 만들고 회전

## transform
기울여짐을 표현하기 위해 rotate(숫자deg) 값으로 귀와 꽃잎을 회전 시켜 기울여짐을 표현했습니다.

## z-index
요소에 우선순위를 주어 앞뒤로 배치를 조정했습니다.

## transition, :hover
캐릭터와 서로 상호작용이 되도록 특정 요소에 마우스를 올리면 변화가 나타나도록 했습니다.
- 꽃잎에 마우스를 올리면 흰색에서 분홍색으로 변화

- 눈에 마우스를 올리면 반쯤 눈 감는 행동

## animation
극적인 등장과 움직임을 표현하기 위해 사용했습니다.
- 맨처음 페이지 로딩 시, 글자가 차례대로 나타나고 사슴 캐릭터가 등장하는 것으로 극적인 등장을 연출

- 귀와 눈동자가 움직여 캐릭터에 생동감을 표현


# 느낀점
- **position: relative와 absolute에 대해 알게 되었습니다.**<br> relative를 기준으로 absolute 속성들이 배치되며 그 안에 또 absolute를 넣어도 부모요소가 기준이 되어 배치된 것을 볼 수 있었습니다. 

- **::before, ::after 가상요소 사용으로 가상요소가 어떤 곳에 생성되고 조정하는 법을 익혔습니다.** <br> html에서 태그가 많이 사용되면 복잡하고 지저분해질 것 같아 최대한 가상요소를 사용했습니다. 이를 통해 가상요소가 어떤 위치에 생성되고 어떻게 조정할지 익혔고 가상요소가 기본적으로 inline 요소인 것을 알았습니다.
html과 css로 캐릭터 만들기!

