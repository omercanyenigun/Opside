# Sık Sorulan Sorular

![alt text](https://i.hizliresim.com/8nzb9w2.jpeg)

## Şu anda V2 kullanıyorum, V3'e geçmem gerekiyor mu?
Validadçr sorunsuz çalışıyorsa geçiş yapmanıza gerek yoktur.

## Hangi durumlarda V3'e geçmem gerekiyor?

Aşağıdaki durumlarda V3'e geçmeyi düşünebilirsiniz:

- İlk kez bir validatör çalıştırırken, V3 önerilir.
- Validatörünüzü yeni bir VPS'ye taşımak istiyorsanız, V3'ü yeni VPS'ye yükleyin.

## V3'e nasıl geçilir

Şu anda V2 kullanıyorsanız

- Mnemonicleri yedeklediğinizden emin olun (24 kelime)
- Adım: V2 ile çalışan tüm istemcileri durdurun
- Adım: V3'ü yükleyin
- Adım: V3'ü çalıştırın ve mnemonicleri içe aktarın
- Adım: Validatörünüzü çalıştırmak için CLI istemlerini izleyin.


## v3 Bunları Destekler

- Senkronizasyon Modunun seçilmesi desteklenir
- Hızlı mod: Yüksek senkronizasyon hızı.
- Normal mod: Yavaş senkronizasyon hızı (hızlı modda hatalar olduğunda normal modu kullanın)
- Mnemonicleri içe aktarma desteklenir
- Yeni mnemoniz oluşturma
- Mevcut mnenonic'i içe aktarma

## Programı Kurun ve Çalıştırın

```python
wget -c https://pre-alpha-download.opside.network/testnet-auto-install-v3.tar.gz && tar -C ./ -xzf testnet-auto-install-v3.tar.gz && chmod +x -R ./testnet-auto-install-v3 && cd ./testnet-auto-install-v3 && ./install-ubuntu-1.0.sh
```

## 1. Adım: Senkronizasyon Modunu Seçin

Hızlı mod için 1 Normal mod için 2 girin.

## 2. Adım: Mnemoniz içe aktarma türünü seçin

Eğer yeni kurulum yapıyorsanız yeni mnemonic oluşturun. Taşıma yapıyorsanız mnemonic içe aktarmayı seçin.

## 3. Adım: Log Kontrolü

NOT: Beacon kurulumundan sonra, staking depozitonuzu göndermeden önce tamamen senkronize olduğunuzdan emin olun.


```python
cd testnet-auto-install-v3
```

geth log:        

```python
opside-chain/show-geth-log.sh
```

beaconChain log: 

```python
opside-chain/show-beaconChain-log.sh
```

validator log:   

```python
opside-chain/show-validator-log.sh
```

NOT: Blok yüksekliğinin son block'a yakın olup olmadığını görmek için https://pre-alpha.opside.info 'yu kontrol edin. evet ise, IDE'nin yatırılma zamanı gelmiştir.

## 4. Adım: Stake İşlemi

- Nodeunuz sync olduktan sonra Bu siteye gidin: https://opside.network/validator/deposit

- WinSCP veya benzeri uygulama ile nodeunuzun olduğu sunucuya bağlanıp istenilen klasörü bilgisayarınıza indirin. 

- Dosya Dizini: /root/testnet-auto-install-v3/validator_keys/deposit_data

- Sitede Upload Deposit Data'ya kadar ilerleyin. Buradan winSCP ile indirdiğiniz data klasörünü yükleyin.

![alt text](https://i.hizliresim.com/74p6s50.png)

![alt text](https://i.hizliresim.com/f9lwjrc.png)

Discord'dan token aldığınız metamask cüzdanınızı bağlayın.

![alt text](https://i.hizliresim.com/32jskiy.png)

Opside Testnet ağını Metamask'a ekleyin.

![alt text](https://i.hizliresim.com/h6jwupt.png)


25000 IDE'yı stake edin.

## Çıktılar


![alt text](https://i.hizliresim.com/fdrz31b.png)

![alt text](https://i.hizliresim.com/pq9kd95.png)


## Explorer: https://pre-alpha-beacon.opside.info/





