다운로드
------------
+ https://kafka.apache.org/downloads


실행
------------
+ kafka 설치 경로로 이동
```
예) C:\kafka\bin\windows
```
+ Zookeeper 실행
```
.\zookeeper-server-start.bat ..\..\config\zookeeper.properties
```

+ kafka 서버 실행
```
.\kafka-server-start.bat ..\..\config\server.properties
```

+ Producer 실행(topic명 'test')
```
.\kafka-console-producer.bat  --broker-list  localhost:9092 --topic test
```

+ Consumer 실행(topic명 'test')
```
.\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic test --from-beginning
```
