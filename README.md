# HomeWork-2

## 문제(1)

* Add quotes to ansible playbook
* 최고점 : 9
*  " 추가하기

<img src="https://user-images.githubusercontent.com/43926186/144050811-62c7367d-f62e-431a-9c2e-acf93b1d8650.png" width="60%" height="70%"/>
<img src="https://user-images.githubusercontent.com/43926186/144051040-9126b28d-b9a8-46c9-8443-16e887d1c248.png" width="60%" height="70%"/>

**입력**

<img src="https://user-images.githubusercontent.com/43926186/144051611-0e420868-6625-4093-96c4-1f055cdd1269.png" width="40%" height="50%"/>

* G를 먼저 눌러 파일의 마지막 줄로 이동한다
* W를 눌러 단어 단위로 앞으로 이동한다.
* i로 현재 위치에서 입력 모드로 시작한다.
* End로 라인 끝으로 이동하여 입력을 마치고 ZZ를 통해서 저장 후 나간다.

**솔루션 영상**

![과제#2-1](https://user-images.githubusercontent.com/43926186/144218122-872a7e9e-eaf6-43d1-b028-0e0efae5f6ba.gif)


## 문제(2)
  
* simple replacements
* 최고점 : 26
* sublime와 emacs글자를 vim으로 교체

<img src="https://user-images.githubusercontent.com/43926186/144103277-800a1ba7-8b21-4eed-bc72-2f2da9f801f1.png" width="60%" height="70%"/>
<img src="https://user-images.githubusercontent.com/43926186/144103337-0b07db84-7102-4810-aef6-a520037b74ec.png" width="60%" height="70%"/>

**입력**
    
<img src="https://user-images.githubusercontent.com/43926186/144102777-c53be938-e52d-4044-8dff-2a9e64238401.png" width="40%" height="50%"/>

* %s/str/replace/g : str -> replace로 치환함
* str은 sublime와 emacs다.
* sublime는 7글자인데 su부터 시작하는 글자 중 me로 끝나는(su.*me)글자를 찾으면 1글자 줄일 수 있다.
* \|를 이용하면 str을 두개를 줄 수 있다.
* g옵션은 한 행에 '원래 문자열'에 입력한 패턴이 여러번 나오면 전체를 변경한다.

**솔루션 영상**

![과제#2-2](https://user-images.githubusercontent.com/43926186/144224125-0d786f02-7de7-4024-9ca0-a5ef30599ede.gif)

## 문제(3)
  
* Satisfy the go linter
* 최고점 : 30
* 두개의 문장 추가하기

<img src="https://user-images.githubusercontent.com/43926186/144106186-ea6264d3-6123-46ac-acbb-4a4f582d957e.png" width="60%" height="70%"/>
<img src="https://user-images.githubusercontent.com/43926186/144106242-1b8df482-0b3f-4b3d-ae2d-57e6620efe15.png" width="60%" height="70%"/>

**입력**
    
<img src="https://user-images.githubusercontent.com/43926186/144106130-cce2ba66-e5ac-4b6c-8479-0464a2275261.png" width="40%" height="50%"/>

* 일단 Version이 있는 4행으로 이동함(가고싶은 라인 넘버 입력 후 G 입력 시 이동)
* yw : 현재 word의 끝까지 복사한다.
* O : 현재 라인을 다음 줄로 밀력 입력 모드를 시작 후 // 입력
* p로 복사 했던 Version 입력
* a : 현재 위치 다음 칸에서 입력 모드 시작하고 TODO입력
* Y : 현재 라인을 복사
* p : 현재 위치 다음에 붙여넣기
* 입력 후 밑으로 내려가서 Debug복사하여 위로 올라가 붙여 넣기
* 한칸 앞으로 옮겨 dw : 현재 wor의 끝까지 잘라내기 기능
* ZZ로 빠져나옴

**솔루션 영상**

![과제#2-3](https://user-images.githubusercontent.com/43926186/144224435-a57ebbf9-574e-4960-ac0c-a210f44f00a2.gif)


## 문제(4)
  
* Plotting some variables in python
* 최고점 : 57
* 1을 각 행의 숫자로 교체하고 k도 교체하기

<img src="https://user-images.githubusercontent.com/43926186/144106975-31539a29-c56d-40ae-9ab2-db970ed74f8d.png" width="60%" height="70%"/>
<img src="https://user-images.githubusercontent.com/43926186/144107024-52083dba-f081-491b-8796-f2d40b937d67.png" width="60%" height="70%"/>

**입력**
    
<img src="https://user-images.githubusercontent.com/43926186/144108039-1793aeb8-1982-4d90-8aff-c0b941beedb8.png" width="80%" height="90%"/>

* 먼저 y1을 변경하기 쉽게 텍스트 대치를 이용해 y1를 abs(y1)로 변경함
* 여기서 맨 아랫줄로 이동하는데 /k를 이용해 k위치로 이동 
* r : 한 글자만 바꿀 때 활용함
* 그리고 맨 위부터 텍스트 대치를 이용해 1을 각 라인의 맞는 숫자로 변경하면서 내려감

**솔루션 영상**

![과제#2-4](https://user-images.githubusercontent.com/43926186/144224617-42884a97-c2ee-47f9-906d-7e5d4dc07e06.gif)

## 문제(5)
  
* Python dataclassed
* 최고점 : 29
* fileds추가하기

<img src="https://user-images.githubusercontent.com/43926186/144108394-009cd45f-09bb-4255-aaf3-acacc6594704.png" width="60%" height="70%"/>
<img src="https://user-images.githubusercontent.com/43926186/144108446-5d18df12-376e-4cae-8d8c-672eb8f22ab8.png" width="60%" height="70%"/>

**입력**
    
<img src="https://user-images.githubusercontent.com/43926186/144109030-799aea76-f77e-4888-b47a-17ee3aca6dc9.png" width="40%" height="50%"/>

* 5G를 이용하여 5행으로 이동한다
* yw앞에 숫자를 입력하면 그만큼 얻어내는데 마지막행으로 이동하여 붙여넣기 함
* J : 현재행과 아래 행 결합 하여 한줄로 만듬
* 텍스트 대치를 이용해 : 부터 필요한 공간 만큼 설정 후 ,로 교체
* . : 문자 한개와 대치됨

**솔루션 영상**

gif


