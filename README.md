# Mynodes
My notes
Kendi yaşadığıdım sorunlara bulduğum çözümleri sıraladım, çözümler yüzde yüz doğru ve kesin çalışıyor diyemem kendim için açtığım repo. 

Eğer Docker permisison denied hatası alırsan. 

```$ sudo groupadd docker```

```$ sudo usermod -aG docker $USER```


```$ newgrp docker```


Sistem ne kadar dolu bakmak için

```df -h ```

RAM kullanımı 
```htop```


SSH bağlantısı yaparken SSH durumuna bakma 

```sudo systemctl status ssh```

Eğer yoksa 

```sudo apt update```

```sudo install openssh-server```


Waiting for cache lock: Could not get lock hatası

```lsof burayahatadakikonumuyaz```
Gelen yerde büyük ihtimalle COMMAND PID gibi bir ekran gelir, PID ile işlem yapacağız

```sudo kill -9 PID```

Şimdi tekrardan kurmaya çalıştığınız paketi deneyebilirsiniz.

!! Bu hatanınn neden olduğunu çözmeedim, sunucumda çok fazla ir şey olmadığı için biraz araştırma yapıp kendim denedim ve oldu. Siz kullanacaksanız ona göre kullanın.


remote setup commands

```sudo apt install xrdp```
```sudo systemctl status xrdp```
```sudo systemctl start xrdp```
```sudo systemctl enable xrdp```
```sudo ufw allow from any to any port 3389 proto tcp```

Eğer kullancı adınız sudoers kısmında yok diye bir hata alıyorsanız 
```su -```
şifreyi girin 
```visudo```
bir dosya açılacak en altta # User privilege specification yazacak ve altında root ve sonrasındaki ALL yazan kısımları kopyala bir altına yapıştır ve root yerine kullanıcı adını yaz 

