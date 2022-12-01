# Basic_CRUD

# 기능 명세서

<aside>
🍪 인터넷 강의를 관리하는 BackOffice

</aside>

- 강의를 추가할 수 있다.
- 강의 목록을 조회할 수 있다.
- 선택한 강의를 조회할 수 있다.
- 선택한 강의 정보를 수정할 수 있다.
- 선택한 강의를 삭제할 수 있다.

# API 설계
|기능|Method|URL|Request|Response|
|---|---|---|---|---|
|강의 추가|POST|/api/save/course|{title: “String”, instructor: “String”, cost: Double}|{msg: “String”, statusCode: int}
|강의리스트 조회|GET|/api/get/courses|0|{"msg": "String”,"statusCode": int,courseList: [{title: “String”, instructor: “String”, cost: Double},{title: “String”, instructor:“String”, cost: Double}, …{title: “String”,instructor: “String”,cost: Double}]}|
|강의 조회|GET|/api/get/course?id=|0|{title: “String”, instructor: “String”, cost: Double}|
|강의 수정|PUT|/api/update/course/{id}|{title: “String”,cost: Double}|{title: “String”, instructor: “String”, cost: Double}|
|강의 삭제|DELETE|/api/delete/course/{id}|0|{msg: “String”, statusCode: int}|
