# Contracta systems users:
```plantuml
@startuml
Engineering as eng
actor Engineers as e
actor Head_of_Engineers as h
h -|> eng
e-|>eng

eng -|> Employee

HR_Team -|> Employee

Managers -|> Employee
@enduml
```