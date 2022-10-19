# 프로젝트명: Hunter Farmer / 개발자: 이재형

# [ 목차 ]
### 1. [컨셉](#컨셉)
### 2. [관련 이미지와 동영상](#관련-이미지와-동영상)
### 3. [대표 이미지의 컨셉과 기반 작품 묘사](#대표-이미지의-컨셉과-기반-작품-묘사)
### 4. [Hunter Farmer의 구성 요소](#Hunter-Farmer의-구성-요소)
### 5. [게임 시스템 디자인](#게임-시스템-디자인)
### 6. [개발 요구사항과 흐름도](#개발-요구사항과-흐름도)

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
 Adult(MDuck, WDuck, Pig, WChicken, MChicken, Goat, Sheep,)

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
넘어갈 수 있다. 마지막 스테이지를 클리어가 되면 플레이어의 최종 승리가 되며 엔딩 크레딧 씬으로 넘어간다.

> ### 2) 보조 규칙
플레이어는 하루마다 작물을 밭에서 키울 수 있으며 하루마다 물을 주면 성장하며 물을 주지 않을 경우에는 자라지
않는다. 작물이 다 자라면 플레이어는 재배하여 무기로 사용할 수가 있다. 작물마다 능력치가 다르며 해당 작물마다 재배량에 따라 능력치가 상승이 된다. 플레이어가 피가 없을때는 작물을 먹어 체력을 회복 시킬 수가 있지만 먹은 작물의 개수는 줄어들기 때문에 능력치가
하락이 될 수도 있다.
<br>

# [개발 요구사항과 흐름도]

## 요구사항

> ### 화면
1) 게임화면
1. 처음 시작시 화면에서 게임시작 버튼과 게임종료 버튼이 있다.
2. 게임시작 버튼을 클릭 시 게임 화면으로 넘어가게 된다.
3. 게임종료 버튼을 클릭 시 게임을 종료하게 된다.

2) 게임화면
1. 시작화면에서 게임화면으로 넘어가게 되면 조작키를 알려주는 안내창이 뜨게 된다.
2. 안내창을 닫게 되면 왼쪽 하단에 반격기와 회피기의 쿨타임을 알려주는 원이 표시가 된다.
3. 

3) 엔딩화면
1. 
2. 
3. 

> ### 몬스터
1. 플레이어 위치에 근접한 몬스터는 플레이어를 공격하러 온다.
2. 플레이어를 공격하러 온 몬스터가 일정 거리를 벗어나게 되면 자신이 있던 자리로 이동하게 된다.
3. 몬스터를 처치하게 되면 

## 키보드 이벤트에 대한 흐름도

![게임프로젝트2 게임 흐름도](https://user-images.githubusercontent.com/114119404/196498045-068b077d-0aa1-4082-888f-451475ae763b.png)

## 스토리 보드

![스토리텔링](https://user-images.githubusercontent.com/114119404/196515063-f1a1d67b-8e23-4e34-b6c4-cef2d826e435.png)
