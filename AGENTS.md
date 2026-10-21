# Instruções para agentes

<!-- DISCOS-LOCAIS:INICIO -->
## Discos desta máquina (decisão do proprietário em 21/10/2026)

- **HD de referência: o NAS** (`/media/guilherme/NAS_GUILE`). Originais, backups e checkpoints dos
  projetos ficam nele; bancos ativos ficam no SSD local, com cópia conferida no NAS.
- **O SanDisk `RCV_Disk` (`/media/guilherme/RCV_Disk`) está corrompido desde 17/10/2026: não ler
  nem gravar nele.** Tudo o que só existia nele foi copiado para o NAS e conferido por SHA-256.
- Caminho com `RCV_Disk` em material novo é erro; em registro antigo, indica onde o arquivo estava
  na época (o mesmo caminho relativo existe no NAS).
- Acervos locais — FAF, CZUR/Scan, Projects and articles e Imports: `~/.local/bin/acervos diagnostico`,
  busca conjunta com `acervos buscar`, e o guia `/media/guilherme/NAS_GUILE/Acervos_Integracao/GUIA_AGENTES.md`.
- Execução na nuvem não tem acesso a esses discos; dados, bancos e PDFs não entram no Git.
<!-- DISCOS-LOCAIS:FIM -->
