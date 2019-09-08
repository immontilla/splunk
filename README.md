# splunk

Splunk Playground

1. Generate a random password issuing
```console
export RANDOMPASS=`date +%s | sha256sum | base64 | head -c 32 ; echo`
```
2. Read its value and store it safely
```console
echo $RANDOMPASS
```
3. Up!
```console
docker-compose up -d
```

Log into Splunk opening the url http://localhost:8000 using admin as username and the password generated previously.