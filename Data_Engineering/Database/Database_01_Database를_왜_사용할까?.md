## Why Database?

<br>
<br>

### Information System

- 조직 운영에 필요한 데이터를 수집하여 저장해 두었다가 필요할 때 유용한 정보를 만들어 주는 수단

<br>
<br>

### 정보 시스템의 발전 : (1) File System

- 데이터를 파일로 관리하기 위해 파일을 생성, 삭제, 수정, 검색하는 기능을 제공하는 소프트웨어

- 응용 프로그램마다 필요한 데이터를 별도의 파일로 관리

<br>

**Limitations of File System**

    - 같은 내용의 데이터가 여러 파일에 중복 저장
    - 응용 프로그램이 데이터 파일에 종속적
    - 데이터 파일에 대한 동시 공유, 보안, 회복 기능이 부족
    - 응용 프로그램 개발 어려움

**Data Redundancy**

    - 같은 내용의 데이터가 여러 파일에 중복 저장
        - 저장 공간의 낭비
        - 데이터 일관성과 데이터 무결성을 유지 어려움

**Data Dependency**

    - 응용 프로그램이 데이터 파일에 종속적
        - 사용하는 파일의 구조를 변경하면 응용 프로그램도 함께 변경해야 함.

<br>
<br>

### 정보 시스템의 발전 : (2) Database System

- DBMS(Database Management System)를 도입하여 데이터를 통합 관리하는 시스템
- DBMS가 설치되어 데이터를 가진 쪽을 서버(Server), 외부에서 데이터 요청하는 쪽을 클라이언트(Client)라고 함.
- DBMS 서버가 파일을 다루며 데이터 일관성 유지, 복구, 동시 접근 제어 등을 수행
- 데이터의 중복을 줄이고 데이터를 표준화하며 무결성을 유지함.

<br>
<br>

### 정보 시스템의 발전 : (3) Web Database System

- 데이터베이스를 웹 브라우저에서 사용할 수 있도록 서비스하는 시스템
- 불특정 다수 고객을 상대로 하는 온라인 상거래나 공공 민원 서비스 등에 사용됨

<br>
<br>

### 정보 시스템의 발전 : (4) Distributed Database System

- 여러 곳에 분산된 DBMS 서버를 연결하여 운영하는 시스템
- 대규모 응용 시스템에 사용됨

<br>
<br>

### File System vs. Database System

| **구분** | **파일 시스템** | **DBMS** |
| --- | --- | --- |
| 데이터 중복 | 데이터를 파일 단위로 저장하므로 중복 가능 | DBMS를 이용하여 데이터를 공유하기 때문에 중복 가능성 낮음 |
| 데이터 일관성 | 데이터의 중복 저장으로 일관성이 결여됨 | 중복 제거로 데이터의 일관성이 유지됨 |
| 데이터 독립성 | 데이터 정의와 프로그램의 독립성 유지 불가 | 데이터 정의와 프로그램의 독립성 유지 가능 |
| 관리 기능 | 보통 | 데이터 복구, 보안, 동시성 제어, 데이터 관리 기능 등을 수행 |
| 프로그램 개발 생산성 | 나쁨 | 짧은 시간에 큰 프로그램을 개발할 수 있음 |
| 기타 장점 | 별도의 소프트웨어 설치가 필요 없음 
(운영체제가 지원) | 데이터 무결성 유지, 데이터 표준 준수 용이 |