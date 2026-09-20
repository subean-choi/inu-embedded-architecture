# 임베디드 구조

- 임베디드 구조 중간고사
- 임베디드 구조 기말고사

---

# 임베디드 구조 중간고사

# Lecture Note 1
### 하드웨어 구성 요소
- 중앙처리장치 (CPU)
- 기억장치 - 주기억장치, 보조기억장치
- 입출력장치 
### 마이크로 컴퓨터의 기본 구성 요소 3가지
- CPU부 - CPU와 칩셋
- 메모리부 - 읽기전용 ROM (프로그램 메모리) , 읽고 쓰기 RAM (데이터 메모리)
- 입출력장치 접속부
### 버스의 정의 및 필요성
- 정의 : 정보를 교환하기 위해 CPU와 하드웨어 요소들을 연결해주는 신호선들의 집합
- 필요성 : 자주 사용하는 신호선의 배선 수를 줄임
### 칩셋의 구성
- 노스브리지(north bridge) - 메모리 컨트롤러, 주로 고속 장치
- 사우스브리지(south bridge) - i/o컨트롤러 , 주로 저속 장치
+) 프로세서, 펌웨어 칩
### 마더보드 또는 메인보드
- 컴퓨터 시스템의 주기판
# Lecture Note 3
### 시스템 소프트웨어 정의 및 역할
- 정의 : 하드웨어 구동과 관련되어 컴퓨터 시스템을 효율적으로 다루기 위한 프로그램들의 집합
- 역할 
<table>

<tr>
<td>사용자 ↔ 시스템</td>
<td>로더</td>
<td>HW 명령 ↔ 시스템</td>
<td>언어처리기</td>
<td>응용 프로그램</td>
<td>운영체제</td>
</tr>
<tr>
<td></td>
<td>진단</td>
<td></td>
<td>라이브러리</td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td>유틸리티</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</table>

