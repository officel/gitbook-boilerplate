# uml

## memo

* "uml"プラグインでWARNが出力されてGitBookが公開できないので見送り中

```uml
@startuml

class User {
  username
  password
  +sign_in()
}

class Group {
  name
}

class Member {
  roles
}

User .. Member
Group .. Member

@enduml
```

## Usecase

```uml
@startuml

(First usecase)
(Another usecase) as (UC2)  
usecase UC3
usecase (Last\nusecase) as UC4

@enduml
```
