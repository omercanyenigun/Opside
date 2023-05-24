## Opside PoS Guide
![alt text](https://i.hizliresim.com/8nzb9w2.jpeg)

# Donanım

- İşletim Sistemi: 64-bit Linux, Mac OS X 10.14+, Windows 10+ 64-bit (Ubuntu 20.04+)

- CPU: 4

- Ram: 16GB

- Disk: En az 500 GB boş alana sahip SSD (mainnette 2 TB önerilir)

## PoS Rewards

Opside, ETH 2.0'ın geliştirilmiş bir sürümüne dayalı bir PoS konsensüsü kullanır. Validatör olarak katılmak için, kullanıcıların belirli bir miktarda IDE'yi yatırma sözleşmesine yatırması ve üç ayrı yazılım çalıştırması gerekir: yürütme istemcisi, mutabakat istemcisi ve validatör. Validatörler, ağ üzerinden yayılan yeni blokların geçerliliğini doğrulamaktan ve zaman zaman kendileri yeni bloklar oluşturup yaymaktan sorumludur. Bir validatör dürüst olmayan veya ihmalkar davranırsa, stake edilen IDE kaybedilecektir.

PoS kapsamında, Opside sabit bir blok üretim hızına sahiptir ve süre yuvalara (12 saniye) ve dönemlere (32-zaman dilimleri) bölünmüştür. Her yuvada, rastgele seçilen bir validatör, yeni bloklar oluşturmaktan ve bunları ağdaki diğer nodelara göndermekten sorumlu blok savunucusu olarak hizmet eder. Ek olarak, her yuvada, oylarını kullanarak önerilen bloğun geçerliliğini belirlemek için validatörlerden oluşan bir komite rastgele seçilir. Kesin mekanizma için lütfen ETH PoS'a bakın.

Opside, Alpha test ağında EIP-4844'ü desteklemeyi planlıyor ve ZK-Rollup'ın yürütme sonrasında tek tek nodelara aşırı yük bindirmeden işlem verileri sağlamasını sağlamak için Veri Kullanılabilirliği Örneklemesini (DAS) kullanıyor. Validatörler, tüm verilerin mevcut olduğunu doğrulamak için blobtaki işlem verilerini rastgele örnekler. Bu teknik aynı zamanda blok üreticilerinin tüm verilerini güvenli hafif istemciler için kullanılabilir hale getirmesini sağlayabilir. Teklif Veren-Oluşturan Ayrımı (PBS) altında, yalnızca blok oluşturucunun tüm bloğu işlemesi gerekirken, diğer validatörler doğrulama için veri kullanılabilirliği örneklemesini kullanır.

Genel olarak staking, ağ korumasına katılımı basitleştirir ve ademi merkeziyetçiliği destekler. Validatör nodelar, standart dizüstü bilgisayarlarda çalıştırılabilir ve bazı proxy staking pooları, kullanıcıların yeterli bir IDE bakiyesi olmadan stake yapmasına bile izin verir.

NOT: vALİDATÖR olmak için, yatırma sözleşmesine 25000 IDE yatırmanız gerekir.

## Kontrol Noktası Senkronizasyonu

```python
wget -c https://pre-alpha-download.opside.network/testnet-auto-install-v2.tar.gz 
tar -C ./ -xzf testnet-auto-install-v2.tar.gz
chmod +x -R ./testnet-auto-install-v2
cd ./testnet-auto-install-v2
```
