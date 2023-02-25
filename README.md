#  :
```

```



𝗦𝗽𝗵𝗶𝗻𝘅 1.1 Node Setup

Türkçe kaynak bulamadağım için bu şekilfe bir repo hazırlayayım dedim.

Ben Vps sağlayıcı olarak Digitalocean kullanıyorum, 

# Minimum Sistem Gereksinimleri :
```
-250 GB SSD storage
-16 GB of ram,  4+ GB of virtual memory recommended
-Hosting: 8 GB RAM + 8 GB Virtual Memory
```
# 1 - İlk önce güncellemeleri yapalım :
```
sudo apt update && apt upgrade -y
```
# Karşınıza bu şekilde bir ekran çıkarsa 1 2 3 4 5 6 yazıp enter basın :
```
![image]https://prnt.sc/7IbLq7sw5FaU
```
# 2 -  Curl kurulumu yapalım :
```
sudo apt-get install curl 

```
# 3 - Docker kurulumu yapalım :
```
sudo apt install docker.io

```

# 3 - Docker Versiyonu kontrol edelim, eğer versiyon ile alakalı çıktı  aldıysanız sorun yok demektir. :
```
docker --version

```
