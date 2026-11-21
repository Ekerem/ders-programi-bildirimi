# Kazanım Bildir — web sürümü ve plan dosyaları

**Web sürümü:** https://ekerem.github.io/ders-programi-bildirimi/ (`index.html`, `sw.js`, `version.json`). Haftalık ders programına göre o haftanın öğrenme çıktılarını gösterir; ders programı tarayıcıda saklanır, plan dosyaları bu depodan okunur.

## Plan dosyaları

Bu depo, **Ders Programı Bildirimi** Android uygulamasının internetten güncellediği dosyaları tutar.
Uygulamada **Ayarlar → 🔄 Planları güncelle** düğmesine basıldığında aşağıdaki dosyalar indirilir.

| Dosya | İçerik |
|---|---|
| `surum.json` | Sürüm tarihi, açıklama ve indirilecek dosyaların listesi |
| `takvim.json` | Okul takvimi: hafta numarası → tarih aralığı |
| `plans/dersler.json` | Ders listesi (kod, ad, fotoğrafta aranan kısaltmalar) |
| `plans/KOD_SINIF.json` | Bir dersin bir sınıf düzeyi için haftalık öğrenme çıktıları (ör. `MAT_5.json`) |

## Güncelleme nasıl yapılır?
1. Değişen plan dosyalarını `plans/` klasörüne yükleyin (aynı adla üzerine yazın).
2. Yeni bir ders/sınıf eklediyseniz dosya adını `surum.json` içindeki `dosyalar` listesine ekleyin.
3. `surum.json` içindeki `surum` tarihini değiştirin.

Uygulama tüm dosyaları indirip doğruladıktan sonra eskilerin yerine koyar; bir dosya bozuksa hiçbirini değiştirmez.

Kaynak: MEB Türkiye Yüzyılı Maarif Modeli taslak çerçeve yıllık planları (tymm.meb.gov.tr).
