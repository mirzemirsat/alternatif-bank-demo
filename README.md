# Digital Banking | Account & Transfer Demo

Örnek hesaplar üzerinden bakiye görüntüleme ve para transferi akışını gösteren bankacılık arayüzü demosu.

## Özellikler

- Hesap listesi, isim/IBAN araması ve hesap detayı.
- Hesap hareketleri ve sayfalı transfer geçmişi.
- Gönderen/alıcı ve bakiye kontrolleri bulunan transfer akışı.
- Türk lirası ve Türkçe tarih biçimlendirmesi.

## Teknolojiler

Next.js **13.5.1**, React 18, TypeScript, Tailwind CSS ve shadcn/ui. Sürüm bilgisi `package.json` ile eşleştirilmiştir.

## Yerel çalıştırma

```bash
git clone https://github.com/mirzemirsat/DENEMEEE.git
cd DENEMEEE
npm ci
npm run dev
```

Varsayılan adres `http://localhost:3000`. Kontroller: `npm run typecheck`, `npm run lint`; derleme: `npm run build`, ardından `npm start`.

## Demo kapsamı

`lib/api.ts`, `lib/mock-data.ts` içindeki örnek kayıtlarla çalışır. Gerçek banka API'si veya gerçek para hareketi yoktur. İstemci içindeki demo verileri kalıcı bankacılık kaydı sayılmaz. IBAN alanı kontrolleri banka entegrasyonu veya hesap sahipliği doğrulaması sağlamaz.

Alternatif Bank görsel referansları bir demo tasarımının parçasıdır; resmi banka ürünü veya kurum onayı iddiası yoktur.

## Kaynak yapısı

`app/` sayfaları, `components/` arayüz bileşenlerini, `lib/` mock API ve veri modellerini içerir.

İlişkili, farklı iş akışları içeren demo: [onyuz](https://github.com/mirzemirsat/onyuz).
