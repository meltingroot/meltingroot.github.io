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
<figcaption>안드로이드 스튜디오 → File → Settings </figcaption>

## 1 - 2.  File  → Settings
![1-2]({{ "/assets/images/20241110/1-2.png" | relative_url}})
<figcaption>Version Control → Git → test</figcaption>

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

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/images/unsplash-image-9.jpg)

git.exe의 경로를 입력해주면 됨.

(깃을 설치 후 프로젝트를 열면 똑똑한 안드로이드 스튜디오가 자동으로 path를 잡아줌)


# Step 2:  GitHub 계정과 연동
![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/images/unsplash-image-9.jpg)
Version Control → GitHub → add Account...


# Step 3: Authorize in GitHub
![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/images/unsplash-image-9.jpg)
Authorize in GitHub 버튼을 클릭하면 GitHub 계정을 인증해야 한다

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/images/unsplash-image-9.jpg)
1) 다음 해당 사용자 이름, 암호 입력창이 뜸.
2) GitHub 계정을 입력한 후 로그인 버튼을 클릭
→  로그인이 성공하면 다행이지만 나는 여기서 로그인이 되지 않았음...


# Step 4: 로그인 문제 발생 → "+" 버튼 클릭
![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/images/unsplash-image-9.jpg)
![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/images/unsplash-image-9.jpg)
Login In with Token...
- GitHub을 통해서 로그인하기
- Token으로 로그인하기
- GitHub Enterprise로 로그인하기 
→ 총 세 가지 옵션이 있음.
 그중에 토큰을 선택


Add `theme: "minimal-mistakes-jekyll"` to your `_config.yml` file.

If you're migrating from an existing Minimal Mistakes site you shouldn't have to change anything else after this. If it's a new site consult then docs to [properly config]({{ "/docs/configuration/" | relative_url }}).

**Please Note:** Paths for image headers, overlays, teasers, [galleries]({{ "/docs/helpers/#gallery" | relative_url }}), and [feature rows]({{ "/docs/helpers/#feature-row" | relative_url }}) have changed and now require a full path. Instead of just `image: filename.jpg` you'll need to use the full path eg: `image: assets/images/filename.jpg`. The preferred location is now `assets/images` but can be placed elsewhere or external hosted. This all applies for image references in `_config.yml` and `author.yml` as well.
{: .notice--danger}

## Step 5: `jekyll new` Tweaks

If this is a new site be sure to add the following files to `_data/` and customize as you see fit. There is currently no way of bundling them in with the theme, so be sure to consult the docs on how to properly use both.

- [`_data/ui-text.yml`](https://github.com/mmistakes/minimal-mistakes/blob/master/_data/ui-text.yml) - UI text [documentation]({{ "/docs/ui-text/" | relative_url }})
- [`_data/navigation.yml`](https://github.com/mmistakes/minimal-mistakes/blob/master/_data/navigation.yml) - navigation [documentation]({{ "/docs/navigation/" | relative_url }})

You'll also need to: 

- Replace `<site root>/index.html` with a modified [Minimal Mistakes `index.html`](https://github.com/mmistakes/minimal-mistakes/blob/master/index.html).
- Change `layout: post` in `_posts/0000-00-00-welcome-to-jekyll.markdown` to `layout: single`.
- Remove `about.md`, or at the very least change `layout: page` to `layout: single` and remove references to `icon-github.html` (or [copy to your `_includes`](https://github.com/jekyll/minima/tree/master/_includes) if using).

---

That's it! If all goes well running `bundle exec jekyll serve` should spin-up your site. If you encounter any bumps please file an issue on GitHub and make sure to indicate you're testing the pre-release Ruby gem version.

[File an issue](https://github.com/mmistakes/minimal-mistakes/issues/new){: .btn .btn--info .btn--large}

Thanks!
