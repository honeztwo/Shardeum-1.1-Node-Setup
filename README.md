

𝗦𝗽𝗵𝗶𝗻𝘅 1.1 Node Setup


![_tKXncPnvvrDHTwvr-JDG](https://user-images.githubusercontent.com/95377480/221382041-c992c2fc-c673-44e1-931d-eb473e0552ed.jpeg)


Türkçe kaynak bulamadağım için bu şekilfe bir repo hazırlayayım dedim.

Ben Vps sağlayıcı olarak Digitalocean kullanıyorum, 

# Minimum Sistem Gereksinimleri :

```
-250 GB SSD storage
-16 GB of ram,  4+ GB of virtual memory recommended
-Hosting: 8 GB RAM + 8 GB Virtual Memory
```


Benim oluluşturduğum node ;

```
2 Cpu
4 Gb Ram
160 GB Sdd

```
# 1 - İlk önce güncellemeleri yapalım :

```
sudo apt update && apt upgrade -y
```
# Karşınıza bu şekilde bir ekran çıkarsa 1 2 3 4 5 6 yazıp enter basın :

![Screenshot_1](https://user-images.githubusercontent.com/95377480/221381921-4a2ef8d5-64d2-481e-abb2-7f616e5f6adb.png)

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
![Screenshot_7](https://user-images.githubusercontent.com/95377480/221381927-9bcb4e16-964d-4356-b16d-0c67a44c1b88.png)

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
*![Screenshot_2](https://user-images.githubusercontent.com/95377480/221381923-e6b1158e-1c59-4874-bab2-4f7882302477.png)

*![Screenshot_3](https://user-images.githubusercontent.com/95377480/221381924-610ff278-0217-4992-90b7-1d69410a993b.png)

*![Screenshot_4](https://user-images.githubusercontent.com/95377480/221381926-972ae0f5-a5ec-4d38-b64d-c110de4d20cf.png)




Buradaki işlemler biraz uzun sürüyor beklemek lazım.

![Screenshot_5](https://user-images.githubusercontent.com/95377480/221382097-54947dbf-bd18-42fe-8e87-9b7590d85f37.png)

# 7 -  Şimdi Shardeum dosyasına girelim :

```
cd .shardeum
```
Shell dosyasına girelim ;

```
./shell.sh
```

# 8 -  Nodumuzu başlatalım !! 
Bu işlemi yaptıktan sonra nodumuz şuan çalışır durumda olması lazım !

```
operator-cli gui start

```
*![Screenshot_6](https://user-images.githubusercontent.com/95377480/221382099-32350eb8-efa0-4807-88b4-fbef9d4f7217.png)

# 9 -  Dashboard için hazırlıklar 

```
https://localhost:8080/
```

Localhost yazan kısma Vps'in public IP adresini yazalım, örnek verecek olursak ;

https://48.18.153.38:8080/

Sonra bunu tarayıcınıza kopyalayıp yapıştırın. 

Sizden validatore bağlanmanız için şifre isteyecek , daha önceden belirlediğiniz şifreyi girip dashboard erişim sağlayabilrisiniz.

![Screenshot_8](https://user-images.githubusercontent.com/95377480/221382211-1450d5a0-3af7-44bb-b06e-01ffed73c500.png)

Buradan validatörü çalıştırıp min 10 Shm stake etmeniz gerekli.


![Screenshot_9](https://user-images.githubusercontent.com/95377480/221382238-079fea1d-89d2-4f1a-b042-901f735837d1.png)
![Screenshot_10](https://user-images.githubusercontent.com/95377480/221382239-d6dae581-3f3b-453b-9293-e2c20da6eb4c.png)


