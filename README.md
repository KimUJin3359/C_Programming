# C_Programming

### 프로그래밍 지식
- 프로그램 : 컴퓨터 프로그램이란, 컴퓨터에 의해 실행되는 순차적인 일련의 명령어 집합
- 프로그래밍 언어 : 프로그램을 작성하기 위해 만들어진 언어
- 프로그래밍 언어 종류
  - 저급 언어(Low Level Language) : 기계어(Machine Language), 어셈블리어(Assembly Language)
  - 고급 언어(High Level Language) : PASCAL, FORTAN, C
  - 저급 언어와 고급 언어의 기준은 특정언어가 우수하다거나 좋다는 의미가 아님
  - 하드웨어의 표현에 가까울수록 저급언어, 인간의 표현에 가까울수록 고급언어
- 기계어 : 컴퓨터가 직접 해독할 수 있는 2진 숫자 Binary Digit으로 되어있는 언어
- 인스트럭션 : machine instruction(명령어)
- 어셈블리 언어
  - 기계어 코드의 단점을 해결하기 위하여 어셈블리 언어가 등장
  - 기계어를 대신하는 단어(mnemonic)을 사용하는 방식
  ```
  어셈블리 : ADD R0, R1
  기계어 : 0000 0001 0010 1011 1000 0000 0010 0000
  ```
- 전처리(Preprocess)
  - 소스파일 내부에 있는 전처리 명령을 수행하는 과정
  - 소스파일내부에서 \#으로 시작되는 문장들은 C언어 코드가 아닌 전처리 명령어들의 집합
  - 전처리기 : 전처리 명령어를 수행
  - 전처리 명령어 : 소스파일을 컴파일 하기 전에 해당 헤더파일을 포함할 지 안할지, 컴파일을 할지 말지를 결정  
- 컴파일
  - 프로세서는 어셈블리 언어 역시 이해할 수 없음(기계어만 이해할 수 있음)
  - 고급 언어(기계어가 아닌 모든 언어)로 작성된 프로그램을 프로세서가 이해할 수 있는 기계어로 번역하는 과정
  - 각종 문법 에러를 검사(C언어의 문법에 맞지 않을 시, 컴파일에러나 경고를 발생)
  - 컴파일 에러가 없다면 기계어로 번역된 목적 코드 '\*.obj'파일을 생성
- 컴파일러 : 컴파일을 해주는 도구 
- 크로스 컴파일러 :
- 링크
  - 보통 하나의 C언어 소스 파일이 하나의 기계어 코드를 만드는 것으로 족하나, 대형 프로그램의 경우에는 다수의 소스 파일을 동시에 컴파일 해야 하는 경우가 존재
  - 컴파일 과정에서 생성된 목적 코드를 여러 개 모아서 링커를 통해 하나의 목적코드로 만드는 과정
  - 링크 과정이 끝나서 하나의 목적 코드가 생성된 이후에 실행 가능한 파일인 .exe 형태를 만들 수 있음
- 원시 프로그램 :
- 원시 언어 :
- 목적 언어 :
- 어셈블 :
- 어셈블러 :
- 임베디드 프로그래밍 언어 : C/C++, 어셈블리어 언어

### 언어의 특징
- C/C++
  - 1972년 Bell 연구소의 연구원 데니스 리치에 의해 만ㄷ르어짐
  - 운영체제를 제작하기 위해 만들어진 언어
  - 모듈성, 효율성, 이식성이 우수, 단순하고 강력한 특징이 있음
  - C언어의 한계를 극복하고자 객체지향 개념을 포함한 C++이 등장
  - 현재까지도 매우 널리 사용되는 언어  
- Java
  - 1995년 선 마이크로시스템의 제임스 고슬링에 의해 만들어짐
  - 소형 가전기기 및 모바일 등 임베디드 기기에서 사용하기 위한 목적
  - 객체지향언어, 플랫폼 독립적, 견고하고 보안에 강력, 동적인 특징을 가짐

