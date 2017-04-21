# puml


{% plantuml %}

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

{% endplantuml %}


## Usecase

{% plantuml %}
@startuml

(First usecase)
(Another usecase) as (UC2)  
usecase UC3
usecase (Last\nusecase) as UC4

@enduml
{% endplantuml %}

