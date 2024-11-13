---
title:  "[ Android Studio -Git ] 안드로이드 스튜디오 깃허브 연동 하기 (commit/push)"

categories: 
  - Git
tags:
  - Git
  - Github
toc: true
toc_label: "Getting Started"
toc_sticky : "true"
---
안드로이드 스튜디오에서는 깃허브 연동 기능을 제공한다. 

안드로이드 스튜디오에서 깃허브 계정을 등록하고 깃허브 Repository를 연결하면 커밋과 푸시(Commit/Push) 기능을 이용하여 작성한 코드를 깃허브에 업로드할 수 있다. 

이 기능을 이용함으로써 내가 작업한 코드의 변경 내용을 안드로이드 스튜디오를 통해 실시간으로 확인할 수 있으며, 버전 관리에도 용이하다.

# Step 1: Git 버전 확인 

## 1 - 1. Git 버전 확인
![1-1]({{ "/assets/images/20241110/1-1.png" | relative_url}})
{% capture notice_1-1 %}
* 1) 안드로이드 스튜디오
* 2) File
* 3) Settings
{% endcapture %}
<div class="notice--info">
  {{ notice_1-1 | markdownify }}
</div>

## 1 - 2.  File  → Settings
![1-2]({{ "/assets/images/20241110/1-2.png" | relative_url}})
{% capture notice_1-2 %}
* 1) Version Control 클릭
* 2) Git 클릭
* 3) test버튼 클릭
* → 현재의 깃 버전과 실행 테스트를 진행할 수 있음
{% endcapture %}
<div class="notice--info">
  {{ notice_1-2 | markdownify }}
</div>


## 1 -  3  버전 확인 완료
![1-2]({{ "/assets/images/20241110/1-3.png" | relative_url}})

git.exe의 경로를 입력해주면 됨.

(깃을 설치 후 프로젝트를 열면 똑똑한 안드로이드 스튜디오가 자동으로 path를 잡아줌)


# Step 2:  GitHub 계정과 연동
![2]({{ "/assets/images/20241110/2.png" | relative_url}})
{% capture notice_2 %}
* 1) Version Control
* 2) GitHub
* 3) add Account...
{% endcapture %}
<div class="notice--info">
  {{ notice_2 | markdownify }}
</div>


# Step 3: Authorize in GitHub
![3-1]({{ "/assets/images/20241110/3-1.png" | relative_url}})

Authorize in GitHub 버튼을 클릭하면 GitHub 계정을 인증해야 한다

![3-2]({{ "/assets/images/20241110/3-2.png" | relative_url}})
{% capture notice_3-2 %}
* 1) 다음 해당 사용자 이름, 암호 입력창이 뜸.
* 2) GitHub 계정을 입력한 후 로그인 버튼을 클릭
* →  로그인이 성공하면 다행이지만 나는 여기서 로그인이 되지 않았음...
{% endcapture %}
<div class="notice--info">
  {{ notice_3-2 | markdownify }}
</div>


# Step 4: 로그인 문제 발생 → "+" 버튼 클릭
![4-1]({{ "/assets/images/20241110/4-1.png" | relative_url}})
 
![4-2]({{ "/assets/images/20241110/4-2.png" | relative_url}})
{% capture notice_4 %}
* GitHub을 통해서 로그인하기
* Token으로 로그인하기
* GitHub Enterprise로 로그인하기
→ 총 세 가지 옵션이 있음.
 그중에 토큰을 선택
{% endcapture %}
<div class="notice--info">
  {{ notice_4 | markdownify }}
</div>


# Step 5: Add GitHub Account 
![5]({{ "/assets/images/20241110/5.png" | relative_url}})


# Step 6: 토큰을 발급받기 위해 Git 이동
![6]({{ "/assets/images/20241110/6.png" | relative_url}})
{% capture notice_6 %}
* GitHub → Settings
{% endcapture %}
<div class="notice--info">
  {{ notice_6 | markdownify }}
</div>