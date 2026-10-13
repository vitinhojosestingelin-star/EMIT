# EMIT — protótipo funcional

Uma aplicação web responsiva e instalável (PWA), inspirada nas referências visuais fornecidas.

## Funcionalidades incluídas
- Início com resumo do dia, tempo de tela, tarefas, hábitos e metas
- Planejamento em visão semanal, mensal e lista
- Criar, editar, concluir e excluir atividades
- Temporizador de foco de 15, 25, 45 ou 60 minutos
- Registro manual de tempo de tela e meta diária
- Hábitos com marcação diária
- Metas com progresso editável
- Reflexões pessoais
- Relatórios iniciais e exportação JSON
- Perfil, configurações e página informativa EMIT+
- Salvamento local no navegador
- Layout responsivo para computador e celular
- Manifest e service worker para instalação como PWA

## Como testar no computador
Abra `index.html` no navegador. Para testar a instalação PWA e o modo offline, sirva a pasta por HTTPS ou localhost.

Exemplo, se tiver Python instalado:
```bash
python -m http.server 8000
```
Depois abra `http://localhost:8000`.

## Como instalar no Android
1. Publique a pasta em um host HTTPS (por exemplo, seu serviço de hospedagem).
2. Abra o endereço no Chrome para Android.
3. Abra o menu do navegador e escolha **Instalar app** ou **Adicionar à tela inicial**.

## Observações importantes
- Esta é uma versão inicial funcional, não um APK nativo.
- Os dados ficam no armazenamento local do navegador e não sincronizam automaticamente entre dispositivos.
- O tempo de tela é inserido manualmente; o navegador não consegue medir ou bloquear o uso geral de outros apps do Android.
- Notificações push, login, banco de dados em nuvem, pagamentos e sincronização exigem backend e configuração adicional.
- O EMIT+ é apenas uma tela demonstrativa; não há cobrança.

## Estrutura
- `index.html` — estrutura da aplicação
- `styles.css` — identidade visual e layout responsivo
- `app.js` — navegação, telas e funcionalidades
- `manifest.json` — configuração de instalação
- `sw.js` — cache offline básico
- `icon.svg` — ícone do app