### C언어의 특징 및 종류
#### C언어의 특징
- 장점
  - 고급 및 저급 언어간 특징을 모두 갖고 있음
  - 하드웨어에 접근이 용이
  - 단순함
  - 풍부한 연산자 제공
  - 데이터 형이 매우 다양함
  - 전처리기가 존재
  - 구조적 프로그래밍 언어
  - 제어구조가 강력
  - 실행 속도가 빠름
  - 다른 컴퓨터에 이식이 쉬움
- 단점
  - C언어의 강력한 점과 유연성은 치명적인 단점이 될 수 있음
    - 메모리 번지의 직접적인 접근으로 인한 문제 발생 가능
- 적용 분야
  - Unix
  - 컴퓨터 게임
  - 임베디드 시스템
  - 로봇 자동화
  - PC 어플리케이션 등

#### C언어의 종류
- ANSI C/ ISO C 표준
  - C언어가 널리 사용됨에 따라 다양한 라이브러리가 생겨났고, 많은 개발자들이 혼란을 겪음
  - ANSI는 1983년 X3J11이라는 C언어 표준 위원회를 설립하고 이 위원회가 제안한 표준이 1989년 정식으로 채택
  - 1990년 ISO도 C 표준을 채택하였는데, 둘다 본질적으로 동일
- C99 표준
  - 1994년 C9X 위원회, ANSI/ISO 공동위원회가 C표준의 개정작업을 시작
  - 특징
    - 국제 문자 집합을 처리
    - 미비점 보완
    - 과학과 공학 프로젝트가 요구하는 정밀한 계산이 가능하도록 실용성 개선
- C11 표준
  - 2007년 표준 위원회 C1X는 C11로 구현
  - 프로그래밍 보안 및 안전에 대한 시대적 요청
  - C99의 일부 기능이 C11에서는 선택 사항
  - 병행 프로그래밍에 대한 선택적 지원

#### C언어의 기본 구조
- 전처리기문(Preprocessor), 전역 데이터(전역 변수, 전역 함수)와 함수로 구성
- 함수 : 블록으로 구성
- 블록 : 문장으로 구성
- 문장 : 선언문, 대입문, 함수 호출문, 제어문, NULL문, 블록

### 컴파일
- 컴파일 : 인간이 이해할 수 있는 형식언어로 작성된 소스 코드를 CPU가 이해할 수 있는 기계어로 번역하는 과정
- gcc -v -save=temps 옵션 : 컴파일 과정에서 나타나는 .i, .o, .s파일들을 모두 저장
- gcc -g 옵션 : 어셈블리 및 기계어 코드를 볼 수 있음
- objdump -S 옵션 : 바이너리 파일의 정보
  - 디버깅 정보 + 인스트럭션 + 인스트럭션에 대응하는 기계어 코드
  - objdump -s : 읽기 전용 데이터 공간도 보여줌
  - 원래 소스 + 초기화 코드 + 종료 코드
- xxd '프로그램명' : 메모리에 저장된 상태 보기
- 빌드 프로세스
  - 전처리 -> 컴파일 -> 어셈블 -> 링킹

### 데이터형
- Data Type
  - 프로그램 = 데이터형 + 데이터형에 대한 연산
- 이해의 어려움
  - 수학적인 개념과 다름 : 수학에서 정수는 무한
  - suffix에 따른 수 많은 정수 표기법 : 100과 100L은 다름
