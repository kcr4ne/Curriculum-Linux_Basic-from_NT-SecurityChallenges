# Linux 업데이트 및 업그레이드<br><br><hr>
저번 시간에 ubuntu를 설치했죠?
이번에는 Linux를 업데이트하고 업그레이드 해봅시다.

아래 명령어는 Linux를 업데이트하는 명령어 입니다.
<code style="background-image: linear-gradient(135deg, #000000, #ffd057); color: #e9e8ff;">sudo apt update</code><br>
업데이트를 했으니 이번에는 업그레이드도 해볼까요?
업그레이드는 업데이트와 다르게 명령어 입력 후 [Y/n]으로 업그레이드 의사를 물어봅니다.
Y를 입력하면 업그레이드가 진행되고 N을 입력하면 업그레이드가 최소됩니다. (대소문자 상관 없음)
<code style="background-image: linear-gradient(135deg, #000000, #ffd057); color: #e9e8ff;">sudo apt upgrade</code><br>
가끔씩 Linux에서 무언가를 설치할 때 오류가 생겨서 설치하지 못 하는 경우가 발생하는 데
이때, update나 upgrade 명령어를 입력해주면 설치 오류가 해결될 수 있습니다. (<del>어째서..?</del>)<br>
이 명령어에서 사용한 sudo라는 명령어는 Windows에서의 관리자 권한으로 실행과 같은 의미로 Linux에서는 관리자를 root라고 지칭합니다.
<br><br>

# Vi 편집기 사용<br><br><hr>
Linux에서 txt파일이나 python, c언어로 프로그램을 만들어보고 싶지 않으신가요? <del>아니면 말고요..</del> <br>
그런 당신을 위한 훌륭한 편집기가 있습니다.<br>
바로 <b>vi 편집기</b>죠.<br>
사용 방법은 다음과 같습니다.<br>
vi 파일이름.확장자<br>
&nbsp&nbsp&nbsp ex) <code style="background-image: linear-gradient(135deg, #37ff00, #ffb3fb); color: #000000;">vi NiceTop.txt</code><br>
&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp<code style="background-image: linear-gradient(135deg, #37ff00, #ffb3fb); color: #000000;">vi nicetop.c</code><br>
&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp<code style="background-image: linear-gradient(135deg, #37ff00, #ffb3fb); color: #000000;">vi N1c3T0p.py</code>
<br><br>
직접 해볼까요?<br><br>
vi 명령어로 파일을 하나 만들어봅시다.<br>
<img src="https://i.ibb.co/TBsMPBVs/image.png" alt=""/><br>
아래의 이미지처럼 나오면 ==i키==를 눌러서 insert 모드로 변경할 수 있습니다
<img src="https://i.ibb.co/2pQ62qC/image.png" alt=""/><br>
이제 키보드로 내용을 입력할 수 있습니다.
<img src="https://i.ibb.co/WNv7VT3T/image.png" alt=""/><br>
내용을 입력하셨다면 키보드의 <span style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">ESC</span>키를 누르고
<span style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">:wq</span>를 입력하시면 됩니다.<br>
여기서 <span style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">:w</span>는 저장하겠다는 명령어이고 <span style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">:q</span>는 나가겠다는 명령어 입니다.<br>
파일에 변경사항이 있다면 저장하고 나가거나 <span style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">:q!</span>로 저장하지 않고 강제로 나가는 방법이 있습니다.
<img src="https://i.ibb.co/r2Fmx7BC/image.png" alt=""/><br>
이제 저장이 잘 되었는 지 확인해볼까요??
<br><br>

# cat 명령어 사용<br><br><hr>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">cat 파일이름</code>으로 파일의 내용을 확인할 수 있습니다.<br>
<img src="https://i.ibb.co/0VJ73kjH/image.png" alt=""/><br>
잘 나오시나요?<br>
CTF나 워게임에서 쉘을 따내면 cat 명령어를 사용해서 문제의 정답인 flag 값을 확인할 수 있으니 필수로 알아야 하는 명령어 중 하나 입니다.
<br><br>

