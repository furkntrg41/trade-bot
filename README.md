# Trade Bot

Python ile geliştirilmiş kripto para algoritmik trading botu.

## Özellikler

- Binance entegrasyonu ile otomatik alım/satım
- Docker ile containerize edilmiş deployment
- Hetzner sunucu kurulum scriptleri
- Çoklu strateji ve optimizasyon desteği

## Hızlı Başlangıç

```bash
# Konfigürasyonu düzenle
cp config.json.example config.json

# Docker ile başlat
docker-compose up -d

# Durumu kontrol et
docker-compose logs -f
```

## Deployment

```bash
# Hetzner sunucu kurulumu
bash HETZNER_KUR.bat

# Production deployment
bash deploy_production.sh
```

## Proje Yapısı

```
config/              # Strateji konfigürasyonları
user_data/           # Bot verileri ve loglar
archive/             # Eski strateji arşivi
referanslar/         # Teknik referans dökümanları
```