- 기본 데이터형 : 정수 데이터형 + 실수 데이터형
- 데이터형이 많은 이유
  - 적재적소에 알맞은 데이터형을 쓰기 위함
    - 메모리 효율성 및 연산 속도
  - char로도 충분한 경우, long 형처럼 메모리를 많이 차지하는 데이터형을 쓸 필요 없음
  
  ![22620E385847BD1104](https://user-images.githubusercontent.com/50474972/113671686-a84f8300-96f1-11eb-86cd-9e2d1507b76e.png)

#### 2의 보수
- 컴퓨터는 음수를 2의 보수로 표기
- 보수 공식
  - 2 ^ (N + 1) = M + C
    - N : 비트 수
    - M : 보수를 구하는 숫자
    - C : 2의 보수

#### char
- 부호비트 1 bit + 7 bit
- MSB 최상위 비트를 부호비트라 함
  - 1 : 음수
  - 0 : 양수
- 하위 7bit로 수를 나타냄

#### 형 변환(Casting)
- sizeof()
  - sizeof는 함수가 아닌 연산자
  - 구조체에서는 padding을 포함하여 계산
  - 배열
    - 배열명은 포인터 값을 갖는 상수, 하지만 4Byte로 출력되지 않음
    - 칸 수 * 칸 당 Byte로 계산
  ```
  char str[32] = "hello";
  
  sizeof(str) -> 32
  strlen(str) -> 5
  ```
- 묵시적 형변환(자동 형변환)
  - 데이터 형이 좌측이 큰 경우 자동으로 캐스팅
    - int <- char 대입
  - 원칙적으로 형이 다르므로 연산시 에러를 내야함
- 명시적 형변환
  - 자동 형변환을 할 수 없어 truncation이 발생하지만 이를 감내하고 형변환 할 경우 

### 엔디언
- 컴퓨터의 메모리와 같은 1차원의 공간에 여러 개의 연속된 대상을 배열하는 방법(바이트 순서)을 뜻함
- 빅 엔디언 : 큰 단위가 앞에 나옴
  - 최상위 바이트부터 차례로 저장
  - 네트워크에서 주소를 빅 엔디언으로 씀
  - ARM CPU에서는 Big endian이 default
- 리틀 엔디언 : 작은 단위가 앞에 나옴
  - 최하위 바이트부터 차례로 저장
  - Intel CPU에서는 Little Endian 사용
  ```
  -100(int)
  빅 엔디언 : ff ff ff 9c
  리틀 엔디언 : 9c ff ff ff
  ```
- 미들 엔디언 : 두 경우에 속하지 않거나, 둘을 모두 지원하는 것

  | 빅 엔디안 | 리틀 엔디안 |
  | --- | --- |
  | Unix의 RISC 계열의 프로세서가 사용 | Intel 계열의 프로세서가 사용 |
  | 네트워크에서 사용하는 바이트 오더링 | |
  | 비교연산에서 속도가 빠름 | 계산연산에서 속도가 빠름 |
  
### 변수와 메모리
#### 메모리
- 우리가 보는 주소는 실제 물리적 주소가 아닌 경우가 많음
- 임베디드에서는 주소 = 물리적 주소
- C에서 변수는 메모리 stack, heap, bss, data에 저장
- 변수를 만들었다고 모든 변수가 메모리에 생성되지는 않음

#### MSB와 LSB
- MSB(Most Significant Bit)
  - 최상위 비트
- LSB(Latest Significant Bit)
  - 최하위 비트 

### 비트연산
- 임베디드에서 많이 사용됨(상위 어플리케이션에서는 빈도가 낮음)
- 종류
  - AND
  - OR
  - NOT
  - XOR
  - LEFT SHIFT
  - RIGHT SHIFT
- 용도
  - 특정 비트를 세트
  ```
      0000
   OR 0010
   -------
      0010
  - 세번째 비트를 1로 세팅
  ```
  - 특정 비트를 클리어
  ```
      1111
  AND 0111
  --------
      0111
  - 첫번째 비트를 0으로 초기화
  ```
  - 특정 비트를 반전
  ```
      1111
  XOR 0010
  --------
      1101
  - 세번째 비트를 1 -> 0으로 반전
  ```
  - 특정 비트값 알아내기 or 특정 비트를 추출
  ```
      1010
  AND 0010
  --------
      0010
  - 세번째 비트에 1이 들어가 있음을 알 수 있음    
  ```

### Firmware 프로그래밍
- MCU : 한 칩안에 CPU/메모리/Disk 모두 포함
  - CPU, RAM, ROM으로 구성된 하나의 컴퓨팅 시스템

#### MCU 제어 방법
- 핀에 1 신호를 주면, 전류가 흐르면서 연결된 장치가 켜짐
- PIN 8개 단위로 묶어서 관리
  - PA : P0 ~ P7를 통칭하는 말로 가정
  - PB : P8 ~ P15를 통칭하는 말로 가정
  - PC : P16 ~ P24를 통칭하는 말로 가정

#### Memory Mapped I/O
- 일반적으로 메모리 공간은 값을 임시로 저장하기 위한 공간
- 특정 메모리 공간을 입출력을 위한 공간으로 사용(memory mapped I/O)
- Hardware적으로 정해진 주소가 있음
- 포인터를 이용하여 장치 제어
  ```
  unsigned char *p = 'I/O 주소';
  *p = 0xf0;
  
#### 임베디드에서 비트연산을 사용하는 이유
- Memory Mapped I/O 구조에서 하드웨어를 제어하기 위해 포인터를 이용하여 장치를 제어
- 특정 비트만 제어해서, 다른 장치를 건드리지 않고 특정 장치만 신호를 주거나 읽을 수 있음
- 비트 연산을 통해 원하는 비트만 수정/읽기가 가능
  ```

### 함수 정의와 선언
- 함수의 정보는 Text영역에 저장됨

#### 함수 인자 전달
- Argument : 전달인자, 인자, 보내는 값
  ```
  sum(1, 2);
  ```
- Parameter : 매개변수, 함수가 호출되면 받는 값들, 입력 변수명
  ```
  int sum(int a, int b)
  {
    return (a + b);
  }
  ```
- 규칙
  - Argument의 개수와 Parameter의 개수는 같아야함
  - 보낼 때 값을 여러개 전달할 수 있음
  - 리턴 할 때는 하나의 값만 리턴 가능
- 여러 개의 값을 리턴 받고 싶을 때
  - 전역 변수를 사용
  - 포인터를 이용
  - 구조체 변수를 사용

### static
- static = 정적
- static 키워드를 쓰는 곳 마다 역할이 다름
  - 지역 변수에 static
    - 함수에서만 쓸 수 있는 전역변수로 취급됨
    - 함수 외부에서 불러쓰지는 못하지만, 함수내에 해당 값이 남아있어서 계속 유지가능
  - 함수에 static
    - 현재 사용중인 c파일 내에서만 사용 가능
    - 다른 파일이 사용 못하는 함수
  - 전역 변수에 static
    - 현재 사용중인 c파일 내에서만 사용 가능
    - 다른 파일이 사용 못하는 전역변수

### Preprocessor 과정
#### Preprocessor 역할
- 컴파일 하기 전 전처리 과정
  - c 파일을 읽어 전처리를 한 후, i 파일로 만듬
  - "전처리기 지시문"들을 처리(\*.i 파일) 
    - \#include : 파일 내용 그대로 복사
    - \#define : 글자 그대로 치환
    - \#if / \#ifdef
    - \#pragma : 컴파일러 전용 전처리기 지시문
- 컴파일은 파일을 하나만 번역
- 프리프로세서도 하나의 파일씩 처리

#### \#ifdef문
- \#ifdef '이름' : \#define '이름'이 되어 있을때 실행
- \#ifndef '이름' : \#define '이름'이 되어 있지 않을 때 실행
- \#else : \#ifdef, \#ifndef가 선언되고 그 외의 조건에서 실행
- \#endif : \#ifdef, \#ifndef 종료
- \#undef : \#def 제거

#### \#if문
- \#if문은 \#ifdef와 달리 값으로 코드 수행여부 결정
  - \#if
  - \#else
  - \#elif
  - \#endif
```
#if 0
// Test Case
#endif
```
- 코드를 포함시키지 않는 용도
```
# if defined FT_H
...
#endif
- #if defined
  - 하나만 쓰면 #ifdef와 동일
  - defined를 쓰면 &&, ||, ==, !=, >< 등 연산 기호를 사용 할 수 있음
```

#### \#define을 쓰는 이유
- Build System에서 \#define을 추가해 줄 수 있음
- GCC 옵션
  - gcc -D [define 이름]
  - gcc -D [define 이름]=[값]
- Makefile 수정
  - gcc -D [define 이름] 옵션을 사용
- 활용
  - Hardware 초기화 코드
  ```
  #ifndef ENGINE
  #error
  #endif
  
  ...
  - ENGINE이 있어야 동작
  ```
- 임베디드 Debug 모드
  - 개발시는 Debug : 로그 메세지 다량, Assert문 다량, Dump
  - 배포시는 Release : 로그 제거, Assert 제거

