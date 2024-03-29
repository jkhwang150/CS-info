# 컴파일러(Compiler)
프로그램 전체를 스캔하여 고급언어를 기계어(바이트 코드)로 번역한다. C/C++/Java와 같은 언어에 사용한다.

### 컴파일이란?
고급언어로 작성된 파일을 기계어로 변환하는 과정을 말한다.

### 컴파일 과정(java)
1. 프로그래머가 java 언어로 소스코드를 작성합니다.
2. javac 컴파일러를 사용하여 기계어(바이트 코드)로 변환하고 .class파일을 생성한다.
3. 컴파일된 .class파일을 클래스로더로 전달한다.
4. 동적 로딩을 통해 필요한 클래스를 로딩 및 링크하여 런타임 데이터 영역 jvm의 메모리에 올린다.
5. jvm 메모리에 올라온 바이트코드들을 실행엔진을 통해 실행시킨다.

### 특징
- 초기 스캔시간이 오래 걸리지만, 실행 파일이 생성된 후 빠르게 실행이 가능하다.
- 기계어 변환과정에서 더 많은 메모리를 사용한다.
- 전체 코드를 스캔하기 때문에 실행 전에 오류를 발견할 수 있다.

# 인터프리터(Interpreter)
프로그램 실행시 한 번에 한 문장씩 고급언어를 기계어로 변환한다. Python, Ruby, Javascript와 같은 언어에 사용한다.

### 특징
- 한문장씩 번역 후 실행하기에 실행 시간이 느리다.
- 파일을 생성하는 과정이 없어 메모리 효율이 좋다.
- 프로그램을 실행시키고 오류가 발견되면 즉시 중단시킨다.
