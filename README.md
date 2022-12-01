# Basic_CRUD

# API 설계
|기능|Method|URL|Request|Response|
|---|---|---|---|---|
|강의 추가|POST|/api/save/course|{title: “String”, instructor: “String”, cost: Double}|{msg: “String”, statusCode: int}
|강의리스트 조회|GET|/api/get/courses|0|{
"msg": "String”,
"statusCode": int,
courseList: [
{
  title: “String”,
  instructor: “String”,
  cost: Double
},
{
  title: “String”,
  instructor: “String”,
  cost: Double
},
           …
{
  title: “String”,
  instructor: “String”,
  cost: Double
}
               ]
}
|강의 조회|GET|/api/get/course?id=|0|
|강의 수정|PUT|/api/update/course/{id}|{title: “String”,cost: Double}|
|강의 삭제|DELETE|/api/delete/course/{id}|0|
