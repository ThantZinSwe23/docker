# Docker Usage Command

```bash
docker ps
```
လက်ရှိ Run နေတဲ့ Container List ကိုထုတ်ပြချင်ရင်သုံးသည်။

```bash
docker ps -a
```
Container List အားလုံးကိုထုတ်ပြချင်တဲ့အခါမှာသူံးသည်။

```bash
docker rm <container-name> or <container-id>
```
Container တစ်ခုဖျက်ချင်တဲ့အခါမှာသူံးသည်။

```bash
docker rmi <image-name> or <image-id>
```
Image တစ်ခုဖျက်ချင်တဲ့အခါမှာသူံးသည်။

```bash
docker image ls -q 
```
Image အားလုံးရဲ့ ID ကိုထုတ်ပြချင်တဲ့အခါမှာသုံးသည်။

```bash
docker image rm $(docker image ls -q) 
```
Image အားလူံးကိုဖျက်ချင်တဲ့အခါမှာသုံးသည်။

```bash
docker run
```
Docker Container တည်‌ဆောက်တဲ့အခါမှာသုံးသည်။

```bash
docker run -it 
```
Docker Container ကိုတည်ဆောက်ပြီး Run တဲ့အခါမှာသုံးသည်။

```bash
docker build -t .
```
Dockerfile ကို Docker Image အဖြစ်ပြောင်းတဲ့အခါမှာသုံးသည်။

```bash
docker run -d --name <container-name> -p <local-port:port> <image-name>
```
Docker Image ကို Container အဖြစ်ပြောင်းပြီး Run တဲ့အခါမှာသုံးသည်။

```bash
docker-compose build
```
Dockerfile အားလူံးကို Docker Compose ဖြင့် Docker Image နဲ့ Volume တည်ဆောက်ဖို့အတွက်သုံးသည်။

```bash
docker-compose up -d 
```
Docker Image အားလူံးကို Docker Compose ဖြင့် Docker Container တစ်လူံးတည်ဆောက်ဖို့အတွက်သုံးသည်။

```bash
docker-compose down
```
Docker Compose ဖြင့် Docker Container တစ်လူံးဖျက်ချင်တဲ့အခါမှာသုံးသည်။

```bash
docker exec -it <container-name> /bin/bash
```
Docker Container တစ်လူံးထဲဝင်တဲ့အခါမှာသုံးသည်။
