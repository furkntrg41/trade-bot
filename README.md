<div align="center">

# Trade Bot

**Python tabanlı kripto para algoritmik trading botu**

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![Docker](https://img.shields.io/badge/Docker-ready-2496ED?style=flat-square&logo=docker&logoColor=white)](https://docker.com)
[![Binance](https://img.shields.io/badge/Exchange-Binance-F0B90B?style=flat-square&logo=binance&logoColor=black)](https://binance.com)
[![License](https://img.shields.io/badge/License-MIT-22c55e?style=flat-square)](LICENSE)

</div>

---

## Özellikler

- Binance Futures entegrasyonu ile otomatik alım/satım
- Docker ile containerize edilmiş, production-ready deployment
- Hetzner VPS tek-komut kurulum scriptleri
- Çoklu strateji desteği ve performans optimizasyonu
- Unified bot mimarisi ile strateji karşılaştırma

---

## Hızlı Başlangıç

### Gereksinimler
- Docker & Docker Compose
- Binance API anahtarları

### Kurulum

```bash
# Repo'yu klonla
git clone https://github.com/furkntrg41/trade-bot.git
cd trade-bot

# Docker ile başlat
docker-compose up -d

# Logları takip et
docker-compose logs -f
```

---

## Deployment

### Hetzner VPS (önerilen)

```bash
# Sunucu kurulumu (tek komut)
cat HETZNER_TEK_KOMUT.txt

# Ya da adım adım:
bash server_setup.sh
bash HETZNER_KUR.bat
```

### Production

```bash
bash deploy_production.sh
# veya
docker-compose -f docker-compose.production.yml up -d
```

---

## Proje Yapısı

```
.
├── config.json                   # Ana bot konfigürasyonu
├── docker-compose.yml            # Development ortamı
├── docker-compose.production.yml # Production ortamı
├── deploy_production.sh          # Production deployment scripti
├── server_setup.sh               # Sunucu ilk kurulum scripti
├── config/                       # Strateji konfigürasyonları
├── user_data/                    # Bot çalışma verisi ve loglar
├── archive/                      # Geçmiş strateji arşivi
└── referanslar/                  # Teknik referans dökümanları
```

---

## Dökümanlar

| Dosya | İçerik |
|-------|--------|
| [BOT_COMPARISON_DECISION.md](BOT_COMPARISON_DECISION.md) | Strateji karşılaştırma kararları |
| [OPTIMIZATION_SUMMARY.md](OPTIMIZATION_SUMMARY.md) | Optimizasyon sonuçları |
| [PRODUCTION_DEPLOYMENT.md](PRODUCTION_DEPLOYMENT.md) | Production deployment rehberi |
| [QUANT_ARBITRAGE_ANALYSIS.md](QUANT_ARBITRAGE_ANALYSIS.md) | Kantatitatif arbitraj analizi |
| [COMMANDS_REFERENCE.md](COMMANDS_REFERENCE.md) | Komut referansı |

---

## Lisans

[MIT](LICENSE) © 2026 furkntrg41
