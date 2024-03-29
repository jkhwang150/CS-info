# RDB (Realtional DataBase)
 테이블, 행(row), 열(column)의 정보를 구조화하는 방식이다.
- 테이블이라는 최소 단위로 구성되며, 테이블은 하나 이상의 열과 행으로 이루어져 있다.
- 데이터 처리 및 데이터 쿼리를 효율적으로 처리하기 위해 테이블에 저장한다.
- 조인 또는 링크를 설정하여 여러 데이터 포인트 간의 관계를 쉽게 이해하고 정보를 얻을 수 있다.

### 장점
- 스키마가 명확하게 정의되어 있다.
- 데이터 무결성을 보장한다.
- 각 데이터를 중복없이 한 번만 저장한다.

### 단점
- 유연성이 떨어져 데이터 스키마를 사전에 계획해야 하므로 추후 수정이 어렵다.
- 관계를 맺고 있어 조인문이 많은 복잡한 쿼리가 만들어질 수 있다.
- 대체로 수직적 확장만 가능하다.


# NoSQL(비관계형 DB)
- 테이블 형식이 아닌 데이터 유형에 따라 다양한 유형으로 데이터를 저장한다. 주로 문서, 키 값, 와이드 컬럼, 그래프 등을 사용하낟.
- 유연한 스키마를 제공하여 대량의 데이터와 높은 사용자 부하에서도 확장이 가능하다.
- 스키마의 유형에 따라 데이터를 읽어 온다.

### 장점
- 스키마가 없어 유연하게 언저덴지 데이터를 조정하고 새로운 필드가 추가 가능하다.
- 데이터는 필요로 하는 형식으로 저장되어 있기에 읽어오는 속도가 빠르다.
- 수직 및 수평 확장이 가능해 모든 요청에 대한 처리가 가능하다.

### 단점
- 데이터 중복을 업데이트해야 한다.
- 데이터가 여러 컬렉션에 중복되어 수정할 경우 모든 컬렉션에서 수행해야 한다.

# RDB VS NoSQL

### 데이터 저장(Storage)
- RDB같은 경우는 SQL 언어를 통해 테이블에 저장하고 미리 작성된 스키마를 기반으로 정해진 형식에 맞게 데이터를 저장한다.
- NoSQL의 경우 키 값, 문서, 그래프 등 다양한 방식으로 데이터를 저장한다.

### 스키마(Schema)
- RDB는 고정된 스키마가 필요하며 처리하려는 데이터 속성별로 열에 대한 정보를 미리 정해야 한다. 스키마 변경이 가능하지만 DB전체를 수정하거나 오프라인으로 전환해야할 수도 있다.
- NoSQL은 스키마를 유연하게 관리할 수 있다. 즉식 행과 열을 추가할 수 있고 데이터를 반드시 입력하지 않아도 된다.

### 쿼리(Query)
- RDB는 테이블 형식과 관계에 맞춰 데이터를 요청해야 한다. 요청하는 방식이 정해져 SQL 언어와 같이 구조화된 쿼리를 사용한다.
- NoSQL은 데이터 그룹 자체를 조회하는 것에 ㅊ점을 두어 구조화되지 않은 쿼리 언어로도 데이터를 요청할 수 있습니다.

### 확장성(Scalability)
- RDB는 수직적으로 확장하며 많은 메모리와 CPU를 필요로 합니다. 또한 여러 개의 서버에 걸쳐 관계를 정의할 수 있지만 복잡하며 오랜 시간을 소요해야 합니다.
- NoSQL은 수평적으로 확장합니다. 서버를 추가로 구축하면 트래픽 처리가 편해지는데 클라우드 기반의 인스턴스에 호스팅하면 상대적으로 비용이 저렴합니다.
