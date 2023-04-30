# 프로젝트명: Hunter Farmer / 개발자: 이재형

# [ 목차 ]
### 1. [컨셉](#컨셉)
<h4> ● 메인 컨셉 </h4>    
<h4> ● 서브 컨셉 </h4>    

### 2. [관련 이미지와 동영상](#관련-이미지와-동영상)
### 3. [대표 이미지의 컨셉과 기반 작품 묘사](#대표-이미지)
### 4. [Hunter Farmer의 구성 요소](#Hunter-Farmer의-구성-요소)
<h4> ● 메커니즘 </h4>
<h4> ● 이야기 </h4>
<h4> ● 미적요소 </h4>
<h4> ● 기술 </h4>

### 5. [게임 시스템 디자인](#게임-시스템-디자인)
<h4> ● 게임 오브젝트 분해  </h4>
<h4> ● 오브젝트 피라미터 </h4>
<h4> ● 플레이어 캐릭터 피라미터 </h4>
<h4> ● 게임의 규칙 </h4>

### 6. [개발 요구사항과 흐름도](#개발-요구사항과-흐름도)
<h4> ● 요구사항 </h4>
<h4> ● 키보드 이벤트에 대한 흐름도 </h4>
<h4> ● 스토리 보드 </h4>

### 7. [프로토타입 개발 요구사항](#프로토타입-개발-요구사항)

### 8. [프로토타입 개발작업 일정](#프로토타입-개발작업-일정)

### 9. [프로토타입 주차별 구현 과정](#프로토타입-주차별-구현-과정)

# [컨셉]

## 메인컨셉 : 섬멸

- 적(몬스터)을 쓰러트린다 즉 섬멸시킨다는 의미로 적의 공격을 파악하며 쓰러트린다는 컨셉이다.

### 서브 컨셉 1 : 패턴

- 몬스터마다 플레이어를 공격하는 방법 즉 패턴이 다르며, 특정 패턴으로 역으로 공격을 파훼하거나 몬스터가 피격이 안되는 경우가 있다.  그렇기 때문에 플레이어는 몬스터마다 패턴을 파악하며 쓰러트려야 한다.

### 서브 컨셉 2 : 체력

- 플레이어가 몬스터에게 공격을 받으면 데미지를 입어 깎이며 0이 될 시 죽게 된다. 죽지 않게 하기 위해 작물을 먹거나 공격을 피해야 한다.

### 서브 컨셉 3 : 기력

- 플레이어가 공격이나 패턴을 회피할때 사용하며 없을 시에는 공격과 회피가 불가능해진다. 상황에 따라 기력을 아껴서 몬스터의 공격에 대비해야 한다.

### 서브 컨셉 4 : 보스

- 몬스터 중 가장 강한 몬스터이며 그렇기 때문에 여러가지의 패턴이 구성되어 있고 체력이 많다.

### 서브 컨셉 5 : 농사

- 플레이어는 몬스터를 쓰러트릴 무기 즉, 작물을 재배하여야 한다. 작물마다 자라는 시간이 다르며 물을 주워야 자란다.

### 5번의 서브 컨셉 1 : 무기

- 플레이어가 농사를 하여 재배한 작물이 무기가 되며 이 작물로 몬스터를 쓰러트려야한다. 작물마다 능력치가 다르며 플레이어마다 자신에게 맞는 작물을 찾아야 한다.

### 5번의 서브 컨셉 1 : 수집

- 작물을 수집할수록 체력과 해당 작물의 능력치가 상승하므로 많은 작물을 수집하여야한다. 또한, 플레이어의 피가 없을 시 작물을 먹으면 회복이 가능함으로 많은 작물을 먹어줘야 한다.

### 5번의 서브 컨셉 1 : 구입

- 플레이어는 몬스터를 사냥하여 얻은 골드(돈)로 씨앗을 구매하여 작물을 키울 수 있다.

<br><br>

# [관련 이미지와 동영상]

### 1. 패턴 컨셉과 관련된 이미지

