---
layout: post
title:  "GitHub Pages - jekyll remote theme"
date:   2020-04-05
categories: github
tags: github jekyll
---


GitHub Pages + jekyll + remote theme 로 static web page 만드는 방법.
> 특징
> - 프로그램 설치 불필요.
> - css 등 커스터마이징 불가능? 

# 1. Create a new repository
>   `{username}`.github.io

# 2. jekyll theme
>   https://github.com/topics/jekyll-theme
>
>   -> https://github.com/mmistakes/minimal-mistakes/ 선택

# 3. _config.yml
>   https://github.com/mmistakes/minimal-mistakes/blob/master/_config.yml
>   `copy`
>
>   ```https://github.com/{username}/{username}.github.io```
>   -> Create new file
>
>   `{username}`.github.io/`_config.yml`
```yaml
......
remote_theme        : "mmistakes/minimal-mistakes"
......
url                 : "https://{username}.github.io" 
baseurl             : "" 
......
```

# 4. index.html
>   `{username}`.github.io/`index.html`
>
```markdown
---
layout: home
author_profile: true
---
```

# 5. https://`{username}`.github.io/   접속해보기

# 6. post 작성하기
> `_posts` 아래의 md 파일들을 인식하여 보여준다. 파일 이름 형식 `YYYY-MM-DD-name-of-post.md`


