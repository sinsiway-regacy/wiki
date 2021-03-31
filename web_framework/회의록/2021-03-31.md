## 2021-03-31 [Web Framewok] 회의록

**1. Wiki 플랫폼**

github wiki를 활용하여 markdown으로 페이지 작성

https://github.com/sinsiway/wiki/wiki



**2. DB 접근 방식**

| 방식                  | 설명                                                         | 비고                                             |
| --------------------- | ------------------------------------------------------------ | ------------------------------------------------ |
| 기존 DAO 클래스 방식  | @Repository 지정 및 EgovAbstractMapper extends 활용          | 기존 iBatis와 같은 방식                          |
| Mapper interface 방식 | Mapper 인터페이스 작성 및 @Mapper annotation 지정            | @Mapper는 marker annotation(표준프레임워크 제공) |
| Annotation 방식       | query xml 없이 mapper 인터페이스 상 @Select, @Insert 등을 활용 | Dynamic SQL 등의 사용에 제약이 있음              |

Mapper interface 방식을 표준으로 결정

