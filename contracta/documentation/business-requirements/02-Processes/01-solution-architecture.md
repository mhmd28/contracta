# Solution Architecture
<h5>The Contracta solution is designed to solve real estate company and building contractors managerial challenges revolving around project and human resource management and monitoring.
Contracta Systems:</h5>
1. Attendance Monitoring System (AMS).
2. On-Site Project Monitoring System (SPMS).
3. Project Management System (PMS).

* Components Diagram:
```plantuml
@startuml
rectangle "Contracta Solution" as CONTRACTA {
    component AMS
    component SPMS
    component PMS
}
actor Engineers 
note bottom of CONTRACTA
  Contracta is the name of the 
  solution including these systems
end note


''' INTERACTIONS
Head_of_Engineers -> PMS
Engineers -> SPMS 
Employees -> AMS
HR_Team -> AMS
Managers -> AMS
PMS <- SPMS
SPMS -> AMS


@enduml
```