#### Service list 조회
```
ros2 service list
```
#### 서비스 정의
```
ros2 service type
 ex) ros2 service type /turtle1/teltport_absolute
```
#### 서비스 정의 조회 내용
```
ros2 intetface show
 ex) ros2 interface show turtlesim/srv/TeleportAbsolute
```
#### Service Request
```
ros2 service call <service name> <service definition> "data"
 ex) ros2 service call /turtle1/teleport_absolute turtlesim/srv/TeleportAbsolute "{x: 2, y:2, theata: 1.57}"
```
#### Service Reset, Reset의 Service Definition 확인
```
ros2 service type /reset
 -> std_srvs/srv/Empty
 ex) ros2 service call /reset std_srvs/srv/Empty {}
```
