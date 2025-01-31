## download agent.jar file and run this jar
```bash
curl -sO http://192.168.164.132:8080/jnlpJars/agent.jar
nohup java -jar agent.jar -url http://192.168.164.132:8080/ -secret cea1717f58a77cc4065607887368acb85408c7351dbc91020cd71e31536a542d -name "frappe-bench" -webSocket -workDir "/home/frappe" > nohup.out 2>&1 &
```
## kill process by its name 
```bash
pkill -f agent.jar
```
