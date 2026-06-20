# Requirements

## English

### General & DJ Software
- Music analyzed by Rekordbox must be compatible.
- The system must read cue and memory points.
- Mixxx must allow both CDJ mode and Vinyl mode.

### Hardware Requirements
- Use a Raspberry Pi as the central compute unit.
- Ensure standalone operation, allowing USB DJ controllers to run independently without a laptop.
- Use a dedicated powered USB hub to prevent brownouts.
- Prefer class-compliant USB audio interfaces.
- Support an optional 7" touchscreen for local UI.
- Provide 3D printed parts for mounting and cable strain relief.

### Software Requirements
- Guarantee deterministic startup and safe fallback behavior when devices are missing.
- Use transparent plain-text configuration files.
- Feature a touchscreen-first UI launcher.
- Run Mixxx with preconfigured profiles and mappings.
- Route master output and headphone cue through ALSA/PipeWire.

## Português

### Geral e Software DJ
- As músicas analisadas pelo Rekordbox devem ser compatíveis.
- O sistema deve ler os cue e memory points.
- O Mixxx deve permitir o modo CDJ e modo Vinyl.

### Requisitos de Hardware
- Usar um Raspberry Pi como unidade central de processamento.
- Garantir operação independente (standalone), permitindo que controladoras DJ USB funcionem sem a necessidade de um laptop.
- Usar um hub USB alimentado dedicado para evitar quedas de energia (brownouts).
- Preferir interfaces de áudio USB class-compliant.
- Suportar uma tela sensível ao toque de 7" opcional para a interface de usuário local.
- Fornecer peças impressas em 3D para montagem e alívio de tensão dos cabos.

### Requisitos de Software
- Garantir inicialização determinística e comportamento de contingência seguro quando os dispositivos estiverem ausentes.
- Usar arquivos de configuração em texto puro (plain-text) e transparentes.
- Apresentar um launcher de interface de usuário otimizado para telas sensíveis ao toque.
- Executar o Mixxx com perfis e mapeamentos pré-configurados.
- Roteamento da saída master e de fones de ouvido (cue) via ALSA/PipeWire.
