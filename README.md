# ADV Player Catalog

Catálogo público de vídeos com audiodescrição usados pelo ADV Player.

## Estrutura

- `catalog.json`: lista de conteúdos disponíveis no aplicativo.
- `descriptions/`: arquivos de audiodescrição no formato `.adv`.
- GitHub Releases: arquivos de vídeo, evitando armazenar mídias grandes no histórico Git.

## Formato do catálogo

```json
{
  "version": 1,
  "videos": [
    {
      "id": "demonstracao",
      "title": "Vídeo de demonstração",
      "language": "pt-BR",
      "videoUrl": "https://github.com/andersonlourenc/adv-player-catalog/releases/download/v1.0-demo/demonstracao.mp4",
      "advUrl": "https://raw.githubusercontent.com/andersonlourenc/adv-player-catalog/main/descriptions/demonstracao.adv"
    }
  ]
}
```

Cada item deve possuir um identificador único, um título, o idioma da audiodescrição e URLs HTTPS para o vídeo e o arquivo ADV.
