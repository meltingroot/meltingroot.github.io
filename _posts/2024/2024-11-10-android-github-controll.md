---
title:  "[ Android Studio -Git ] 안드로이드 스튜디오와 Github 연동 (commit/push)"

categories: 
  - Git
tags:
  - Git
  - Github
  - Android Studio
toc: true
toc_label: "Github 연동"
toc_sticky : "true"
---
안드로이드 스튜디오에서 Github 계정을 등록하고 Github Repository를 연결하면 Commit/Push 기능을 이용하여 작성한 코드를 Github에 업로드할 수 있다. 이 기능을 이용함으로써 내가 작업한 코드의 변경 내용을 안드로이드 스튜디오를 통해 실시간으로 확인할 수 있으며, 버전 관리에도 용이하다.

## Step 1: Git 버전 확인 

### 1 - 1. Git 버전 확인
![1-1]({{ "/assets/images/20241110/1-1.png" | relative_url}})
* 안드로이드 스튜디오 → File → Settings

### 1 - 2.  File  → Settings
![1-2]({{ "/assets/images/20241110/1-2.png" | relative_url}})
1. Version Control 선택
2. Git 선택
3. test버튼 선택

**Note:** 현재의 깃 버전과 실행 테스트를 진행할 수 있음
{: .notice--info}


### 1 -  3  버전 확인 완료
![1-2]({{ "/assets/images/20241110/1-3.png" | relative_url}})
* git.exe의 경로를 입력

**Note:** 깃을 설치 후 프로젝트를 열면 똑똑한 안드로이드 스튜디오가 자동으로 path를 잡아줌
{: .notice--info}



## Step 2:  GitHub 계정과 연동
![2]({{ "/assets/images/20241110/2.png" | relative_url}})
1. Version Control
2. GitHub
3. add Account...



## Step 3: Authorize in GitHub
![3-1]({{ "/assets/images/20241110/3-1.png" | relative_url}})
* Authorize in GitHub 버튼을 선택하면 GitHub 계정을 인증해야 함

![3-2]({{ "/assets/images/20241110/3-2.png" | relative_url}})
1. 다음 해당 사용자 이름, 암호 입력창 출력
2. GitHub 계정을 입력 후, 로그인 버튼 선택

**Note:** 로그인이 성공하면 다행이지만...
{: .notice}



## Step 4: 로그인 문제가 발생 한 경우
![4-1]({{ "/assets/images/20241110/4-1.png" | relative_url}})
 
![4-2]({{ "/assets/images/20241110/4-2.png" | relative_url}})
* GitHub을 통해서 로그인
* Token으로 로그인
* GitHub Enterprise로 로그인

→ 총 세 가지 옵션이 있음. 그중에 토큰을 선택



## Step 5: Add GitHub Account 
![5]({{ "/assets/images/20241110/5.png" | relative_url}})



## Step 6: 토큰을 발급받기 위해 Git 이동
![6]({{ "/assets/images/20241110/6.png" | relative_url}})
* GitHub → Settings



## Step 7:  Developer settings
![7]({{ "/assets/images/20241110/7.png" | relative_url}})



## Step 8:  개인 액세스 토큰 선택
![8]({{ "/assets/images/20241110/8.png" | relative_url}})
1. 개인 액세스 토큰
2. 새 토큰 생성



## Step 9: 토큰 설정
![9]({{ "/assets/images/20241110/9.png" | relative_url}})
1. Expiration 30 days, Select scopes 설정 주의
2. repo, admin:org, gist 체크
3. 비밀번호를 입력 후 토큰 발급
4. 토큰 복사



## Step 10: 토큰으로 GitHub 계정 추가
![10]({{ "/assets/images/20241110/10.png" | relative_url}})
1. 5번 에서 뜨던 팝업창으로 이동 
2. 복사한 토큰 붙여 넣기
3. 계정 추가가 잘되었으면 위 그림과 같이 화면에 자신의 계정이 생성됨



## Step 11: Git Repository 생성
![11]({{ "/assets/images/20241110/11.png" | relative_url}})
* VCS → Create Git Repository


## Step 12: Create Git Repository
![12]({{ "/assets/images/20241110/12.png" | relative_url}})
1. VCS  →  Import into Version Control  →  Create Git Repository 선택 
2. 확인 선택



## Step 13: 실행 확인
![13]({{ "/assets/images/20241110/13.png" | relative_url}})
* 실행하고 나면 빨간색 글씨로 변함 → GitHub에 올라가지 않은 새로운/ 수정된 코드



## Step 14: Manager Remotes
![14]({{ "/assets/images/20241110/14.png" | relative_url}})
* Git → Manager Remotes



## Step 15: Git Remote 추가
![15]({{ "/assets/images/20241110/15.png" | relative_url}})
* + 버튼 선택


## Step 16: 리파지토리 경로 추가
![16]({{ "/assets/images/20241110/16.png" | relative_url}})
* 연결할 리파지토리 경로 입력



## Step 17: 리파지토리 경로 추가 확인
![17]({{ "/assets/images/20241110/17.png" | relative_url}})
* remote가 저장 성공되었다는 것을 확인


## Step 18: Commit
### 18 - 1. 체크버튼 선택
![18-1]({{ "/assets/images/20241110/18-1.png" | relative_url}})
* 상단 바에 체크 버튼을 선택

**Note:** 다른 방법 : VCS → Commit or VCS → Git → Commit directory
{: .notice--info}


### 18 - 2. Commit
![18-2]({{ "/assets/images/20241110/18-2.png" | relative_url}})
* Commit 할 파일 체크 → Commit


## Step 19: Push
![19]({{ "/assets/images/20241110/19.png" | relative_url}})

**Note:**  Commit 후 Push를 해줘야 GitHub 리파지토리에 반영됨
{: .notice--danger}