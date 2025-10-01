Address Management App (Adres Yönetim Uygulaması)
Bu proje, bir .NET Minimal API backend'i ve React (Vite/Material UI) frontend'inden oluşan full-stack bir Adres Yönetim Uygulamasıdır.


🛠️ Teknolojiler
Kategori

Teknoloji

Açıklama

Backend

.NET 8 Minimal API (C#)

Hızlı ve hafif CRUD ve Parsing işlemleri için.

Frontend

React (Vite)

Modern, hızlı ve state yönetimini kolaylaştıran yapı.

UI/Styling

Material-UI (MUI)

Profesyonel ve erişilebilir kullanıcı arayüzü bileşenleri.

Veritabanı

In-Memory List

Mülakat gereksinimine uygun olarak geçici veri saklama.

🚀 Projeyi Çalıştırma Talimatları
Projenin hem backend hem de frontend kısımlarını çalıştırmak için iki ayrı terminal kullanmanız gerekmektedir.

1. Backend'i Başlatma
Bu, CRUD ve Ukraynaca metin ayrıştırma (parsing) hizmetlerini sunan API'dır.

# Terminal 1: Backend
cd AddressApp.Api
dotnet run

API, varsayılan olarak http://localhost:5000 adresinde çalışacaktır.

2. Frontend'i Başlatma
Bu, kullanıcı arayüzünü (React) çalıştırır.

# Terminal 2: Frontend
cd address-app-client
npm install      # Sadece ilk çalıştırmada veya node_modules silindikten sonra gereklidir
npm run dev

Frontend, varsayılan olarak http://localhost:5173 adresinde veya benzer bir portta çalışacaktır.

✨ Uygulanan Özellikler ve Bonuslar
Bu projede temel CRUD işlemlerinin yanı sıra aşağıdaki özellikler entegre edilmiştir:

Gelişmiş Arama/Filtreleme: Frontend'de tüm alanlarda (ülke, şehir, adres vb.) anlık, dinamik arama ve filtreleme özelliği mevcuttur.

Toplu Veri İşleme (Parsing):

Backend'de, Ukraynaca dahil olmak üzere tek bir metin dizesinden Regex kullanılarak ülke, şehir ve adres bilgilerinin ayrıştırılması uygulanmıştır.

POST /api/addresses/parse endpoint'i bu işlevi yerine getirir.

Kullanıcı Arayüzü (UI): Proje, modern ve yüksek kaliteli bir kullanıcı deneyimi sunmak için Material-UI (MUI) kullanılarak tasarlanmıştır.

📁 Proje Yapısı
.
├── AddressApp.Api/             # .NET Minimal API Backend
│   ├── Program.cs              # Ana API ve Endpoint Tanımları
│   └── Models/Address.cs       # Adres modeli
├── address-app-client/         # React Frontend Projesi
│   └── src/App.jsx             # Tüm UI ve Frontend Logic
└── README.md