### 커널의 정의 및 역할
- 정의 : 운영체제의 핵심부로 항상 주기억장치에 상주
- 역할 : 하드웨어와 소프트웨어 요소들 사이의 통신과 시스템 자원 관리
### 시스템 호출 정의 및 역할
- 커널에 운영체제의 서비스를 요청하는 절차
- 역할 : 응용프로그램은 프로그래밍 언어에서 지원하지 않는 기능을 운영체제의 루틴에서 호출해 사용
### OLE 의미
= Object Linking and Embedding (= 개체 연결 및 포함)
= 외부 문서 참조기능을 위한 윈도우 OS 표준
# Lecture Note 4
### 어셈블리어 언어 정의
- 사람이 이해할 수 있는 고급언어와 기계어 사이에 존재하는 기계마다 다른 CPU 고유의 중간언어
- 기계어와 정확히 1:1 대응
### 연산코드 필드 및 오퍼랜드 필드 의미
= 고급언어 → 기계어로 번역되는 과정
1) 연산코드 필드 = 명령, 동작을 지정
2) 오퍼랜드 필드 = 연산의 대상을 찾는 법
### 컴파일러, 인터프리터 비교
= 번역 프로그램의 종류
1) 인터프리터 - 소스코드를 한 줄씩 읽어 번역하고 실행하는 방식
= 오류 찾기 Good, 메모리 공간 적게 사용, 속도 느림
2) 컴파일러 - 소스 코드를 한 번에 모두 읽어 번역해 놓고 실행
= 메모리 공간 많이 사용, 속도 빠름
### 서브루틴 의미
= 메인 프로그램의 독립적인 일부분으로 필요할 때 호출되어 “재사용”할 수 있는 프로그램
# Lecture Note 5
## 특정 하드웨어 흉내 
### 시뮬레이션 의미 
= 실제 하드웨어 구동 없이 실행되는 소프트웨어적인 모의 실험 방법
### 에뮬레이션 의미
= 다른 하드웨어를 대신 구동해 특정 하드웨어를 모방
### 다중작업 정의
= 멀티태스크 혹은 멀티 태스킹 = 동시에 처리해야 할 여러개의 작업
## 우선순위 할당 방식
### 전면 작업 정의
= 다중작업 가능한 컴퓨터의 활성 창에서 수행되는 작업
= 후면 작업에 대해 실행 우선순위 높음
### 후면 작업 정의
= 우선순위가 낮은 프로그램은 우선순위가 높은 프로그램이 쉴 때만 조작되는 상태
### 새도우 램의 정의
= ROM의 실행속도를 증가시키기 위해 이를 복사해 사용하는 RAM 메모리 영역
### 반도체 메모리의 동작 속도가 빠른 순서
1) 캐시 메모리 - SRAM
2) 메인 메모리 - DRAM
3) 바이오스 칩 - ROM
## 부팅할 때 메모리 비우는 방법
### 콜드 부트 의미
= 전원이 꺼져 메인메모리의 내용이 모두 삭제된 상태에서 시작하는 부팅
= 하드웨어적으로 컴퓨터를 완전하게 초기화
### 웜 부트 의미
= 메모리의 남은 내용은 엔진의 열기와 비례하다
= 컴퓨터의 전원이 켜져 있어 주기억장치에 내용이 아직 남아있는 상태에서 시작하는 부팅
### POST의 의미 및 역할
= Power On Self Test
= 롬 바이오스의 일부로 컴퓨터를 켜거나 리셋 될 때 수행되는 내부 테스트 프로그램
- 역할 : 메인보드에 대해 자체적인 하드웨어 테스트 실시
### UEFI 펌웨어의 역할
1) 부트 서비스
- 운영체제를 로드하는 부팅 실시
- UEFI 펌웨어가 플랫폼을 소유하는 동안에만 가능
2) 실시간 서비스
- OS동작 중에도 시스템 설정과 한정된 그래픽 제어
### 신호의 액티블 레벨 의미
- 디지털 회로의 신호가 High나 Low의 어느 한 레벨 중에서 “의미 있는 동작”을 하도록 신호의 활성상태를 설계하는 것.
### 트리거, 레벨 트리거, 에지 트리거 의미
1) 트리거 - 어떤 하드웨어 장치를 동기에 맞추어 동작시킬 수 있도록 제공되는 신호
ㄱ. 레벨 트리거 - 신호선에 연결된 장치들이 입력신호의 “하이”나 “로우”레벨에 동기되어 동작
ㄴ. 에지 트리거 - 신호선에 연결된 장치들이 입력신호의 “라이징”에지나 폴링 에지에 동기되어 동작
# Lecture Note 6
## CPU의 구성 요소
### 연산장치, 레지스터, 제어장치 의미 및 역할
1) 연산장치 (ALU)
- 산술 및 논리연산장치
2) 레지스터
- 연산을 위해 다양한 용도로 사용되는 CPU 내부의 일시적인 기억장소
3) 제어장치
- 명령을 해석하고 실행하기 위한 “제어 신호 발생”
### 몇비트 컴퓨터인가를 판정하는 2가지 방법
1) 데이터 버스의 비트 수
= CPU 내부와 외부 사이에 한 번에 주고받을 수 있는 데이터 버스의 비트 수
2) 범용 레지스터의 비트 수
= CPU 내부 범용 레지스터가 “정수 연산”에서 한 번에 처리할 수 있는 비트 수
### 보조 프로세서 의미 및 역할
- 메인 프로세서에 없거나 부족한 기능을 도와 컴퓨터 시스템의 성능을 높여주는 특수목적용 프로세서
### 부동소수점 처리 장치 정의
= 수치연산 보조프로세서
## 레지스터의 구성
### 어큐뮬레이터  (== 누산기)
- 연산에 가장 빈번하게 사용, 데이터를 일시 저장
- 연산 결과가 다시 자신에게 “누적”
### 프로그램 카운터 (PC)
- 다음에 인출해 올 “명령어의 주소”를 저장
### 메모리 주소 레지스터
- 주소버스로 주소를 출력하기 전에 임시로 저장 (= 주소 임시 저장)
### 메모리 버퍼 레지스터
- 데이터 버스로 데이터를 읽고 쓸 때 임시로 저장 (= 데이터 임시 저장)
-
### CPU 범용 레지스터 용도 3가지
1) 어큐뮬레이터 - 데이터를 주로 저장
2) 포인터 - 데이터의 “주소”를 저장
3) 카운터 - 데이터의 “개수”를 저장
# Lecture Note 7
### 마이크로 연산 의미
= CPU에서 “한 클럭 펄스” 동안에 일어나는 세부 동작
### 레지스터 전송 언어(RTL) 정의
= 레지스터의 동작을 기호로 나타낸 언어
= 어셈블리 언어의 중립적인 형태
### 누산기를 사용하는 이유 (어큐뮬레이터)
- 한정된 범용 레지스터의 사용 개수를 줄임
### CPU 명령어 세트를 설계할 때 고려 사항들
1) 명령어 형식 - 연산 코드와 오퍼랜드 필드의 비트 수
2) 주소지정 방식 - 실제 피연산자를 찾아내는 방법
3) 연산의 종류 - “목적에 따라” 실행할 연산의 종류
4) 데이터 타입 - 정수, 부동소수점 표현 방식과 비트 수
⇒ 명주연데 (명주가 연대에서 데이트할 때 고려사항)
### 일반적인 명령어 형식
1) 연산코드(연산자) - 연산의 동작을 지정
2) 오퍼랜드(피연산자) -연산에 필요한 대상이나 위치를 표시
# Lecture Note 8
### 어드레싱 모드 ( = 주소지정 방식)
= 명령어 형식에 포함된 오퍼랜드 필드에서 “실제 피연산자”를 찾아내는 방법
### 유효주소
- 실제 오퍼랜드의 주소, 즉 실제 피연산자가 저장된 메모리 위치
### 간접주소
- 유효주소가 저장된 메모리 (유효주소의 주소)
## 주소지정 방식의 종류
\<어셈블리 명령어; 레지스터 전송 언어\> 로 표시
### 1) 암시적 주소지정 방식
= 오퍼랜드 없이 연산코드 자신만으로 특정 레지스터의 동작을 암시 
ex) INC;  AC ← AC +1
### 2) 즉시 주소지정 방식
= 명령어 형식의 오퍼랜드 필드에 \<즉시 사용할 수 있는 데이터 수치\>로 실제 피연산자가 들어 있읨
ex) ADD B, 90H; B ← B+90H
### 3) 직접 주소지정 방식
= 오퍼랜드 필드에 실제 피연산자가 저장된 메모리 위치인 “유효주소”가 들어있음
ex)  ADD B, [1234H]; B ← B+M[1234H]
### 4) 간접 주소지정 방식
= 오퍼랜드 필드에 유효주소가 저장된 메모리 위치인 “간접주소”가 들어있음
ex) ADD B, [[5678H]] ;  B ← B + M[M[5678H]]
### 5) 레지스터 간접주소 방식
= 오퍼랜드 필드에서 지정한 레지스터에 유효주소 장
ex) ADD B, [C] ; B ← B+M[C]
### 6) 상대 주소지정 방식 
= 오퍼랜드 필드에서 지정한 프로그램 카운터 PC에 저장된 주소 값과 변위 값 d를 더해 유효주소 계산
ex) ADD B, [PC+d] ; B ← B + M[PC+d]
### 7) 인덱스 주소지정 방식
= 상대 주소지정 방식의 일종, PC 대신 인덱스 레지스터 IX를 별도로 사용하면 배열 연산에 유리
ex) ADD B, [IX+d] ; B ← B +M[IX+d]
## 정수의 산술연산
### 1의 보수 표현 (-127\~+127)
= 음수는 양수에서 모든 비트의 1과 0을 반전 (단, 부호 비트는 바꾸면 노노)
### 2의 보수 표현(-128\~+127)
= 음수는 1의 보수 표현에 1을 더해 표시
## 정수의 표현
### n비트로 표현 가능한 10진수의 범위
- 1의 보수 표현 → -(2\^(n-1)-1) \~ (2\^(n-1)-1)
- 2의 보수 표현 → -(2\^(n-1)) \~ (2\^(n-1)-1)
# Lecture Note 9
### 고정 소수점 방식
= 소수점 위치가 고정되고 정수부와 소수부로 표시
### 부동 소수점 방식
= 소수점의 위치를 편리하게 이동시켜 그 위치를 “지수”로 나타냄
<table>

