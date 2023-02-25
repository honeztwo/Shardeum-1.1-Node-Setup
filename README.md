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
# 4 - Githup reposunu klonlayalım :

```
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

# 5 - docker-compose dosyasını oluşturalım :

```
sudo chmod +x /usr/local/bin/docker-compose
```
# 6 - Kurulum dosyasını indirelim :

Y/n gelecek Y basıp enterlayalım,

* Çok Önemli Tekrar Y/N gelecek burada sizden daha sonra kullanmanız için şifre belirlemenizi isteyecek, belirlediğiniz şifreyi unutmayın!!
* Entere bastıktan sonra size bir kaç şey  soracak herhangi bir şey yazmadan hepsine enterlayıp geçin


```
curl -O https://gitlab.com/shardeum/validator/dashboard/-/raw/main/installer.sh && chmod +x installer.sh && ./installer.sh
```



# 7 -  Şimdi Shardeum dosyasına girelim :

```
cd .shardeum
```
Shell dosyasına girelim ;

```
./shell.sh
```

# 7 -  Nodumuzu başlatalım !! 
Bu işlemi yaptıktan sonra nodumuz şuan çalışır durumda olması lazım !

```
operator-cli gui start

```

# 8 -  Dashboard için hazırlıklar 

```
https://localhost:8080/
```
Localhost yazan kısma Vps'in public IP adresini yazalım, örnek verecek olursak ;

https://48.18.153.38:8080/