![어쌔신크리드오디세이](https://user-images.githubusercontent.com/114119404/191637710-d6dce931-578d-4167-a067-9caf88e70b19.png)    
이름: 어쌔신크리드 오디세이

선정한 이유: 플레이어가 몬스터(Enemy)를 공격하면 몬스터가 피격을 당하며 넉백을 당하지만 위의 게임처럼 몬스터가 특정한 색으로 바뀌며 공격을 당해도 넉백을 당하지 않고 강한 공격을 한다.

유사한 점: 특정 패턴에서 몬스터의 슈퍼아머 후 강한 공격


![로스트아크](https://user-images.githubusercontent.com/114119404/191638125-62c7bf65-4840-4517-9534-0f22a40ff503.png)    
게임 이름: 로스트아크

선정한 이유: 몬스터가 플레이어에게 강한 데미지를 주는 패턴을 사용 시 위의 사진처럼 특정한 색으로 바뀌며 플레이어가 해당 패턴을 파훼하지 못하면 강한 데미지를 입게된다.

유사한 점: 플레이어가 몬스터의 특정 패턴을 파훼 (실패 시 강한 공격)

![가디언테일즈](https://user-images.githubusercontent.com/114119404/191638289-bc06cbe4-6e03-4011-8073-e6632cc5887a.png)    
게임 이름: 가디언 테일즈

선정한 이유: 몬스터가 플레이어의 위치에 원이나 사각형으로 해당 위치를 공격한다는 것을 알리고 몇 초의 시간이 지난 후 해당 위치에 몬스터가 공격을 하며 플레이어가 해당 위치에 있을 시에 데미지를 입는다.

유사한 점: 특정 패턴으로 해당 위치를 알린 후 공격

### 2. 보스 컨셉과 관련된 이미지

![가디언테일즈1](https://user-images.githubusercontent.com/114119404/191638458-abb82f19-4475-436f-b6e3-62ec637dd071.png)    
게임 이름: 가디언 테일즈

선정한 이유: 게임 화면 위에 보스의 체력바가 있어 보스의 피가 얼마나 남아있는지 확인 할 수 있고 다른 몬스터와 다르게 가장 강하기 때문에 몸이 다른 몬스터에 비해 크다. 또, 보스 몬스터이기 때문에 일반 몬스터와 다르게 다양한 패턴을 사용한다.

유사한 점: 보스의 체력바, 다른 몬스터에 비해 큰 몸, 일반 몬스터에 비해 다양한 패턴

### 3. 체력과 기력 컨셉과 관련된 이미지

![몬스터헌터1](https://user-images.githubusercontent.com/114119404/191638964-98eb779d-3a2e-4b71-b3c0-68d720d373d1.png)
![몬스터헌터2](https://user-images.githubusercontent.com/114119404/191638979-10fa7923-2745-4cfd-aaaa-55919e5471f0.png)    
게임 이름: 몬스터 헌터 월드

선정한 이유: 캐릭터의 체력과 기력을 나타내는 UI가 내가 개발할 최종 작품과 비슷하여 선정하였고 몬스터에 공격을 당하면 체력 게이지가 닳고 달리거나 공격을 하면 기력 게이지가 달아 공격이나 회피를 하지 못한다.

유사한 점: 체력과 기력 UI, 공격을 당하면 체력 게이지 감소와 달리거나 공격 시 기력 게이지 감소

### 4. 농사 컨셉과 관련된 이미지

![스타듀밸리](https://user-images.githubusercontent.com/114119404/191639154-5b6c0d58-d486-40ce-8875-05506241dc62.png)    
게임 이름: 스타듀밸리

선정한 이유: 플레이어가 농사를 지어 작물을 재배를 하여 재배한 작물이 무기가 된다. 또, 컨셉이 섬멸이라 어두운 분위기라 생각을 하지만 위의 게임처럼 밝은 분위기를 나타낼 것이다.

유사한 점: 플레이어가 직접 농사하여 재배, 밝은 분위기

### 5. 구입 컨셉과 관련된 이미지

![스타듀밸리1](https://user-images.githubusercontent.com/114119404/191639169-85f6cdc9-39f7-4c61-93bc-2dc909657d85.png)    
게임 이름: 스타듀밸리

선정한 이유: 플레이어가 몬스터를 쓰러트릴 때 골드(돈)이 나오는데 그 골드로 상인한테 씨앗을 구매를 할 수 있다. 씨앗을 구매하여 작물을 키울 수 있다.

유사한 점: 골드로 상인한테 씨앗을 구매 할 수 있음

### 6. 수집 컨셉과 관련된 이미지

![스타듀밸리2](https://user-images.githubusercontent.com/114119404/191639174-116740c3-ceb4-4107-abf0-7f8d771b6808.png)    
게임 이름: 스타듀밸리

선정한 이유: 스타듀밸리의 스탯은 해당 작업을 많이 할 수록 증가하는 점을 이용하여 작물을 재배한 만큼 해당 작물의 공격력을 증가 시키면 좋을 거 같아 선정하였다.

유사한 점: 스탯, 횟수로 인한 스탯 증가

<br><br>

# [대표 이미지]

![대표이미지](https://user-images.githubusercontent.com/114119404/191640303-a4dda6ee-5a64-4c1a-8950-d1e6f905134f.jpg)    

<br><br>

# [대표 이미지의 컨셉과 기반 작품 묘사]

> ### 대표이미지 기반 : 

왼쪽 상단에는 플레이어의 체력과 기력을 나타내는 UI로서 몬스터에게 공격을 당할시 체력이 감소를 하고 공격과 회피, 반격을 사용시 기력이 감소한다.

왼쪽 하단에는 플레이어의 기술로 반격과 회피 이미지가 있는데 사용시 쿨타임(재사용 시간)이 얼마나 남았는지 알려주는 UI이다.

왼쪽 중앙에는 몬스터가 있으며 몬스터 위에는 몬스터의 이름과 체력이 존재하며 몬스터의 체력이 0이 되면 몬스터는 쓰러지게 된다. 

몬스터마다 패턴이 존재하며 몸이 파란색이나 붉은색으로 바뀌며 공격을 시전하는데 해당 그림에는 파란색으로 빛나며 패턴을 사용 중이라는 것을 알려준다.

오른쪽 중앙에는 플레이어(자신)로 손에는 자신이 직접 키운 작물이며 무기인데 작물마다 공격 범위와 공격 속도가 다르다.

> ### 컨셉에 따른 게임 흐름 : 
1. 플레이어는 처음 시작 시 씨앗을 제공하는데 해당 씨앗을 기른 다음 재배한다.
2. 플레이어가 재배 중인 작물에게 물을 주지 않으면 해당 작물은 자라지 않으며 물을 준 다음 하룻밤이 지나야 작물에게 영향이 끼친다.
3. 재배한 작물이나 주위에 있는 야생 식물로 몬스터를 섬멸한다.
4. 몬스터를 섬멸한 보상으로 돈을 벌어 상인에게 다양한 식물을 구매하여 재배한다.
5. 여러 작물을 재배하거나 한 가지의 작물을 많이 수집하여 강해진 다음 보스 몬스터를 처치한다.
6. 플레이어의 기력이 모두 소모시 잠시 탈진 상태가 일어나며 체력이 모두 소진 시 쓰러지며 하루 전날로 돌아간다.

<br><br>

# [Hunter Farmer의 구성 요소]

## 1. 메커니즘

[도전 과제]

1. 작물을 재배하여 그 작물로 몬스터를 섬멸하라
2. 몬스터를 섬멸한 보상으로 재화를 얻어 씨앗을 구매하라
3. 여러 가지의 작물들을 수집하여 더욱 강해져라
4. 보스 몬스터를 섬멸하여 농장을 지켜라

[재미 요소]

1. 가상의 작물이 아닌 실제로 존재하는 작물로서 기를 수 있다.
2. 각 작물에 물을 제공해야 자라며 주지 않을 시에 자라지 않는다.
3. 몬스터(동물)마다 1~2개의 패턴을 사용하며 플레이어는 반격이나 회피로 공략을 바꿀 수 있다.
4. 작물로 몬스터(동물)를 공격을 하여 쓰러트리는데 작물마다 공격 범위와 속도가 다르며 원하는 작물로 교체 할 수 있다.
5. 플레이어의 체력이 적을 때 무기로 사용하는 작물을 먹어 체력을 회복 시킬 수 있다.
6. 보스 몬스터는 다른 몬스터와 다르게 몸짓이 크고 더 많은 패턴을 가진다.

<br>

## 2. 이야기

[만들게 된 배경]    
평소가 농사게임을 즐겨하는데 농사게임에 RPG를 넣으면 어떤느낌일까? 라는 생각을 갖고만 다니다가
게임프로젝트2에서 기획을 하게되어 만들게 되었다. 농사와 RPG를 하는 게임이 여럿 있어서 참신함을
가지고자 무기를 자신이 기른 작물로 하면 좋을 것 같아서 기획을 하게 되었다.

[참신함]    
1. 무기가 우리가 생각하는 철제 검이나 활을 생각하는데 관점을 바꾸어 무기를 작물로 설정함
2. 포션으로 체력을 회복하는 것이 아닌 무기인 작물을 먹어 회복 시킬 수 있음

[카메라 관점]      
플레이어의 중심으로 플레이어가 움직일 때마다 카메라도 플레이어를 따라 이동함 

<br>

## 3. 미적요소

[디자인]    
1. 컨셉이 섬멸이지만 서브 컨셉으로 농사가 있기에 어두운 분위기보단 밝은 분위기를 가진다.
2. 깊은 산 속이므로 나무와 풀 같은 자연적인 요소가 많다.

[음향]     
1. 산 속의 분위기기 때문에 새 소리나 자연과 어울리는 음향을 추가
2. 보스 몬스터와 대결을 할 때에는 웅장한 음향을 추가하여 몰입 할 수 있도록 함
3. 실제 몬스터(동물)가 걷거나 맞을 때 그에 맞는 음향을 추가

<br>

## 4. 기술

유니티를 이용하여 PC용으로 개발

<br><br>

# [게임 시스템 디자인]

## 게임 오브젝트 분해

![오브젝트분해](https://user-images.githubusercontent.com/114119404/196509747-0b92bed0-a7f4-4b43-939b-c4dcb2e27c99.png)
![오브젝트분해2](https://user-images.githubusercontent.com/114119404/196509751-00a2309a-5673-4da8-828b-35d953428d09.png)
![오브젝트분해3](https://user-images.githubusercontent.com/114119404/196509753-a1a12c9f-c974-478b-a501-60ac2606effb.png)
![오브젝트분해4](https://user-images.githubusercontent.com/114119404/196509757-e57d95c8-3852-4a3b-bcbb-ff5158c20b7f.png)
![오브젝트분해5](https://user-images.githubusercontent.com/114119404/196509758-344e4ab5-4d1b-4b1e-9b56-d9614815660b.png)
![오브젝트분해6](https://user-images.githubusercontent.com/114119404/196509761-dcdda8b5-1683-44e0-a7af-05cce526fcfe.png)

<br>

## 파라미터(속성)

1) 오브젝트 이름: Baby(Duck, Pig, Chicken, Goat, Sheep, Cow, WildBoar, Alpaca),
 Adult(MDuck, WDuck, Pig, WChicken, MChicken, Goat, Sheep,)

|속성|영문명칭|설명|
|:---:|:---:|:---:|
|체력|Hp|일반 몬스터의 체력|
|공격력|Atk|일반 몬스터가 플레이어를 공격했을 떄의 수치|
|공격범위|AttackRange|일반 몬스터의 공격하는 범위|
|이동속도|MoveSpeed|일반 몬스터의 이동속도|
|골드|Gold|일반 몬스터를 처치했을 때의 나오는 골드량|

<br>

2) 오브젝트 이름: Adult Cow, Adult WildBoar, Adult Sheep

|속성|영문명칭|설명|
|:---:|:---:|:---:|
|체력|Hp|보스 몬스터의 체력|
|공격력|Atk|보스 몬스터가 플레이어를 공격했을 때의 피해 수치|
|공격범위|AttackRange|보스 몬스터의 공격하는 범위|
|이동속도|MoveSpeed|보스 몬스터의 이동속도|
|골드|Gold|보스 몬스터를 처치했을 때의 나오는 골드량|

<br>

3) 오브젝트 이름: Radish, GreenOnion, Cucumber, Pepper, Mushroom

|속성|영문명칭|설명|
|:---:|:---:|:---:|
|공격력|Atk|몬스터를 공격할 때의 입히는 피해 수치|
|공격범위|AttackRange|몬스터를 공격하는 범위|
|공격속도|AttackSpeed|몬스터를 공격하는 범위|
|체력회복수치|Heal|플레이어가 작물을 먹었을 때의 플레이어의 체력 증가 수치|
|자라나는 시간|GlowTime|작물을 재배하기까지의 걸리는 시간|
|씨앗가격|SeedPrice|씨앗을 구매하는 가격|

<br>

## 행동

1) 오브젝트 이름: Player

|행동|영문명칭|설명|
|:---:|:---:|:---:|
|서있기|Idle|가만히 서있을 때의 행동|
|걷기|Walk|플레이어가 평소 이동하는 행동|
|뛰기|Run|기력을 소모하며 빠르게 이동하는 행동|
|회피|Evade|짧은 순간에 빠르게 이동할 하는 행동|
|공격|Attack|몬스터를 공격하는 행동|
|반격기|Counter|몬스터의 강한 공격을 반격하는 행동|
|먹기|Eat|체력을 회복 시키기 위해 하는 행동|
|죽음|Die|플레이어의 체력이 0이 될 시의 행동|

<br>

2) 오브젝트 이름: Baby(Duck, Pig, Chicken, Goat, Sheep, Cow, WildBoar, Alpaca),
 Adult(MDuck, WDuck, Pig, WChicken, MChicken, Goat, Sheep,)

|행동|영문명칭|설명|
|:---:|:---:|:---:|
|서있기|Idle|가만히 서있을 때의 행동|
|걷기|Walk|플레이어가 평소 이동하는 행동|
|공격|Attack|플레이어를 공격하는 행동|
|죽음|Die|몬스터의 체력이 0이 될 시의 행동|

<br>

3) 오브젝트 이름: Adult Cow, Adult WildBoar, Adult Sheep

|행동|영문명칭|설명|
|:---:|:---:|:---:|
|서있기|Idle|가만히 서있을 때의 행동|
|걷기|Walk|플레이어가 평소 이동하는 행동|
|공격|Attack|플레이어를 공격하는 행동|
|강한 공격|Strong Attack|특별한 패턴 후 공격을 하는 행동|
|쓰러짐|Fall Down|패턴 중에 플레이어가 반격을 했을 시의 행동|
|죽음|Die|몬스터의 체력이 0이 될 시의 행동|

<br>

## 상태

1) 오브젝트 이름: Player

| <center>현상태</center> | <center>전이상태</center> | <center>전이조건</center> |
|:---:|:---:|:---:|
|평상시|죽는다|체력이 0이 될 시|
|평상시|0.5초동안 무적이 된다.|몬스터에게 피격을 당했을 시|
|무적|평상시|피격 후 0.5초 무적이 지났을 시|
|평상시|회피를 하는 동안 무적이 된다.|플레이어가 회피를 했을 시|
|회피로 인한 문적 상태시|평상시|플레이어가 회피 동작을 다 맞췄을 시|

<br>

2) 오브젝트 이름: Baby(Duck, Pig, Chicken, Goat, Sheep, Cow, WildBoar, Alpaca),
 Adult(MDuck, WDuck, Pig, WChicken, MChicken, Goat, Sheep)

|현상태|전이상태|전이조건|
|:---:|:---:|:---:|
|평상시|죽는다|체력이 0이 될 시|
|플레이어에게 피격을 당하였을 시|플레이어에게 공격을 하며 공격을 하는 동안 피격 무적이 된다.|피격을 더 당할 경우|
|피격 무적이 되어 공격을 한다.|피격 무적이 풀리며 평상시로 돌아간다.|피격 무적 후에 플레이어에게 공격을 시전 했을 경우|

<br>

3) 오브젝트 이름: Adult Cow, Adult WildBoar, Adult Sheep

|현상태|전이상태|전이조건|
|:---:|:---:|:---:|
|평상시|죽는다|체력이 0이 될 시|
|플레이어에게 피격을 당하였을 시|일반 공격을 시전|플레이어에게 피격을 당했을 시|
|일반 공격을 시전|평상시|플레이어에게 일반 공격을 시전 했을 때|
|평상시|강한 공격을 시전|플레이어에게 공격을 3회 했을 시|
|강한 공격을 시전|평상시|플레이어에게 강한 공격을 시전 했을 때|
|플레이어에게 강한 공격을 시전하는 중이였을 때|2초동안 쓰러진다.|플레이어가 강한 공격에 반격기를 사용했을 때|
|잠시 쓰러졌을 때|2초 뒤에 일어나서 평상시|잠시 쓰러졌을 경우|

<br>

## 플레이어 캐릭터 속성(파라미터)

|속성|영문명칭|설명|
|:---:|:---:|:---:|
|체력|Hp|플레이어의 생명력로 0이 될 시 플레이어는 죽게 된다.|
|기력|Sp|플레이어의 세태미나로서 공격과 회피를 할 시 줄어든다.|
|공격력|Atk|몬스터를 공격할 때의 입히는 피해 수치|
|이동속도|MoveSpeed|플레이어가 이동할 때의 속도|
|공격범위|AttackRange|몬스터를 공격할 때의 공격하는 범위|
|공격속도|AttackSpeed|몬스터를 공격할 떄의 공격속도|
|반격기시간|CounterCoolDown|몬스터의 강한 공격을 받아치는 반격기의 재사용 시간|
|회피시간|EvadeCoolDown|짧은 순간을 빠르게 이동할 때 쓰는 회피의 재사용 시간|
|무 스탯|RadishStatus|무를 많이 재배할수록 무의 공격력 크게 증가|
|대파 스탯|GreenOnionStatus|대파를 많이 재배할수록 대파의 공격력과 공격속도 증가|
|오이 스탯|Cucumber|오이를 많이 재배할수록 오이의 공격력과 공격속도 증가|
|고추 스탯|PepperStatus|고추를 많이 재배할수록 고추의 공격속도 크게 증가|
|작물 스탯|CropsStatus|작물을 많이 재배할수록 체력이 증가|

<br>

## 게임의 규칙

> ### 1) 핵심 규칙
플레이어는 하루마다 농사를 하거나 몬스터를 사냥할 수 있다. 몬스터에게 공격을 당하면 피가 줄어들게 되고 0이 될시 하루가 시작되는 날로 이동(초기화)하게 된다. 플레이어가 몬스터를 사냥하기 위해서는 밭에서 사냥맵으로 이동하여야 한다. 스테이지는 총 3개가 있으며 다음 스테이지로 넘어가기 위해서는 해당 스테이지의 보스를 처치해야 다음 스테이지로
넘어갈 수 있다. 마지막 스테이지를 클리어가 되면 플레이어의 최종 승리가 되며 엔딩 씬으로 넘어간다.

> ### 2) 보조 규칙
플레이어는 하루마다 작물을 밭에서 키울 수 있으며 하루마다 물을 주면 성장하며 물을 주지 않을 경우에는 자라지
않는다. 작물이 다 자라면 플레이어는 재배하여 무기로 사용할 수가 있다. 작물마다 능력치가 다르며 해당 작물마다 재배량에 따라 능력치가 상승이 된다. 플레이어가 피가 없을때는 작물을 먹어 체력을 회복 시킬 수가 있지만 먹은 작물의 개수는 줄어들기 때문에 능력치가
하락이 될 수도 있다.
<br>

# [개발 요구사항과 흐름도]

## 요구사항

### 화면
> ● 시작화면
> 1. 처음 시작시 화면에서 게임시작 버튼과 게임종료 버튼이 있다. 
> 2. 게임시작 버튼을 클릭 시 게임 화면으로 넘어가게 된다. 
> 3. 게임종료 버튼을 클릭 시 게임을 종료하게 된다. 
>
> ● 게임화면
> 1. 시작화면에서 게임화면으로 넘어가게 되면 조작키를 알려주는 안내창이 뜨게 된다. 
> 2. 안내창을 닫게 되면 왼쪽 하단에 반격기와 회피기의 쿨타임을 알려주는 원이 있다. 
> 3. 왼쪽 상단에는 플레이어의 체력과 기력이 표시된다. 
> 4. 플레이어가 설정 키를 누르면 게임이 멈추며 설정 창이 나온다. 
> 5. 설정 창에는 조작키를 다시 알려주는 버튼, 돌아가기와 게임 종료 버튼이 있다. 
> 6. 플레이어가 인벤토리 키를 누르면 게임이 멈추며 인벤토리 창이 나온다.
> 7. 인벤토리 창에서 원하는 작물(무기)을 바꿔서 착용할 수 있으며 해당 작물의 갯수를 확인 할 수 있다.
> 8. 농장, 일반, 보스 맵 총 3가지의 맵을 만들어야 한다.
> 9. 기력창 아래에 해당하는 아이템의 갯수가 보인다.
> 10. 맵을 이동하는 포탈 연결
> 11. 플레이어의 체력이 0이되면 게임오버 씬으로 이동한다.

> ● 엔딩화면
> 1. 플레이어가 몬스터를 쓰러트리는 그림이 나오며 시작화면으로 돌아가는 버튼과 게임종료 버튼이 나온다. 
> 2. 돌아가는 버튼을 누르면 시작화면으로 넘어가게 된다. 
> 3. 게임종료 버튼을 누르면 게임이 종료된다. 

### 몬스터
> ● 일반 몬스터
> 1. ~~플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다.~~ => 플레이어에게 피격당한 몬스터는 플레이어를 공격하러 온다. 
> 2. 플레이어가 몬스터를 때리면 해당 몬스터의 체력바가 나온다. (때리기 전까지는 체력이 보이지 않는다.)
> 3. 플레이어를 공격하러 온 몬스터가 일정 거리를 벗어나게 되면 자신이 있던 자리로 이동하게 된다. 
> 4. 몬스터를 처치하게 되면 몬스터를 사라지며 골드가 나와 플레이어의 몸으로 들어간다. 
> 5. 몬스터끼리 거리가 가까워지면 서로 멀어진다.
> 6. 플레이어가 공격을 하면 해당 몬스터의 패턴을 사용한다.
> 7. 일반 몬스터는 스포너 인근을 돌아다닌다. 
> 8. 몬스터의 체력이 0이 되면 몬스터는 사라진다.    
> 9. 몬스터가 피격을 당한 후 플레이어를 추격할때의 속도를 2배로 증가

> ● 보스 몬스터
> 1. 플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다. 
> 2. 플레이어가 몬스터를 때리면 일반 몬스터와는 다르게 가운데 상단에 보스 몬스터의 이름과 체력이 뜬다. 
> 3. 플레이어의 위치가 어디에 있든 공격을 시작한 보스 몬스터는 맵을 벗어나지 않은 이상 계속 따라오게 된다. 
> 4. 해당 보스 몬스터를 처치하게 되면 대량의 골드와 막혀있던 맵을 통과 할 수 있게 된다. 
> 5. 마지막 보스 몬스터를 처치하면 게임이 클리어가 되며 엔딩화면으로 넘어가게 된다.
> 6. 플레이어가 공격을 하면 보스 몬스터는 패턴을 사용한다.
> 7. 몬스터의 체력이 0이 되면 몬스터는 사라진다.

### 플레이어
> 1. 플레이어는 하루마다 농장의 집에서 잠을 자게 되며 자고 난 후 아침마다 자동 세이브가 된다.
> 2. 플레이어의 HP가 다 소모하면 쓰러지게 되고 엔딩 씬으로 가는 것이 아닌 전날 아침으로 돌아가게 된다.
> 3. Hp는 농장에서 천천히 차며, 사냥터에서는 작물을 먹어야 회복시킬 수 있다.
> 4. 플레이어는 Sp(기력)를 다 소모한다면 회피나 반격, 공격, 뛰기를 할 수 없다.
> 5. Sp는 농장에서나 사냥터에서나 상관없이 초당1씩 자동으로 차게 된다.
> 6. 플레이어가 Sp소모를 하는 동안에는 Sp가 차지 않게 된다.
> 7. 회피를 사용하는 동안에는 무적이 되어 몬스터의 공격을 피할 수 있다.
> 8. 화살표(→, ←, ↑, ↓)로 상하좌우를 움직일 수 있다.
> 9. 카메라는 플레이어를 따라 움직인다.
> 10. LShift를 누를시 뛰기, Space Bar를 누를시 회피를 시전한다.
> 11. 플레이어는 공격과 반격기를 사용할 수 있다.

### 작물
> 1. 작물마다 물을 줘야하는 횟수가 다르다. (무 5회, 대파 3회, 오이 2회, 고추 1회)
> 2. 하루마다 작물에 물을 주지 않을 경우 해당 작물의 물을 주는 횟수가 깍아지않는다.
> 3. 작물은 3일 마다 상인에게 몬스터를 잡고 나면 주는 골드로 씨앗과 교환할 수 있다.
> 4. 작물마다 공격력, 공격속도, 공격범위가 다르다.    

## 키보드 이벤트에 대한 흐름도

![게임프로젝트2 게임 흐름도](https://user-images.githubusercontent.com/114119404/196718239-07a3f7d6-0fe0-47c8-8eb3-087c00c0be20.png)

## 스토리 보드

![게임프로젝트2](https://user-images.githubusercontent.com/114119404/196827008-fdfe783d-cfe4-4481-a9c1-643e56689b54.png)

# [프로토타입 개발 요구사항]

### 화면
> ● 시작화면
> 1. 처음 시작시 화면에서 게임시작 버튼과 게임종료 버튼이 있다. 
> 2. 게임시작 버튼을 클릭 시 게임 화면으로 넘어가게 된다. 
> 3. 게임종료 버튼을 클릭 시 게임을 종료하게 된다. 
>
> ● 게임화면    
> 1. 왼쪽 하단에 반격기와 회피기의 쿨타임을 알려주는 원이 있다.     
> 2. 왼쪽 상단에는 플레이어의 체력과 기력이 표시된다. 
> 3. 플레이어가 설정 키를 누르면 게임이 멈추며 설정 창이 나온다. 
> 4. 설정 창에는 돌아가기와 게임 종료 버튼이 있다. 
> 5. 플레이어가 인벤토리 키를 누르면 게임이 멈추며 인벤토리 창이 나온다.
> 6. 인벤토리 창에서 원하는 작물(무기)을 바꿔서 착용할 수 있다.
> 7. 기력창 아래에 해당하는 아이템의 갯수가 보인다.
> 8. 맵을 이동하는 포탈 연결
> 9. 농장, 일반, 보스 맵 총 3가지의 맵을 만들어야 한다.
> 10. 플레이어의 체력이 0이되면 게임오버 씬으로 이동한다.

### 몬스터
> ● 일반 몬스터
> 1. ~~플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다.~~ => 플레이어에게 피격당한 몬스터는 플레이어를 공격하러 온다. 
> 2. 플레이어를 공격하러 온 몬스터가 일정 거리를 벗어나게 되면 자신이 있던 자리로 이동하게 된다. 
> 3. 몬스터끼리 거리가 가까워지면 서로 멀어진다.
> 4. 플레이어가 공격을 하면 해당 몬스터의 패턴을 사용한다.
> 5. 일반 몬스터는 스포너 인근을 돌아다닌다. 
> 6. 몬스터가 피격을 당한 후 플레이어를 추격할때의 속도를 2배로 증가
> 7. 몬스터의 체력이 0이 되면 몬스터는 사라진다. 

> ● 보스 몬스터
> 1. 플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다. 
> 2. 플레이어가 몬스터를 때리면 일반 몬스터와는 다르게 가운데 상단에 보스 몬스터의 이름과 체력이 뜬다. 
> 3. 플레이어의 위치가 어디에 있든 공격을 시작한 보스 몬스터는 맵을 벗어나지 않은 이상 계속 따라오게 된다. 
> 4. 플레이어가 공격을 하면 보스 몬스터는 패턴을 사용한다.

### 플레이어
> 1. Hp는 농장에서 천천히 차며, 사냥터에서는 작물을 먹어야 회복시킬 수 있다.
> 2. 플레이어는 Sp(기력)를 다 소모한다면 회피나 반격, 공격, 뛰기를 할 수 없다.
> 3. Sp는 농장에서나 사냥터에서나 상관없이 초당1씩 자동으로 차게 된다..
> 4. 플레이어가 Sp소모를 하는 동안에는 Sp가 차지 않게 된다.
> 5. 회피를 사용하는 동안에는 무적이 되어 몬스터의 공격을 피할 수 있다.
> 6. 화살표(→, ←, ↑, ↓)로 상하좌우를 움직일 수 있다.
> 7. 카메라는 플레이어를 따라 움직인다.
> 8. LShift를 누를시 뛰기, Space Bar를 누를시 회피를 시전한다.
> 9. 플레이어는 공격과 반격기를 사용할 수 있다.

### 작물
> 1. 작물마다 공격력, 공격속도, 공격범위가 다르다.

# [프로토타입 개발작업 일정]

<details>
<summary> 일정 열기 </summary>

### 1주차 ( 일반 몬스터와 플레이어관련 구현 )

#### 몬스터
> ● 일반 몬스터
> 1. 몬스터끼리 거리가 가까워지면 서로 멀어진다.

#### 플레이어
> 1. 화살표(→, ←, ↑, ↓)로 상하좌우를 움직일 수 있다.
> 2. 카메라는 플레이어를 따라 움직인다.

### 2주차 ( 일반 몬스터와 플레이어의 이동 관련 구현 )

#### 몬스터
> ● 일반 몬스터
> 1. 플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다. 
> 2. 일반 몬스터는 스포너 인근을 돌아다닌다. 
> 3. 플레이어를 공격하러 온 몬스터가 일정 거리를 벗어나게 되면 자신이 있던 자리로 이동하게 된다. 

#### 플레이어
> 1. 플레이어는 Sp(기력)를 다 소모한다면 회피나 반격, 공격, 뛰기를 할 수 없다.
> 2. Sp는 농장에서나 사냥터에서나 상관없이 초당1씩 자동으로 차게 된다..
> 3. LShift를 누를시 뛰기, Space Bar를 누를시 회피를 시전한다.

### 3주차 ( UI관련 구현 )

#### 화면
> ● 시작화면
> 1. 처음 시작시 화면에서 게임시작 버튼과 게임종료 버튼이 있다. 
> 2. 게임시작 버튼을 클릭 시 게임 화면으로 넘어가게 된다. 
> 3. 게임종료 버튼을 클릭 시 게임을 종료하게 된다. 
>
> ● 게임화면    
> 1. 왼쪽 하단에 반격기와 회피기의 쿨타임을 알려주는 원이 있다.     
> 2. 왼쪽 상단에는 플레이어의 체력과 기력이 표시된다. 
> 3. 플레이어가 설정 키를 누르면 게임이 멈추며 설정 창이 나온다. 
> 4. 설정 창에는 돌아가기와 게임 종료 버튼이 있다. 

#### 플레이어
> 1. 플레이어는 공격과 반격기를 사용할 수 있다.

### 4주차 ( 일반 몬스터의 패턴과 플레이어관련 구현 )

#### 몬스터
> ● 일반 몬스터    
> 1. 플레이어가 공격을 하면 해당 몬스터의 패턴을 사용한다.    
> 2. 몬스터가 피격을 당한 후 플레이어를 추격할때의 속도를 2배로 증가    

#### 화면
> ● 게임화면
> 1. 플레이어가 인벤토리 키를 누르면 게임이 멈추며 인벤토리 창이 나온다.
> 2. 인벤토리 창에서 원하는 작물(무기)을 바꿔서 착용할 수 있다.
> 3. 기력창 아래에 해당하는 아이템의 갯수가 보인다.

#### 플레이어
> 1. 회피를 사용하는 동안에는 무적이 되어 몬스터의 공격을 피할 수 있다.
> 2. Hp는 농장에서 천천히 차며, 사냥터에서는 작물을 먹어야 회복시킬 수 있다.

#### 작물
> 1. 작물마다 공격력, 공격속도, 공격범위가 다르다.

### 5주차 ( 보스, 일반 몬스터와 패턴관련 구현 )

#### 몬스터
> ● 일반 몬스터
> 1. 몬스터의 체력이 0이 되면 몬스터는 사라진다.     
> 2. 플레이어가 공격을 하면 해당 몬스터의 패턴을 사용한다.

> ● 보스 몬스터
> 1. 플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다. 
> 2. 플레이어가 몬스터를 때리면 일반 몬스터와는 다르게 가운데 상단에 보스 몬스터의 이름과 체력이 뜬다. 
> 3. 플레이어의 위치가 어디에 있든 공격을 시작한 보스 몬스터는 맵을 벗어나지 않은 이상 계속 따라오게 된다. 
> 4. 플레이어가 공격을 하면 보스 몬스터는 패턴을 사용한다.

### 6주차

#### 화면
> ● 게임화면
> 1. 농장, 일반, 보스 맵 총 3가지의 맵을 만들어야 한다.
> 2. 맵을 이동하는 포탈 연결
> 3. 플레이어의 체력이 0이되면 게임오버 씬으로 이동한다.
 
</details>


# [프로토타입 주차별 구현 과정]    

<details>
<summary> 1주차 </summary>
    
 
#### 플레이어
> 1. ~~화살표(→, ←, ↑, ↓)로 상하좌우를 움직일 수 있다.(100%)~~
> 2. ~~카메라는 플레이어를 따라 움직인다. (100%)~~

#### 몬스터
> ● 일반 몬스터
> 1. ~~몬스터끼리 거리가 가까워지면 서로 멀어진다. (100%)~~

#### 작업 내용
1. 일단 플레이어와 몬스터의 스프라이트를 추가하지 않은 상태의 게임 오브젝트(박스형태)를 만들고 스크립트를 작성하여 구현할 것

#### 구현 사진
![게임프로젝트8주차구현 (1)](https://user-images.githubusercontent.com/114119404/207600984-02d7cbe9-f07a-41d0-977f-7d27a4681a63.gif)    
플레이어가 네모 몬스터가 원으로 플레이어를 화살표4방향으로 상하좌우를 움직이고 몬스터를 서로 가까이 가면 서로 멀어지게 구현하였다.
 
</details>
    
<details>
<summary> 2주차 </summary>

#### 몬스터
> ● 일반 몬스터
> 1. ~~플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다. (100%)~~
> 2. ~~일반 몬스터는 스포너 인근을 돌아다닌다. (100%)~~
> 3. ~~플레이어를 공격하러 온 몬스터가 일정 거리를 벗어나게 되면 자신이 있던 자리로 이동하게 된다. (100%)~~

#### 플레이어
> 1. ~~플레이어는 Sp(기력)를 다 소모한다면 회피나 반격, 공격, 뛰기를 할 수 없다. (100%)~~
> 2. ~~Sp는 농장에서나 사냥터에서나 상관없이 초당1씩 자동으로 차게 된다. (100%)~~
> 3. ~~LShift를 누를시 뛰기, Space Bar를 누를시 회피를 시전한다. (100%)~~

#### 작업 내용
1. 일반 몬스터는 플레이어를 쫓을 때, 스포너 위치로 이동할 때에는 서로 충돌을 하지 않는다.
2. 일반 몬스터는 랜덤으로 숫자를 받아서 그에 해당하는 숫자에 따라서 이동을 하거나 가만히 서 있는다.
3. 플레이어는 기력이 계속 차게 되지만 뛰거나 회피를 하는 도중에는 기력이 차지 않는다.
4. 플레이어 3번 구현 내용 중 공격과 반격을 시전한다는 말이 없었기에 공격과 반격은 구현하지 않았다. (후에 구현할 예정)

#### 구현 
![게임프로젝트9주차구현](https://user-images.githubusercontent.com/114119404/207601229-fcb1d24d-bd46-455e-b749-382fb8f0b476.gif)    
플레이어가 네모 몬스터가 원으로 플레이어가 몬스터의 범위안에 들어가게 되면 플레이어를 추격하도록 구현하였다. 또,
몬스터를 원안에 들어가게 되면 일정 시간마다 이동하도록 구현하였다.
 
</details>
    
 
<details>
<summary> 3주차 ( UI관련 구현 ) </summary>

#### 화면
> ● 시작화면       
> ~~처음 시작시 화면에서 게임시작 버튼과 게임종료 버튼이 있다. (100%)~~     
> ~~게임시작 버튼을 클릭 시 게임 화면으로 넘어가게 된다. (100%)~~    
> ~~게임종료 버튼을 클릭 시 게임을 종료하게 된다. (100%)~~     
> ● 게임화면        
> ~~왼쪽 하단에 반격기와 회피기의 쿨타임을 알려주는 원이 있다. (100%)~~     
> ~~왼쪽 상단에는 플레이어의 체력과 기력이 표시된다. (100%)~~    
> ~~플레이어가 설정 키를 누르면 게임이 멈추며 설정 창이 나온다. (100%)~~    
> ~~설정 창에는 돌아가기와 게임 종료 버튼이 있다. (100%)~~    

#### 플레이어    
> ~~플레이어는 공격과 반격기를 사용할 수 있다. (100%)~~

#### 작업 내용
1. 게임 시작 씬을 추가하여 간단한 버튼 2개를 만들어 게임을 시작하게 하는 버튼과 게임을 종료하게 하는 버튼을 구현한다.
2. 반격기와 회피기의 쿨타임을 알려주는 원이 있는데 기술을 사용 시 해당하는 원이 돌아가면서 색을 채워지게 구현한다.
3. 설정 키는 ESC로 누를 시에 게임의 시간을 정지시키고 가운데 정면에 설정 창이 나온다.
4. 설정 창에는 돌아가기와 게임 종료 버튼이 존재하고 돌아가기를 누를 시 설정 창이 꺼지며 게임의 시간이 다시 재생이 된다. 또, 게임 종료 버튼을 누를 시에 게임이 종료가 된다.
5. 플레이어가 최근 방향을 기준으로 공격을 하며 반격기 또한 동일하게 구현한다. (반격기의 애니메이션 문제로 지금은 일반 공격과 똑같은 애니메이션을 사용)
6. 체력은 빨간색 기력은 노란색으로 되어있으며 증가하거나 감소한다.

#### 구현 사진
![겜프2](https://user-images.githubusercontent.com/114119404/207601627-ef87e777-859e-4d74-b29b-51031807c56f.gif)    
처음 인트로씬으로 게임시작버튼과 게임종료버튼이 있고 게임시작버튼을 누를시 게임이 시작된다.

![겜프3](https://user-images.githubusercontent.com/114119404/207601643-819be75a-58d6-4c10-be08-f6561f4e6616.gif)    
플레이어의 체력이 줄어드는것을 볼 수 있게 실시간으로 줄어들게 해놨으며, 플레이어가 LShift(뛰기)를 사용하면 스태미나가 줄어들고 빠른속도로 이동하게 된다.
또, 카운터와 회피를 사용하면 왼쪽하단에 쿨타임이 줄어들어 플레이어가 확인할 수 있게 구현하였다.

![겜프1](https://user-images.githubusercontent.com/114119404/207601652-7ef9e2e0-0f3f-4b25-946c-39e9d4634687.gif)    
플레이어가 ESC(설정)키를 누르면 설정 창이 나오게 되고 게임을 종료할 수 있게 버튼을 만들어 플레이어가 원할 때 종료하도록 구현하였다.
 
</details>
    
 
<details>
<summary> 4주차 ( 일반 몬스터의 패턴과 플레이어관련 구현 ) </summary>

#### 몬스터
> ● 일반몬스터    
> ~~플레이어가 공격을 하면 해당 몬스터의 패턴을 사용한다. (100%)~~   
> ~~몬스터가 피격을 당한 후 플레이어를 추격할때의 속도를 2배로 증가 (100%)~~

#### 화면
> ● 게임화면        
> ~~플레이어가 인벤토리 키를 누르면 게임이 멈추며 인벤토리 창이 나온다. (100%)~~   
> ~~인벤토리 창에서 원하는 작물(무기)을 바꿔서 착용할 수 있다. (100%)~~   
> ~~기력창 아래에 해당하는 아이템의 갯수가 보인다. (100%)~~   

#### 플레이어    
> ~~회피를 사용하는 동안에는 무적이 되어 몬스터의 공격을 피할 수 있다. (100%)~~   
> ~~Hp는 농장에서 천천히 차며, 사냥터에서는 작물을 먹어야 회복시킬 수 있다. (100%)~~

#### 작물
> ~~작물마다 공격력, 공격속도, 공격범위가 다르다. (100%)~~   

#### 작업 내용
1. 플레이어가 인벤토리 창에 들어가면 작물 5개가 나오고 클릭 시에 해당하는 무기를 장착한다.   
2. 해당하는 작물을 착용하면 기력바 아래에 해당하는 작물의 갯수가 나온다.(프로토 타입으로 10개로 정함)   
3. 2번과 동일하게 작물을 착용하면 플레이어의 공격과 공격속도, 공격범위가 다르게 구현한다.   
4. 플레이어가 몬스터를 공격을 하면 몬스터가 플레이어에게 공격 패턴을 사용한다.   

#### 추가로 작업한 내용 (주차 별에 미비된 사항은 해당 퍼센트 100%로 변경)    
1. 1주차에서의 카메라가 플레이어를 따라 움직이게 구현   
2. 2주차에서의 플레이어의 기력이 소진되면 공격, 반격, 회피, 뛰기를 할 수 없게 구현   
3. 3주차에서의 플레이어는 공격과 반격에서 반격을 공격과 다르게 애니메이션 수정   
4. Hp는 농장에서 천천히 차며, 사냥터에서는 작물을 먹어야 회복시킬 수 있다. ( 요구사항에 있었던 내용으로 추가가 안되서 )
5. 몬스터가 피격을 당한 후 플레이어를 추격할때의 속도를 2배로 증가

#### 변경된 내용
1. 2주차에서의 플레이어 인근에 몬스터가 도달하면 쫓아간다 => 몬스터가 피격을 당하면 플레이어를 쫓아간다.
2. 기력바 아래에 작물의 갯수를 10개에서 5개로 변경

#### 미비된 내용
1. 작물마다의 공격범위 보완
2. 작물을 인벤토리에서 선택할 때마다 해당하는 작물의 갯수로 변경되게 수정
3. 일반 몬스터의 추가와 패턴 추가
4. 농장을 아직 따로 만들지 않아 자동 회복을 따로 구현하지 않았기 때문에 구현해야함

#### 구현한 내용    
![플레이어 인벤토리 구현 및 작물 공격속도](https://user-images.githubusercontent.com/114119404/207606151-c6c40a35-fa6c-4d47-bf57-ed82eb02aecb.gif)    
플레이어가 E(인벤토리)를 누를시 인벤토리 창이 뜨고 해당하는 작물을 클릭하면 장착을 하게된다. 또, 장착하는 작물마다 공격력과 공격속도가 다르다.

![몬스터 피격시 몬스터의 추력과 회피 무적 구현](https://user-images.githubusercontent.com/114119404/207606168-3ec13ea2-d2c5-43f0-9634-30f93cabd470.gif)    
플레이어가 몬스터를 공격시 몬스터가 플레이어를 추격하며 도달 시에 패턴을 사용하고 플레이어가 회피를 사용하면 피해를 입지 않게 구현하였다.
 
</details>
    
 
<details>
<summary> 5주차 ( 보스, 일반 몬스터와 패턴관련 구현 ) </summary>
 
#### 몬스터
> ● 일반 몬스터    
> ~~몬스터의 체력이 0이 되면 몬스터는 사라진다. (100%)~~    
> ● 보스 몬스터    
> ~~플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다. (100%)~~    
> ~~플레이어가 몬스터를 때리면 일반 몬스터와는 다르게 가운데 상단에 보스 몬스터의 이름과 체력이 뜬다. (100%)~~      
> ~~플레이어의 위치가 어디에 있든 공격을 시작한 보스 몬스터는 맵을 벗어나지 않은 이상 계속 따라오게 된다. (100%)~~      
> ~~플레이어가 공격을 하면 보스 몬스터는 패턴을 사용한다. (100%)~~     

#### 보완한 내용
1. ~~작물마다의 공격범위 보완 (100%)~~
2. ~~작물을 인벤토리에서 선택할 때마다 해당하는 작물의 갯수로 변경되게 수정 (100%)~~
3. ~~일반 몬스터의 추가와 패턴 추가 (100%)~~

#### 작업 내용    
1. 일반 몬스터의 체력이 플레이어의 공격으로 0이하가 되면 죽어서 사라지게된다.    
2. 플레이어가 보스 몬스터를 공격할 시  보스 몬스터가 플레이어를 추격하며 화면 상단 가운데에 보스의 이름과 체력이 나오는 UI구현    
3. 보스 몬스터가 플레이어를 추격하는 도중 플레이어가 해당 맵을 나가게 되면 쫓아가지 않게 구현 및 보스 몬스터의 체력 100%로 변경    
4. 보스 몬스터가 플레이어에게 피격을 당하면 랜덤 패턴 3개 중 1개를 랜덤으로 사용한다.    

#### 변경된 내용
1.이번 주차 보스 몬스터의 2번째 구현인 보스가 플레이어 위치 근처에 있다면 플레이어를 공격하게 구현 => 플레이어가 공격할 시에 공격하게 구현    

#### 미비된 내용
1. 보스 몬스터 UI 구현
2. 보스 추가 패턴 2~3개 구현

#### 구현한 내용    
![작물 갯수 차별화와 일반 몬스터 추가와 패턴 추가](https://user-images.githubusercontent.com/114119404/207602078-ecced472-3d32-4496-b83a-4f26585ab250.gif)    
플레이어가 작물을 먹게 되면 해당하는 무기의 갯수가 줄어들게 구현을 하였으며 일반 몬스터를 추가하였고 몬스터의 패턴을 추가하였다.

![보스 추가 및 패턴 1개 추가](https://user-images.githubusercontent.com/114119404/207602106-97d06545-7034-4d10-bee1-d083a3c30885.gif)    
보스를 추가를 하였고 플레이어가 보스를 공격하면 플레이어를 공격하는 패턴을 사용한다.
 
</details>
    
 
<details>
<summary> 6주차 </summary>
 
 #### 화면
> ● 게임화면
> 1. ~~농장, 일반, 보스 맵 총 3가지의 맵을 만들어야 한다. (100%)~~
> 2. ~~맵을 이동하는 포탈 연결 (100%)~~
> 3. ~~플레이어의 체력이 0이되면 게임오버 씬으로 이동한다. (100%)~~

#### 보완한 내용
1. ~~보스 몬스터 UI 구현 (100%)~~
2. ~~보스 추가 패턴 2~3개 구현 (100%)~~
3. ~~플레이어가 농장에 있을 때 체력 자동 회복을 구현 (100%)~~

#### 작업한 내용
1, 일반 몬스터 포탈 이용시 공격 금지 및 자신의 영역으로 이동 구현    
2. 농장과 사냥터 이동하게 구현    
4. 보스몬스터 패턴 2개 추가    
5. 농장맵 추가 및 사냥터와 보스맵 구현    
6. 농장에서 플레이어의 작물 갯수 최대 값으로 변경    
7. 농장에서 플레이어의 체력이 계속 증가하게 구현    

#### 미비된 내용
1. 플레이어의 체력이 0되면 게임오버 씬으로 이동하는 것을 하지 못함

#### 구현한 내용    
![보스와 일반 몬스터 포탈로 인한 공격 중지](https://user-images.githubusercontent.com/114119404/207602328-d2ab3f81-9d12-444e-aed2-943ca23bcb93.gif)    
플레이어가 전투 중 포탈을 타고 가면 보스와 일반 몬스터가 공격을 중지하게 구현한 내용이다.

![농장에서 작물 갯수 초기화 및 체력 계속 증가](https://user-images.githubusercontent.com/114119404/207602355-2d4c6b4b-df1c-4d0f-a86b-95157b8189b1.gif)    
농장에서는 플레이어의 체력이 프레임마다 1씩 차오르고 작물의 갯수는 최대 값으로 바뀌게 된다.

![보스몬스터 패턴](https://user-images.githubusercontent.com/114119404/207602377-dd8a842b-a25f-48e2-a908-0b24124c1f83.gif)    
보스의 패턴으로 사진과 같이 공격을 한다.
 
</details>
    

<details>
<summary> 7주차( 보강주차 ) </summary>    

#### 화면
> ● 게임화면
> 1. ~~플레이어의 체력이 0이되면 게임오버 씬으로 이동한다. (100%)~~

#### 보완한 내용
1. ~~보스 패턴 보완 (100%)~~
2. ~~플레이어의 체력이 0되면 게임오버 씬으로 이동하는 것을 하지 못함 (100%)~~

#### 추가로 구현한 내용    
1. 보스 패턴 중 파티클 추가    

#### 작업한 내용
1. 보스의 두번째 패턴 사용 후 플레이어와 충돌시 두번째 스킬의 장판이 다시 생성되는 버그 수정
2. 보스의 세번째 패턴 사용 중에 플레이어가 보스에게 카운터 시전시 파티클이 나오게 구현

#### 구현한 내용
![플레이어 죽음](https://user-images.githubusercontent.com/114119404/207613179-c0c61b82-2be5-45d5-bc68-d260ac9fc7be.gif)      
플레이어의 체력이 0이되면 게임오버씬으로 넘어가게 되고 게임종료버튼을 누를시 게임을 나가게 된다.

![보스 파티클 추가](https://user-images.githubusercontent.com/114119404/207613187-5c4771a7-177b-408f-b7f7-03d8b502890e.gif)    
보스의 세번째 패턴 사용 중에 플레이어가 보스의 앞에서 카운터 사용시 파티클이 나오게 구현하였다.
 
</details>
    
 
# [포트폴리오 개발작업 일정]    

<details>
<summary> 일정 열기 </summary>
     
1~2주차 <br/> 
OT 및 포트폴리오 계획서 및 발표 자료 준비     
     
<br/>
 
3주차 <br/> 
1. 프로토타입 프로젝트 버그 수정
2. 코드 최적화
     
<br/>
 
> 4주차 <br/> 
1. 오이로 공격시 오이가 회전하면서 날라가며 몬스터가 맞을시 피해 입게 구현 <br/> 
2. 고추로 공격시 고추가 일직선으로 날라가며 몬스터가 맞을시 피해 입게 구현 <br/> 
3. 플레이어가 D키를 누르면 플레이어 정면으로 물통이 나오고 위에서 아래로 흐르게 구현 <br/> 
4. 무와 대파는 공격시 횟수당 갯수가 줄어들게, 오이와 고추는 공격시 갯수가 줄어들게 구현 <br/> 

<br/>    
5주차 <br/> 
1. 고추와 오이로 일반 몬스터 피격시 몬스터가 뒤로 물러나게 구현 <br/> 
2. 해당 작물의 갯수가 다 사라지면 손에서 사라지게 구현 <br/> 
3. 작물의 갯수가 다 사라지면 공격을 할 수 없게 구현 <br/> 
 
<br/>    
 
6주차 <br/> 
1. 일반 스테이지 변경 (일반 몬스터 1종 추가할 자리와 원래 몬스터 자리 변경) <br/> 
2. 일반 스테이지 1개 추가 (두번째 스테이지) <br/> 
3. 일반 몬스터 알파카, 염소 2종 구현 <br/> 
 
<br/>    
 
7주차 <br/> 
1. 일반 몬스터 돼지, 양 2종 구현 <br/> 
2. 돼지, 양 2스테이지로 배정 <br/> 
 
<br/>    
 
8주차 <br/> 
중간고사로 미 기입 <br/> 
 
<br/>    
 
</details>
 
# [포트폴리오 주차별 구현 과정]

## 버그 수정 내용 (해당 주차에 일어난 수정한 내용은 기입하지 않음)       
 
1. 오이 무기 회전이 자연스럽지 않게 반대로 회전하는 버그     
상황: 해결 / 3월 31일 오전 1시 34분    

2. 닭 몬스터 패턴 사용 중일 때 포탈 이동 시 패턴이 안끓기고 계속 커지는 버그    
상황: 해결 / 3월 31일 오전 3시 10분    
 
3. 일반 몬스터 자동 이동시 좌우반동 심한 버그    
상황: 해결 / 3월 31일 오전 3시 26분    
 
4. 플레이어의 작물이 0이 되어도 공격이 되는 버그    
상황: 해결 못함     

<details>
<H4> <summary> 1주차 </summary>    
 
포트폴리오 OT
 
</details>

 
<details>
<summary> 2주차 </summary>    
 
포트폴리오 계획서 제작 및 발표
 
</details>
 
  
<details>
<summary> 3주차 </summary>
    
프로토타입 프로젝트에서 코드 수정 및 피드백

피드백 내용
1. 고추, 오이, 대파, 무에서 고추와 오이를 원거리 무기로 변경함
2. 물을 뿌리는 에셋이 없어 물통을 키 입력시 나온다음 물 파티클이 아래로 흐르도록 함
3. 작물이 없을시 사라지고 공격을 못하게 함
 
</details>

<details>
<summary> 4주차 </summary>

 
 
</details>

 
<details>
<summary> 5주차 </summary>
 

 
</details>

 
<details>
<summary> 6주차 </summary>
 

 
</details>


<details>
<summary> 7주차 </summary>

 
</details>

 