<tr>
<td>고정소수점 방식</td>
<td>부동 소수점 방식</td>
<td>프로그래밍 방법</td>
</tr>
<tr>
<td>1230000000000</td>
<td>1.23 x 10\^12</td>
<td>1.23e12</td>
</tr>
<tr>
<td>0.0000000000123</td>
<td>1.23 x 10\^(-12)</td>
<td>1.23e-12</td>
</tr>
</table>

### 2진 부동소수점 표현방식에서 지수 바이어스를 사용하는 이유
= 부호를 갖는 지수를 2의 보수로 표현하면 두 수의 크기를 비교하기 어렵기 떄문
### 정규화 형식 의미
= 소수점 앞에 정수부로 항상 1이 오도록 정규화
### IEEE 754 표준 부동 소수점 수식 표현
```math
F2 = (-1)^s*1.m*2^e
```
k비트 지수부에 저장되는 값은
```math
e+(2^(k-1) -1)
```
예시) -1.1101x2\^4를 IEEE 745 표준의 32비트 2진 부동소수점 형식으로 저장하고, 이를 16진수로 표현
1) 음수이므로 부호 비트에 1
2) 지수부는 4+127 =131  → 2진수로 1000 0011
3) 가수부는 소수점 오른쪽의 1101이 맨 앞에 옴
4) 16진수로 표현하면 → 0xC1E80000
? → 2진수로 1(부호) 100 0001 1(지수부) 110 1000 0000 0000 0000 0000(가수부)
# Lecture Note 10
### 논리적 시프트 연산 의미
= 부호를 고려하지 않고 스프트 레지스터 비트들이 좌우로 1비트씩 이동
= 곱셉이나 나눗셈 등의 적용
### 순환 시프트 연산 의미
= 부호를 고려하지 않음
= 부호 비트를 포함해 시프트 레지스터의 비트들이 좌우로 회전해 다시 반대쪽 입력으로 들어감
= “직렬 데이터”의 비트 전송 등 사용
### 산술적 시프트 연산 의미
= 부호 비트는 고정 (제외) 나머지 비트들이 좌우로 이동
= 2의 보수 표현에서 산술적 우측 시프트는 부호비트가 우측으로 복사
### 제어방식
1) 하드와이어 제어 방식
= 하드웨어만으로 마이크로 연산을 수행하도록 구성
2) 마이크로 프로그램 제어 방식
= 제어 메모리에 저장된 마이크로명령어를 찾아 순차적으로 실행
### 매핑의 개념
= 다른 데이터 세트와 대응 관계를 가진 일련의 데이터 세트를 1:1로 맺어주는 과정
## 제어신호를 만드는 방법
1) 수평적 마이크로프로그램
= 마이크로 연산 필드의 비트를 “그대로 이용해” 그 비트 수만큼 1:1 대응하도록 제어 신호선을 출력하는 방법 
2) 수직적 마이크로프로그램
= 마이크로 연산 필드의 비트를 “디코더로 해독해” 제어 신호선의 개수를 늘리는 방법
# Lecture Note 12
### 명령어 기본 사이클
1) 명령어 인출 사이클 - cpu가 메모리에서 명령어를 읽어오는 단계
2) 명령어 실행 사이클 - cpu가 명령어를 수행하는 단계
## 서브루틴 호출과 복귀
### 메모리의 스택 영역 역할
= 서브루틴을 호출 할 때 메인 프로그램의 위치로 다시 돌아올 “복귀 주소 저장”
# Lecture Note 13
### 인터럽트 개념
= 프로그램의 정상 처리순서를 방해하는 서비스 요구
- cpu 외부장치나 프로그램 요청에 의해 발생
- 일반 서브루틴과 달리 대부분 “전혀 예상치 못한 시점”에서 cpu에 서비스 요구
# Lecture Note 14
### PCB (Process Control Block)
1) process state - running, waiting, etc
2) program counter - location of instruction to next execute
3) CPU registers - contents of all process centric registers
4) CPU scheduling information - priorites, scheduling queue pointers
5) Memory management information - memory allocated to the process
6) Accounting information
7) I/O status information
### Preemptive Scheduling Policies
= preemptive scheduling policy interrupts proessing of a job and transfers the CPU to another job.
### Non-Preemptive Scheduling Policies
= functions without external interrupts.
# Lecture Note 15
## 병렬계산
### 비트레벨 병령계산
- 반도체 cpu 프로세서 내부에서 컴퓨터 워드의 비트수를 늘려 한 번에 처리할 수 있는 비트 수를 늘린 것
### 명령어 레벨 병렬 계산
- 프로그램의 겨로가에 영향을 주지 않으면서 명령어의 순서를 재배열하고 그룹으로 묶어 병렬로 실행
### 데이터 병렬 계산
- 각 처리장치가 같은 작업을 하면서 데이터를 분산시킨 서로 다른 데이터 조각을 처리하는 구조
- 처리 방법은 동일하나 많은 데이터를 가질 때 유용
### 작업 병렬 계산
- 다중 프로세서를 이용한 작업
- 실행 장치가 서로 다른 병렬컴퓨터에 작업을 분배하는데 중점, 같은 작업이나 서로 다른 작업을 나누어 실행
### 명령어 파이프라인 개념
= 하나의 명령어 사이클을 여러 단계로 나누고 각 단계에서 동시에 다른 명령어를 처리하도록 cpu 설계
= 파이프라인의 깊이는 총 단계의 수
- 각 단계는 독립적인 모듈로 구성되어 서로 다른 명령어를 다른 단계에서 동시에 처리하도록 설계
# Lecture Note 16
### 4단계 파이프라인 구조
1단계 : 명령어 인출
2단계 : 명령어 해독
3단계 : 연산 실행
4단계 : 연산 결과 저장
### 슈퍼 스칼라 구조 개념
= 한 명령어 사이클 동안 여러 개의 명령어를 동시에 처리할 수 있도록 설계한 CPU 구조
### 램 상주 프로그램
= 실행 후 종료 될 때 제거되는 다른 프로그램과 달리 메모리에 전체나 일부가 남아 항상 대기
- 필요할 때 부르면 즉시 나타나 일을 수행
# Lecture Note 17
### 엔디언
= 메모리 주소와 같은 논리적으로 1차원적인 공간에 여러 개의 연속된 자료를 배열하는 방법
1) 빅엔디언 - 큰 단위 바이트가 앞 번지에 옴
2) 리틀 엔디언 - 작은 단위의 바이트가 앞 번지로 옴
[image omitted: personal or temporary Notion asset]
### 엑세스 타임 의미
= cpu가 데이터의 저장 위치에 접근을 완료하거나 응답을 받기 시작하는 데 걸린 시간
### 하드디스크 스와핑 개념
= 메인 메모리의 내용과 보조기억장치인 하드디스크의 내용을 상호교환 하는 것
= 스왑 파일을 가상메모리를 사용할 때 실제 메모리인 램에 대한 확장으로 하드디스크에 만들어지는 파일
### 페이지와 단위 개념
- 가상메모리 공간을 일정한 크기로 나누어, 메인 메모리와 하드 디스크 사이에 한 번에 이동하는 단위