# 디렉토리(폴더) & 파일 만들고 지우기 / pwd 명령어 사용<br><br><hr>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">mkdir 디렉토리 이름</code>로 Windows의 폴더와 같은 디렉토리를 만들 수 있습니다.<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">ls</code>로 현재 디렉토리 위치의 파일 목록을 확인할 수도 있죠.<br>
<img src="https://i.ibb.co/mVwvN0YQ/image.png" alt=""/><br>
반대로 지우는 명령어는 <code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">rmdir 디렉토리 이름</code>이며 이때는 디렉토리 내부가 비어 있어야만 삭제할 수 있습니다.<br>
<img src="https://i.ibb.co/1YTZ8g7b/image.png" alt=""/><br>
혹시 지금 당신이 어느 디렉토리에 위치해 있는 건지 궁금하지 않으신가요?
ubuntu에 <code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">pwd</code>라고 입력해보세요!<br>
"/home/아이디"로 나오지 않나요?<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">pwd</code> 명령어는 Print Working Directory라는 뜻으로 현재 작업 중인 디렉토리 경로를 출력해주는 명령어입니다.<br>
<img src="https://i.ibb.co/8nD35Rkw/image.png" alt=""/><br>
이제 우리는 디렉토리를 만들고 지울 수 있고 현재 작업 중인 디렉토리 위치도 알 수 있습니다.<br>
그럼 이번엔 디렉토리를 들어갔다가 나가는 명령어도 써볼까요?
<br><br>

# Change Directory(cd)<br><br><hr>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">cd 디렉토리</code>로 디렉토리 내부로 들어갈 수 있고
<img src="https://i.ibb.co/DHnDMMP8/image.png" alt=""/><br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">cd ..</code>으로 나올 수 있습니다.
<img src="https://i.ibb.co/d0nLgfFP/image.png" alt=""/>
<br><br>

# 자주 쓰는 Linux 기본 명령어 모음<br><br><hr>
> Linux에는 명령어가 많기 때문에 개인적으로 자주 사용하는 명령어를 소개하고 커리큘럼을 마치겠습니다.
<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">sudo su</code> - root로 권한 변경 (비밀번호 설정 시 비밀번호 입력 필요)<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">sudo 명령어</code> - 관리자 권한으로 명령어 실행<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">apt install, update, upgrade</code> - 각각 설치, 업데이트, 업그레이드<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">cd 디렉토리 or 디렉토리 경로</code> - 현재 위치한 디렉토리 변경 (cd .. 으로 현재 디렉토리에서 상위 디렉토리로 이동)<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">cat 파일명</code> - 파일 내용 보기<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">ssh 접속할 주소</code> - 접속할 주소에 SSH 접속<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">ls</code> - 파일, 디렉토리 리스트를 볼 수 있는 명령어 (ls -al로 숨겨진 파일, 디렉토리 확인 가능)<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">pip install (python3-pip 설치 후 사용 가능)</code> - Python 패키지 설치 명령어 (시스템 해킹 커리큘럼에서 Pwntools 설치 시 나옴)<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">touch 파일명</code> - 파일 생성<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">rm 파일명</code> - 해당 파일 삭제, 디렉토리는 rmdir로 삭제 가능하지만 디렉토리가 비어있어야 삭제 가능(rm -rf로 비어있지 않아도 삭제 가능)<br>
<code style="background-image: linear-gradient(135deg, #898989, #5d00ff); color: #ffffff;">chmod 옵션 파일명</code> - 파일에 권한 부여 (Read(4), Write(2), Execute(1)), (파일 소유자, 그룹, 그 외) ex) chmod 741 nicetop.txt<br>

# 마무리<br><br><hr>
이 커리큘럼에서 설명한 명령어 외에도 정말 다양한 명령어가 많기 때문에 Linux는 직접 사용하면서 익숙해져야 합니다.<br>
이상으로 Linux 기초 커리큘럼을 마치겠습니다.<br>
감사합니다.
