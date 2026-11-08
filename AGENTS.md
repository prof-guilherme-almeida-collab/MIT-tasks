# Instruções para agentes

<!-- DISCOS-LOCAIS:INICIO -->
## Discos desta máquina (decisão do proprietário em 08/11/2026, que revê a de 21/10/2026)

- **Disco de trabalho: o SSD interno de 1 TB** (`/mnt/dados`, rótulo `dados`). Bancos ativos, treinos e
  dados de trabalho ficam nele; o disco do sistema (512 GB) fica para o sistema. Os caminhos antigos em
  `/home` continuam valendo como atalhos (ex.: `~/integrated_search_local/acervos`,
  `~/Documentos/guile/Scan`, treinos em `~/futuro_video_local/voz/`). Dado novo de trabalho vai para `/mnt/dados`.
- **NAS (`/media/guilherme/NAS_GUILE`, SSD externo USB): cópia extra, mobilidade entre máquinas e
  backup.** O comando `~/.local/bin/sincronizar-nas` copia, em mão única (máquina → NAS), `/mnt/dados` para
  `NAS_GUILE/espelho-dados/<máquina>/` e os repositórios (bundles git, status e diffs) para
  `NAS_GUILE/backup/repositorios/<máquina>/`. Originais que só existem no NAS (PDFs dos acervos, vídeos,
  vozes aprovadas) continuam lá: não apagar nada do NAS.
- **O SanDisk `RCV_Disk` (`/media/guilherme/RCV_Disk`) está corrompido desde 17/10/2026: não ler
  nem gravar nele.** Caminho com `RCV_Disk` em material novo é erro; em registro antigo, indica onde o
  arquivo estava na época (o mesmo caminho relativo existe no NAS).
- Acervos locais — FAF, CZUR/Scan, Projects and articles e Imports: `~/.local/bin/acervos diagnostico`,
  busca conjunta com `acervos buscar`, e o guia `/media/guilherme/NAS_GUILE/Acervos_Integracao/GUIA_AGENTES.md`.
- Execução na nuvem não tem acesso a esses discos; dados, bancos e PDFs não entram no Git.
<!-- DISCOS-LOCAIS:FIM -->