---

# 임베디드 구조 기말고사

# Lecture Note 5
### 시뮬레이션( simulation) 의미
= 실제 하드웨어 구동 없이 실행되는 소프트웨어적인 모의실험 방법
### CPU 스케줄링 - 라운드 로빈 방식, 우선순위 할당 방식에 대한 이해
- 라운드 로빈 방식 
= 순서를 순환하며 기회를 균등하게 분활하는 방식
- 우선순위 할당 방식
= 각 응용프로그램들에 대해 작업 우선순위에 따라 시간 할당비율 조정
### 전면( foreground) 작업 정의
= 다중 작업 가능한 컴퓨터의 활성 창에서 수행되는 작업
### 후면(background) 작업 정의
= 우선순위가 낮은 프로그램은 우선순위가 높은 프로그램이 쉴 때만 조작되는 상태
### 롬 바이오스(ROM BIOS) 역할
- 컴퓨터 시스템의 부팅에 관계
- 운영체제를 도와 하드웨어를 저수준 제어
### 콜드(cold)부트 의미
= 전원이 꺼져 메인 메모리의 내용이 모두 삭제된 상태에서 시작하는 부팅
### 웜(warm)부트 의미
= 컴퓨터의 전원이 켜져 있어 주기억장치에 내용이 아직 남아있는 상태에서 시작하는 부팅
### UEFI(united extensible firmware interface)  펌 웨어의 역할
- 부트 서비스 = 운영체제를 로드하는 부팅을 실시
- 실시간 서비스(runtime service) = OS동작 중에도 시스템 설정과 한정된 그래픽 제어
### 신호의 액티브 레벨( active level) 의미
= 디지털 회로의 신호가 high나 low의  어느 한 레벨 중에서 의미있는 동작을 하도록 신호의 활성상태(active state, 액티브 상태)를 설계하는 것.
# Lecture Note 6
### 부동 소수점 청리장치(floating-poiint unit) 정의
= 수치연산 보조 프로세서
### 어큐물레이터( accumulator)
= 연산에 가장 빈번하게 사용, 데이터를 일시 저장 = 누산기
### 프로그램 카운터(PC)
= 다음 인출해 올 명령어의 주소를 저장
### 메모리 주소 레지스터( memory address register, MAR)
= 주소버스로 주소를 출력하기 전에 임시로 저장
### 메모리 버퍼 레지스터( memory buffer register)
= 데이터 버스로 데이터를 읽고 쓸 때 임시로 저장
# Lecture Note 7
### 누산기를 사용하는 이유
= 한정된 범용 레지스터의 사용 개수를 줄임
ex) AC← B+C 대신 AC ←AC+_B
### CPU 명령어 세트를 설계할 떄 고려 사항들
- 명령어 형식
= 연산 코드와 오퍼랜드 필드의 비트 수
- 주소 지정 방식
= 실제 피연산자를 찾아내는 방법
- 연산의 종류
= 목적에 따라 실행할 연산의 종류
- 데이터 타입
= 정수, 부동소수점 표현 방식과 비트 수
### 일반적인 명령어 형식
1. 연산 코드( operation code) → 연산자
=  연산의 동작을 지정
= 연산기호, 연산의 종류와 방법을 나타내는 동작코드
1. 오퍼랜드 (operand) → 피연산자
= 연산에 필요한 대상이나 위치를 표시
= 연산의 대상
# Lecture Note 8
### 1의 보수 표현
→ -127 \~ +127 표현
→ 음수는 양수에서 모든 비트를 1과 0을 반전
### 2의 보수 표현
→ -128 \~ +127 표현
→ 음수는 1의 보수 표현 +1 표시
### n비트로 표현가능한 10진수의 범위
- 1의 보수 표현
```math
-(2^{n-1}-1)\sim(2^{n-1}-1) 
```
- 2의 보수 표현
```math
-(2^{n-1})\sim(2^{n-1}-1) 
```
### 정규화 형식 의미
= 소수점 앞에 정수부로 항상 1이 오도록 정규화
# Lecture Note 9
### 고정 소수점 방식, 부동 소수점 방식의 표현 방식
1. 고정 소수점 방식
= 소수점 위치가 고정되고, 정수부와 소수부로 표시
1. 부동 소수점 방식
= 소수점 위치를 편리하게 이동시켜 그 위치를 지수로 나타냄
[image omitted: personal or temporary Notion asset]
### IEEE 754 표준 2진 부동 소수점의 수식 표현
```math
F_{2} = (-1)^{S(부호)}*1.m(가수)*2^{e(지수)}
```
### 32비트 2진 부동소수점 형식 예제
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
# Lecture Note 10
### 논리적 시프트 연산, 순환 시프트 연산, 산술적 시프트 연산 의미
- 논리적 시프트 연산
= 부호를 고려하지 않음
= 시프트 레지스터 비트들이 좌우로 1비트씩 이동
[image omitted: personal or temporary Notion asset]
- 순환 시프트 연산
= 부호를 고려하지 않음
= 부호 비트를 포함해 시프트 레지스터의 비트들이 좌우로 회전해 다시 반대쪽 입력으로 들어감
- 산술적 시프트 연산
= 부호 비트를 제외한 나머지 비트들이 좌우로 이동
= 2의 보수 표현에서 산술적 우측 시프트는 부호 비트가 우측으로 복사됨
### 수평적 마이크로프로그램, 수직적 마이크로 프로그램
- 수평적 마이크로 프로그램
= 마이크로 연산 필드의 비트를 그대로 이요해 그 비트 수만캄 1:1 대응하도록 제어 신호선을 출력하는 방법
- 수직적 마이크로 프로그램
= 마이크로 연산 필드의 비트를 디코더로 해독해 제어 시놓선의 개수를 늘리는 방법
[image omitted: personal or temporary Notion asset]
# Lecture Note 14
### Preemptive scheduling policy  의미
= Preemptive scheduling policy interrupts processing of a job and transfers the CPU to another job.
### Non-Preemptive scheduling policy 의미
=  Non-Preemptive scheduling policy functions without external interrupts.
# Lecture Note 15
### 비트 레벨 병렬 계산
= 반도체  CPU  프로세서 내부에서 컴퓨터 워드의 비트수를 늘려 한 번에 처리할 수 있는 비트 수를 늘린 것
### 명령어 레벨 병렬 계산
= 프로그램의 결과에 영향을 주지 않으면서 명령어의 순서를 재배열하고 그룹으로 묶어 병렬로 실행
### 데이터 병렬 계산
= 각 처리장치가 같은 작업을 하면서 데이터를 분산시킨 서로 다른 데이터 조각을 처리하는 구조
### 작업 병렬 계산
= 기능 병렬게산, 제어 병렬계산
= 실행 장치가 서로 다른 병렬 컴퓨터에 작업을 분배하는데 중점, 같은 작업이나 서로 다른 작업을 나누어 실행
### 명령어 레벨 병렬계산의 유형 및 구조
[image omitted: personal or temporary Notion asset]
# Lecture Note 16
### 4단계 파이프라인 구조
1. 명령어 인출
2. 명령어 해독
3. 연산 실행
4. 연산결과 저장
### 슈퍼스칼라 구조 개념
= 한 명령어 사이클 동안 여러 개의 명령어를 동시에 처리할 수 있도록 설계한 CPU  구조
### 슈퍼 파이프라인 차수 개념
= 파이프라인 구조의 한 단계 내에서 처리 속도를 몇배로 높이는지 나타내는 비율
### 슈퍼 스칼라, 슈퍼파이프라인 정보를 이용한 병렬 계산의 속도 상승, 속도 상승의 이론적 최대치, 병렬 계산의 효율 계산
[image omitted: personal or temporary Notion asset]
최대치 = sp\*ss\*\*N
효율 =  ( (속도상승)/(최대치))\*100 (%)
# Lecture Note 17
### 엑세스 타임 의미
=CPU가 데이터의 저장 위치에 접근을 완료하거나 응답을 받기 시작하는 데 걸린 시간
### 페이지(page), 페이지 프레임(page frame) 개념
- 페이지
= 가상 메모리 공간을 일정한 크기로 나누어, 메인메모리와 하드디스크 사이에 한 번에 이동하는 단위
- 페이지 프레임
= 가상의 기억공간을 다룰 수 있도록 할당된 메인메모리 영역, 하드디스크의 페이지들 중 하나를 복사해 할당
### 페이징(Pasing) 또는 페이지 교체 개념
= 메인 메모리와 하드 디스크 사이의 페이지 교환 동작
= OS.가 참고하려는 페이지가 메인 메모리에 없으면 하드디스크에 저장해둔 페이지를 참조해 가져옴
# Lecture Note 18
### Thrashing 개념
= 전체 시스템 성능이 저하되어 작업의 진전이 아주 느리거나 아예 없는 상태
### 캐시 메모리(Cache Memory) 정의 및 역할
= 주로 메인 메모리의 엑세스 타임을 줄이기 위해,  cpu와 메인메모리 사이에 사용하는 빠른 속도의 메모리
\<역할\> 
= 프로그램이 현재 사용 중인 내용의 근방을 저장
= 자주 엑세사 하는 데이터나 프로그램 명령을 반복해 검색하지 않고 즉시 사용할 수 있도록 준비
### L1, L2, L3 캐시 의미 및 특징
= CPU에 가까운 순서대로 n차 캐시 혹은 레벨 n 캐시라고 함
= L3, L2, L1으로 올라갈 수록 속도는 증가, 크기는 축소
### 캐시 적중, 캐시 실패 의미
- 캐시 적중
= CPU가 원하는 내용을 캐시에서 발견한 상태
- 캐시 실패
= 원하는 내용이 캐시에 없는 상태
= 메인메묄나 그 아래 계층에서 읽어옴
# Lecture Note 19
### 캐시 쓰기 정책 의미
= 캐시의 블록이 변경되었을 때 메인 메모리의 블록을 갱신하는 방법과 시기를 정하는 것
### 연속 기록(Write-through) 캐시 의미
= cpu가 캐시와 메인 메모리 두군데 데이터를 \<정상 적으로 함께 갱신\> 하는 방식
### 캐시 알고리즘 또는 교체 정책 의미
= 캐시의 내용 중 교체되어 나갈 자료를 결정하는 것
# Lecture Note 20
### The understanding of First-Fit scheme AND Best-Fit scheme
-  First-Fit scheme
= Allocate the Fisrt hole that is big enough
- Best-Fit scheme
= Allocate the SMALLEST hole that is bit enough
### EX) how to work them on Slide 19,21
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
# Lecture Note 21
### The understanding of Dynamic partition
= Available memory kept in contiguous blocks and jobs given only as much memory as they request when loaded.
- Job allocation method
= Fisrt come Fisrt out
### EX) how to work them on slide 7
[image omitted: personal or temporary Notion asset]
# Lecture Note 23
### For Page replacement, the understanding of FIFO(First in Fisrt out) page replacement algorithm
- EX) GIven refernce string, if we use FIFO, how many page faults can be seen?
[image omitted: personal or temporary Notion asset]
### For Page replacement, the understanding of LRU(Least Recently Used)  page replacement algorithm
- EX) GIven refernce string, if we use LRU, how many page faults can be seen?
[image omitted: personal or temporary Notion asset]
# Lecture Note 24
### ZBR(구획비트 기록) 방식 의미
= 디스크 외곽의 헐거운 기록 밀도에서 오는 낭비를 없애기 위해 외곽에 더 많은 섹터 배치
= 하드디스크의 트랙을 여럭 개의 구역(zone)으로 나누어 기록 밀도를 달리하는 방법
### 탐색시간, 회전지연 정의
- 탐색 시간 = 헤드가 원하는 트랙을 찾는 시간
- 회전 지연 = 디스크가 회전해 원하는 섹터에 도달한 시간
# Lecture Note 25
### 인터리빙 또는 인터리브 개념
= 저장장치의 엑세스 성능을 높이기 위해 연속된 데이터가 물리적으로 인접하지 않도록 배열하는 방법
### RAID(redundant array of inexpensive disks) 개념
= HDD의 성능 개선을 위해 여러 디스크를 배열로 연결해 하나의 논리적인 디스크처럼 구동시키는 기술
### RAID 레벨 및 설계 개념 
[image omitted: personal or temporary Notion asset]
### 스트라이핑 개념
= 여러 개의 디스크에 데이터를 똑같은 스트라이프 크기로 나누어 분산 저장
# Lecture Note 26
### 등선 속도 방식 특성
= 디스크가 회전할 때 선속도를 일정한 구동방식
\<특성\>
1. 트랙 위치에 상관없이 동일한 데이터 전송속도
2. 전송속도가 일정해 기록할 때 안정적
3. 애용량 광학디스크 설계의 유리
4. 회전수가 서서히 변해 소음과 진동 거의 없음
### 등각 속도 방식 특성
= 디스크가 회전할 때 각속도가 일정한 구동방식
\<특성\>
1. 헤드가 외곽으로 갈수록 선속도 빨라짐
2. 외곽으로 갈수록 트랙당 섹터 수 늘어나 전송속도 증가
3. 고속 회전으로 소음과 진동 심한 편
4. 전송속도가 계속 변해 기록할 때 안정적이지 못함
5. 탐색 시간이 짧아 액세스 속도에서 유리
# Lecture Note 27
### NTFS 와 비교한 FAT의 장단점
[image omitted: personal or temporary Notion asset]
# Lecture Note 28
### 로우-레벨 포맷 개념 및 특성
= 하드웨어 수준에 가까움, 대개 \<제조 공장에서\> HDD를 출고할 때 실시
\<특성\>
- 트랙과 섹터를 생성한 정보를 특정위치에 저장
- 로우 레벨 포맷 후 디스크 내용은 거의 복구 불가능
### 하이-레벨 포맷 개념 및 특성
=  일반 사용자들이 사용,  \<운영체제 설치 중\> 이나 OS 없는 디스크를 새로 포맷할 때 실시
- 볼륨 부트 섹터의 볼륨 부트 레코드와 파일시스템 영역을 새로 생성, 부팅 및 OS 가 사용가능 하도록 함
- 기존 내용이 완전히 지워지지 않음
# Lecture Note 29
### The understanding of FCFS(Fist Come Fisrt Served) Disk Scheduling Algorithm 
[image omitted: personal or temporary Notion asset]
### The understanding of SSTF(Shortest Seek Time First) Disk Scheduling Algorithm 
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
### The understanding of SCAN Disk Scheduling Algorithm 
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
### The understanding of C-SCAN Disk Scheduling Algorithm 
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
# Lecture Note 30
### 인텔 터보 부스트 기술 개념
= 멀티코어 프로세서에서 이룹 코어의 동작 크럵만 순간순간 동적으로 끌어 올려주는 기술
### 터보 부스트 클럭 계산 
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
### 오버클럭킹(overclocking)  개념
= 시스템버스의 클럭을 임의로 올려 cpu 내부의 코어 클럭을 강제로 끌어 올리는 기법
# Lecture Note 31
### 어드레스 맵 (address map) 개념
= 메모리 주소나 I/O 주소의 범위와 용도를 알기 쉽도록 지도와 같이 세밀한 그림이나 표로 정리한 자료
### 폴링 방식 개념
= CPU가 주기적으로 각 I/O 장치의 상태를 검사해 전송할 데이터가 있으면 이를 처리하는 방식
### CPU 점유율 개념 및 계산
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
[image omitted: personal or temporary Notion asset]
# Lecture Note 32
### DMA  동작 모드 - 사이클 스틸링 모드, 버스트 모드 개념
- 사이클 스틸링 모드
=  CPU 가 메모리 등의 시스템 자원을 사용하지 않는 대기 상태나 내부 동작 중일 때, 마치 CPU 버스사이클을 훔치듯 그때그때 데이터를 전송하는 방식
- 버스트 모드 
= 데이터의 전송방향을 먼저 정하고 한 번에 많은 양의 데이터를 집중적으로 내보내는 방식
### 썬더볼트( Thunderbolt) 인터페이스 의미
= 기존 모든 I/O 버스 인터페이스를 통합 대체할 목
= 다른 방식의 최종목표처럼 컴퓨터 주변 장치와 블루레이 등 모든 디지털기기의 인터페이스를 통합하는 것
### 데이지 체인( Daisy Chain) 버스 결선 방식 개념
= 한 장치에 연겨로딘 다른 장치가 또 다른 장치에 연속해서 연결되는 버스 결선 방식
# Lecture Note 33
### I/O 버스 - 충돌이 발생할 수 있는 대표적인 3개
[image omitted: personal or temporary Notion asset]
### I/O 버스에서 충돌의 방지
[image omitted: personal or temporary Notion asset]
### 버스 마스터링(bus Mastering) 개념
= 주변 장치가  cpu의 간섭을 받지 않고 독자적으로 메모리와 i/o 장치 사이에 데이터를 전송할 수 있도록 해주는 버스 설계 기술
### 버스 중재기가 버스를 중재하는 순서
[image omitted: personal or temporary Notion asset]
### 인터럽트 제어 방식 - 병렬식, 직렬식, 소프트웨어 폴링 방식 특성
- 병렬식 인터럽트 제어
= 각 i/o 장치마다 별도의 IRQ 선과 INTA( 선(인터럽트 확인신호선) 사용
[image omitted: personal or temporary Notion asset]
- 직렬식 인터럽트 제어
= 하나의 IRQ 신호선과 하나의 INTA 신호선 공동 사용
[image omitted: personal or temporary Notion asset]
- 소프트웨어 폴링 방식 인터럽트 제어
= 하나의 IRQ 신호선만 공동으로 사용
[image omitted: personal or temporary Notion asset]
# Lecture Note 34
### +) 프로세서들이 처리하는 명령어와 데이터의 스트림(흐름)의 수에 따라 분류
- 단일 명령어 스트림 - 단일 데이터 스트림 (SISD)
- 단일 명령어 스트림 - 복수 데이터 스트림( SIMD)
- 복수 명령어 스트림 - 단일 데이터 스트림(MISD)
- 복수 명령어 스트림 - 복수 데이터 스트림(MIMD)
### SISD, SIMD, MISD, MIMD 개념 및 특성
- SISD
= 한 번에 한 개씩 명령어와 데이터를 순서대로 처리하는 단일 프로세서 시스템
= 파이프라이닝, 슈퍼스칼라 구조를 이용
[image omitted: personal or temporary Notion asset]
- SIMD
= 배열 프로세서
= 여러 개의 프로세싱 유니트(PU)들로 구성되고,  PU들의 동작은 모두 하나의 제어 유니트에 의해 통제
= 모든 PU들은 하나의 명령어 스트림을 실행
= 데이터 스트림은 여러 개를 동시에 처리
[image omitted: personal or temporary Notion asset]
- MISD
= N 개의 프로세서들이 서로 다른 명령어들을 실행하지만, 처리하는 데이터 스트림은 한 개
→ 비현실적이므로 실제 구현된 경우는 없음
[image omitted: personal or temporary Notion asset]
- MIMD
= N개의 프로세서들이 서로 다른 명령어들과 데이터들을 처리
= 프로세서들간의 상호 작용 정도에 따라 두 가지를 분류
1. 밀결합 시스템 (tightly - coupled system)
2. 소결합 시스템(loosely - coupled system)
