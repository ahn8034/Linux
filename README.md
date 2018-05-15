# Linux

## Linux study
*기본명령어 정리 : http://dany-it.tistory.com/63 참고할 것*

### ls
**파일 및 디렉토리 목록 보기**

### df
**디스크 용량 확인하기**

### du
**현재 디렉토리 용량 확인하기**

### pwd
**현재 디렉토리 경로 확인하기**

### cp
**파일 및 디렉토리 복사하기**

### mkdir
**디렉토리 만들기**

### rm
**파일 및 디렉토리 삭제하기**

### mv
**파일 및 디렉토리 이동하기 & 파일명 변경하기**

### ps
**현재 실행중인 프로세스 목록 보기 기능으로 옵션이 다양하므로 중요한 옵션은 숙지해야함**

* -e, -A : 현재 시스템에서 실행 중인 모든 프로세스 정보를 출력

* -f : 프로세스 정보가 한 줄씩 출력되는데, Username PID PPID C STIME TTY TIME CMD 형식으로 출력

* -l : 프로세스 정보를 한 줄씩 출력하며 -f와 비교 하였을 때, F, S, C, ADDR, WCHAN 등의 정보를 더 출력

* -a : 최근에 많이 실행된 제어 터미널을 가진 프로세스의 정보를 출력

* -G : 이 옵션 뒤에 입력된 EGID를 가지고 있는 프로세스 정보를 출력

* -U : 이 옵션 뒤에 입력된 UID를 가지고 있는 프로세스 정보를 출력

* -u : 이 옵션 뒤에 입력된 EUID를 가지고 있는 프로세스 정보를 출력

* -t : 이 옵션 뒤에 입력된 제어 터미널을 가지고 있는 프로세스 정보를 출력

* -o : 이 옵션을 사용하여 출력 형식을 조정할 수 있고 출력 형식을 조정할 수 있는 것은 user-defined format을 사용하여 user, ruser, group, rgroup, pid, ppid, args등을 조정할 수 있음

* ps -ef : 모든 프로세스를 보여주고, 다양한 정보를 한 줄씩 출력할 수 있음(자주 사용)

### kill
**현재 실행중인 프로세스를 강제 종료하므로 명령어로 옵션이 몇개 있음**
* kill -9 <PID> : 해당 PID를 죽이며, 강제 종료시 DB 같은 것들은 이렇게 죽이면 안됨

### find
**파일 찾기**

### top
**top은 프로세스의 CPU, MEMEORY 사용량 등을 보여줌(기본으로 리눅스에 있지만 CORE별로 나오지는 않음)**
* %us  : 유저 레벨에서 사용하고 있는 CPU의 비중
* %sy : 시스템 레벨에서 사용하고 있는 CPU비중
* %id : 유휴 상태의 CPU 비중
* %wa : 시스템이 I/O 요청을 처리하지 못한 상태에서의 CPU idle 상태인 비중
* PID : 프로세스 ID (PID)
* USER : 프로세스를 실행시킨 사용자 ID
* PRI : 프로세스의 우선순위 (priority)
* NI : NICE 값. 일의 nice value값이다. 마이너스를 가지는 nice value는 우선순위가 높음.
* VIRT : 가상 메모리의 사용량(SWAP+RES)
* RES : 현재 페이지가 상주하고 있는 크기(Resident Size)
* SHR : 분할된 페이지, 프로세스에 의해 사용된 메모리를 나눈 메모리의 총합.
* S : 프로세스의 상태 [ S(sleeping), R(running), W(swapped out process), Z(zombies) ]
* %CPU : 프로세스가 사용하는 CPU의 사용율
* %MEM : 프로세스가 사용하는 메모리의 사용율
* COMMAND : 실행된 명령어

### htop
**htop은 별도 설치 프로그램으로 장점은 CPU CORE별로 표시됨**

*http://hisham.hm/htop/ 참고할 것*

### tree
**별도 설치해야 하는 프로그램으로 디렉토리 구조를 tree 형태로 보여줌**

### awk

### sed

### lsof

### vi
**에디터이며, vim이라고 vi의 개선판이 있으며 리눅스 개발자들은 별도로 설치해서 사용하는 경우가 있음**
* i, ESC - 편집모드, 편집탈출
* h,j,k,l - 방향키(편집모드 탈출시에만 동작)
* CTRL + a - 제일 마지막 글자로 이동하여 편집 모드 전환
* dd - 한줄 삭제
* a - 현재 위치에서 삽입 모드
* SHIFT + y,p - 한줄 복사
* CTRL + f - 다음 페이지 이동
* CTRL + b - 이전 페이지 이동

*http://dany-it.tistory.com/18 참고할 것*


































