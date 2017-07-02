# 1. 깃헙에 가입
https://github.com
![K-003](http://i.imgur.com/hy4OakU.png)
메인 가입화면
![K-004](http://i.imgur.com/sjlUdNh.png)
.을 쓸수없어서 아이디를 zizone으로 만듬
![K-005](http://i.imgur.com/Kv05Vq6.png)
공개하지 않고 쓰려면 프라이빗을 해야하지만 유료니까 우선 무료버전으로 신청
![K-006](http://i.imgur.com/UgYMizb.png)
로그인 하면 나오는 첫화면, 프로젝트를 바로 시작하고 싶지만 가입 메일인증이 안된상태
![K-007](http://i.imgur.com/Nzvve42.png)
Verify email adress 링크를 눌러서 인증 완료

그리고 프라이빗(소스 비공개)을 쓰려면 학교 메일을 쓰는 방법이 있습니다.

대학생, 대졸자의 경우는 학교에서 쓰던 도메인에 ac.kr이 붙은 이메일을 가지고 계실텐데

그 이메일로 인증을 하는 것이죠.

![K-010](http://i.imgur.com/z9YGBZv.png)
깃헙의 학생 개발자팩
![K-011](http://i.imgur.com/4LIvzWL.png)
학생인 경우 가능
![K-012](http://i.imgur.com/QLoJUwx.png)
학생인지 판단을 학교 이메일을 가지고 있냐로 판단을 하는데 이메일에 ac라는 상위 도메인이 있으면 됨
![K-013](http://i.imgur.com/UMB5MQ0.png)
여기에 기입할 이메일은 우상단 아이콘의 본인 아이콘 클릭 - 세팅 - 이메일에서 추가할 수 있다.

# 2. 가입 후 프로젝트 생성

![K-015](http://i.imgur.com/ySOj47n.png)

아직 학생인증이 안되었을테니 퍼블릭 프로젝트로 해보자.

![K-016](http://i.imgur.com/kZMtuxk.png)

좌하단의 .gitignore설정에서 unity를 선택한다.
gitignore는 버전관리를 하는 경우, 실행파일, 오브젝트등 버전관리를 따로 하고싶지 않은
파일확장자 혹은 파일 경로 혹은 폴더등을 지정하여,
얘네는 버전관리를 하지 않을 생각이니 무시해! 라고 지정하는 파일 설정파일이다.

![K-018](http://i.imgur.com/ramXMs2.png)

리드미 파일을 추가한다. 리드미 파일은 프로젝트에 대한 대략적인 설명을 쓰는 파일이고
마크다운 문법으로 되어있다.

프로젝트 말고 특정폴더의 설명을 하는 경우도 그곳에 readme파일을 놓는 방식으로
많이 사용한다.

![K-019](http://i.imgur.com/rmBfDv4.png)

초기화된 github 프로젝트의 모습

# 3. 기존 프로젝트를 github에 등록하기 혹은 git으로 버전관리되는 프로젝트로 변경하기

![K-020](http://i.imgur.com/Rv4qptj.png)

우선은 초록색 버튼을 눌러 주소를 복사한다. 우측의 복사 버튼을 눌러도 클립보드에 저장된다.

![K-022](http://i.imgur.com/2jwGmZC.png)

그리고 git이라는 프로그램을 설치해야한다. 사실 깃헙(github)은 git(깃)으로 세팅된 프로젝트를
공유하기 편하게 해주는 서비스라서, 이번에 배워야 할 내용은 git사용법과 github사용법이다.

github이 없어도 git을 사용할 수 있지만 ( 버전관리를 할 수는 있다. ), 공공의 서버에 올려서 랜섬웨어나, 유니티 업그레이드 후의 프로젝트 폭발, 하드디스크의 문제등을 해결하기 위한 것이 목적이라면

깃헙이나 bitbucket등의 git저장소 서비스를 사용하는 것이 좋다.

![K-023](http://i.imgur.com/bkLAK6V.png)

![K-024](http://i.imgur.com/gbAVDmW.png)

![K-025](http://i.imgur.com/cZwa3mY.png)

각자 환경에 맞는 git을 설치한 뒤 unityGame이라는 폴더를 만든다. ( 당신의 게임 프로젝트 명 )

Git Bash는 윈도우 사용자를 위한 것으로 terminal을 사용할 수 있는 맥 사용자나 우분투 사용자는

gitBash는 신경쓰지 않아도 된다. 대신 당신의 termial을 켜라

![K-026](http://i.imgur.com/9RoXSXJ.png)

이 unityGame폴더에 들어가서 마우스 우클릭을 하면 위와 같이 나오는데 Git Bash Here를 눌러서 가상터미널( 검은 CUI창을 켠다.)

리눅스와 맥 사용자는 터미널을 이용해서 해당 위치로 이동한다

  cd <해당디렉토리>

와 같이 사용하면 된다.

![K-028](http://i.imgur.com/dlu6JNk.png)

그리고 git clone 커맨드랑 아까 복사한 주소를 이용해서 . (현재디렉토리)에 내려받는다

![K-029](http://i.imgur.com/k14gyrH.png)
다 받아진 unityGame폴더의 모습 아까 생성한 .gitignore파일과 readme.md파일이 보인다.
그리고 숨김파일로 된 .git폴더는 이 버전관리 될 프로젝트의 이력등 기타 내부적으로 쓰이는 프로젝트 정보를 가지고 있으므로, 삭제하면 안된다.

![K-030](http://i.imgur.com/MJVXa91.png)
이번에 예제로 사용할 유니티 프로젝트를 하나 만들면서, 유니티 관련 세팅도 알아보자

![K-031](http://i.imgur.com/EyEkUeG.png)
생성 직후

![K-033](http://i.imgur.com/dBYIrrb.png)
세팅의 에디터로 들어가서

![K-032](http://i.imgur.com/2xLFimK.png)
visible Meta files

![K-035](http://i.imgur.com/Lfjk5kf.png)
그리고 에셋의 메타데이터 (씬 등에서 언제 변경했는지 혹은 누구 자식으로 들어가있는지와 같은 설명데이터)
를 텍스트로 저장하도록 한다. 이걸 해야 씬, 프리팹 등의 파일을 버전관리 할 수 있다.

![K-036](http://i.imgur.com/006l7L8.png)
테스트해볼 씬을 추가

![K-037](http://i.imgur.com/PwiXc6r.png)
그리고 프로젝트를 저장하면 아래와 같이 폴더 3개가 생긴다.

이렇게 안생긴 경우 폴더 내용 전체를 선택합니다.

![K-038](http://i.imgur.com/Lu7Nare.png)
그리고 우클릭으로 드래그 앤 드롭 해서, 아까의 새 git프로젝트 clone받은데에다 덮어 씌웁니다.

![K-039](http://i.imgur.com/JtrDMw8.png)
합쳐진 폴더의 모습

![K-043](http://i.imgur.com/IloUj4u.png)
그리고 그 해당 폴더로 이동해서

git status라는 커맨드를 치면 현재 버전관리하도록 설정되지 않은 폴더가 보입니다.
Assets, ProjectSettings 폴더 두개인데

Library는 유니티가 임시로 만드는 파일이므로 따로 버전관리를 하지 않아도 되서 표시가 안되는 것입니다.
이걸 표시하지 말라는 내용을 .gitignore파일을 텍스트에디터 ( 메모장, 에디트플러스, 나노, gedit, atom)등으로 열어보면 알 수 있습니다.

두 폴더를 추가해 봅시다.

git add <추가할 폴더 혹은 파일>
띄어쓰기로 중복 추가 가능, 파일명에 띄어쓰기 있는 경우는 큰따옴표로 감싸야 됨

![K-044](http://i.imgur.com/pwsh5MF.png)
폴더만 추가해도 하위의 파일까지 추가 된다는 것을 알 수 있습니다.

![K-046](http://i.imgur.com/62ZrOaP.png)
git에서는 하루분 작업량이나 일정구간 작업량을 저장하는 것을 commit이라고 하는데 이 커밋할때 쓰는 메세지를 커밋로그라고 부릅니다. 커밋로그에 그날의 작업에 대한 설명을 적어서 나중에 역사처럼 볼 수 있습니다.

![K-047](http://i.imgur.com/PHX0J5h.png)

이 로그를 잘 써놔야 나중에 이전 버전을 찾아보거나, 공동작업자의 작업이 어떤 것이 이루어졌는지 파악이 쉽습니다.

* 아이템 / 무기류 스테이터스 추가

혹은

* 피격시 깜빡이는 이펙트 추가

와 같이 추가된 로그는 보기 편하지만,

* 아이템 추가 및 저장 기능 처리 중 버그 확인, 이펙트 3종 추가, 유니티 버전 업그레이드 후 발생한 에러 처리

와 같이 섞여있으면 좀 보기 힘들겠죠. 하지만 가장 안좋은 것은 커밋로그가 없거나, 기능이나 내용이 변경되었는데 커밋로그를 쓰지 않은 경우겠죠.

# github 저장소에 push하기 ( 서버에 업로드 하기 )

![K-051](http://i.imgur.com/Seas1uJ.png)

git remote -v를 써서 현재 지정된 remote (원격) 저장소 즉 아까 github에 만든 저장소를 확인해봅시다
-v옵션은 목록을 보여주는 옵션이에요

보면 origin 이라고 지정된 주소가 두개가 있고 뒤에 fetch와 push두개가 있네요

fetch는 github서버의 저장소로부터 받아올때이고
push는 자기가 작업한 내용을 서버에 업로드 하는 것입니다.

origin은 그 저장소 url의 별칭이라고 보시면 됩니다.

git push origin 이라고 하면 origin에다 push해라! ( 업로드해라 )
git fetch origin 이라고 하면 origin에서 fetch해라! ( 받아와라 )

라는 뜻이죠.

git push를 써봅시다. 어라 제경우는 에러가 났네요

![K-053](http://i.imgur.com/EkCid8K.png)
우상단의 세팅을 눌러서 이 컴퓨터가 본인의 PC라는 것을 등록해두어야 합니다.

![K-055](http://i.imgur.com/X9h6NI9.png)
SSH and GPG keys를 누르고

![K-056](http://i.imgur.com/xlNOweA.png)
new ssh key버튼을 누르면

![K-058](http://i.imgur.com/za5q4J5.png)
타이틀이야 아무거나 하셔도 됩니다. 저는 구분할 용도로
99만원 주고 산 노트북이라고 쓰려구요

그럼 내용을 뭘 적어야 할까요?

![K-065](http://i.imgur.com/mq50QiE.png)
터미널로 다시 돌아와서 위와 같이 칩니다.
~라는 폴더는 유저의 윈도우던 맥이던 우분투던 로그인한 아이디의 기본디렉토리에요.
.ssh는 ssh용 설정파일이 들어있는 거죠. ssh는 서버에 접속할때 보안처리를 해주는 프로그램이라고 보시면 되요.

ssh-keygen이라는 커맨드로 위와같이 암호화용 키를 만듭니다.
보통은 id_rsa라는 걸로 만들면 되는데 저는 예전에 쓰던 아이디에 쓰는 id_rsa파일이 이미 있어서
id_rsa_zizone이라고 만들었습니다.

이렇게 하면 파일이 2개가 생기는데

id_rsa_zizone하고 id_rsa_zizone.pub
두개에요.

.pub가 없는 파일은 프라이빗키라고 하고, .pub가 있는 파일은 퍼블릭 키라고해서
둘중에 퍼블릭키는 남한테 알려줘도 되는 키에요.

텍스트파일을 그냥 화면에 출력하는 cat명령어를 이용해서 확인해 봅시다

![K-069](http://i.imgur.com/5oNop2d.png)

ssh-rsa부터 내용을 드래그 해서 복사합니다 ( 내용일부는 보안을 위해 지웠습니다.)

![K-070](http://i.imgur.com/dGEjn5k.png)
아까 내용물에 이걸 붙여넣고 확인을 눌러요 ( 내용일부는 보안을 위해 지웠습니다.)

add ssh key 버튼요

![K-072](http://i.imgur.com/KB1DJ2z.png)
키가 등록된 것을 확인 할 수 있네요.

그리고 원래 커맨드 창으로 돌아가서

git push를 누르면 됩니다.

서버에 올라간 것을 확인 가능합니다.

이 파일도 추가해서 한번 올려보겠습니다.
