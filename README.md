# Java Dizayn Pattern

Factory, Singleton ve Strategy tasarım desenlerini Türkçe, günlük hayattan örneklerle anlatan küçük Java projeleri.

> **Not:** Bu depo 2017 yılında eğitim amaçlı yazıldı ve artık güncellenmiyor.

## İçerik

| Klasör | Ne yapar | Çalıştırılacak sınıf |
|---|---|---|
| `FactoryDizaynPattern` | Bursa fabrikası `arabaUret` ile Murat 131, Doğan ve Şahin üretir; satış bayisi siparişi kredi, sigorta, plaka ve teslim adımlarından geçirir | `com.mustafaergan.cars.TestDrive` |
| `SingletonDizaynPattern` | `getInstance()` ile tek bir nesnenin tekrar tekrar kullanıldığını gösterir | `com.mustafaergan.sing.SingletonClient` |
| `StrategyDizaynPattern` | Bir yazılım şirketinde IT uzmanlarının kod yazma ve test etme davranışlarını çalışma anında değiştirir (`KodYazabilme`, `TestEdebilme`) | `com.mustafaergan.mysoftwarecompany.Sirket` |

## Teknolojiler

- Java 8 (yalnızca standart kütüphane, dış bağımlılık yok)

## Çalıştırma

Her klasör ayrı bir Eclipse projesidir. Eclipse'te *File > New > Java Project* ile klasörü konum olarak
gösterip açabilir ya da komut satırından derleyebilirsiniz:

```bash
cd FactoryDizaynPattern
javac -encoding windows-1254 -d out $(find src -name "*.java")
java -cp out com.mustafaergan.cars.TestDrive
```

Bazı kaynak dosyalar Windows-1254 kodlamasıyla kaydedildiği için `-encoding windows-1254` verilmiştir.
