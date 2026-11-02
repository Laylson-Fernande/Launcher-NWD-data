# Launcher-NWD · dados do mapa

Dados públicos do mapa integrado do app **Launcher-NWD** (central NWD), servidos via **GitHub Pages**:

- `roads/v1/` — radares, limites de velocidade, lombadas, pedágios, passagens de nível
- `maps/v1/` — mapa offline (ruas, água, prédios, nomes…), desenhado pelo app
- `graph/v1/` — grafo de ruas para rota sem internet
- `places/v1/` — índice de endereços (com números de casa do CNEFE) para busca sem internet

Gerados toda semana a partir do **OpenStreetMap** (Geofabrik) e do **CNEFE 2022 (IBGE)** pelo
workflow `.github/workflows/road-data.yml` (gerador em `tools/road-data/`). Formato em
[`tools/road-data/README.md`](tools/road-data/README.md).

O código do app fica num repositório privado separado; este repo é público só porque o app baixa
estes dados sem autenticação.

## Licença dos dados

© OpenStreetMap contributors, sob a [Open Database License (ODbL) 1.0](https://www.openstreetmap.org/copyright).
Endereços do CNEFE 2022 © IBGE, Censo Demográfico 2022.

> Pré-requisito do Pages: Settings → Pages → Source: GitHub Actions.
