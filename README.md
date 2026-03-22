<div align="center">

<img src="https://raw.githubusercontent.com/LucasMauril/Monitor-Solar-App/main/icon.svg" width="100" height="100" alt="Monitor Solar"/>

<h1>Monitor Solar</h1>

<p><strong>Dashboard em tempo real para painéis solares com Arduino</strong></p>

<a href="https://github.com/LucasMauril/Monitor-Solar-App/releases/latest/download/Monitor.Solar.exe">
  <img src="https://img.shields.io/badge/⬇%20BAIXAR%20AGORA-Monitor%20Solar%20v1.6.0-6c8aff?style=for-the-badge&logoColor=white" alt="Download"/>
</a>

<br/><br/>

<img src="https://img.shields.io/badge/Windows_10%2B-0078D6?style=flat-square&logo=windows&logoColor=white"/>
<img src="https://img.shields.io/badge/versão-1.6.0-34cba4?style=flat-square"/>
<img src="https://img.shields.io/badge/gratuito-sim-f5a623?style=flat-square"/>
<img src="https://img.shields.io/badge/Arduino-compatível-00979D?style=flat-square&logo=arduino&logoColor=white"/>
<img src="https://img.shields.io/badge/sem_instalação-✓-6c8aff?style=flat-square"/>

<br/><br/>

> Monitore tensão, corrente, temperatura e geração solar em tempo real.<br/>
> Funciona com Arduino **ou** no Modo Simulação — **sem nenhum hardware.**

</div>

---

## 📥 Download e instalação

<table>
<tr>
<td width="60px" align="center">1</td>
<td><a href="https://github.com/LucasMauril/Monitor-Solar-App/releases/latest/download/Monitor.Solar.exe"><strong>Baixe o Monitor Solar.exe</strong></a> pelo botão acima</td>
</tr>
<tr>
<td align="center">2</td>
<td>Execute diretamente — <strong>não precisa instalar Python nem nada</strong></td>
</tr>
<tr>
<td align="center">3</td>
<td>Na primeira abertura, siga o assistente de configuração</td>
</tr>
<tr>
<td align="center">4</td>
<td>Clique em <strong>Iniciar tour</strong> para conhecer todas as funcionalidades em <strong>38 passos</strong></td>
</tr>
</table>

<details>
<summary>⚠️ Windows Defender alertou? Clique aqui</summary>
<br/>

Isso é um **falso positivo** comum em apps feitos com PyInstaller (Python empacotado). O código não contém vírus ou malware.

**Para continuar:**
1. Clique em **"Mais informações"**
2. Clique em **"Executar assim mesmo"**

Ou adicione uma exclusão no Windows Defender para a pasta onde o `.exe` está.

</details>

---

## 🚀 Funcionalidades

<details>
<summary><b>📊 Dashboard ao vivo</b></summary>
<br/>

- Gráfico de potência com gradiente animado e tooltip interativo
- **Sparklines** nos cards de tensão, corrente, potência e consumo
- **Gauge de eficiência** com 3 zonas coloridas (Baixa / Moderada / Boa)
- **Contador de leituras e taxa Hz** no rodapé do gráfico
- **Uptime da sessão** — cronômetro em tempo real no topbar
- **Previsão de geração do dia** baseada na taxa atual de geração
- **Notificação de meta atingida** com animação shimmer na barra de progresso
- Card de Saldo que **pulsa em vermelho** quando o consumo supera a geração
- Temperatura do painel (DS18B20) com alerta de cor acima de 55°C/70°C
- ECONOMIA HOJE em R$ com CO₂ evitado e projeção mensal
- Exportar **CSV** e **relatório PDF** completo

</details>

<details>
<summary><b>☀️ Tracker Solar 2 eixos — Servo MG996R</b></summary>
<br/>

- Servo **MG996R** (11kg/cm) para painéis maiores e mais pesados
- Diagrama SVG animado que segue os dados em tempo real
- **Modo noturno automático** 🌙 — servos vão para posição de repouso ao anoitecer
- Intervalo configurável: 1min / 5min / **15min** / 30min / 1h
- **Gráfico histórico do ganho** — últimas 12h de eficiência
- **Exportar CSV de ângulos H/V** — histórico completo de posição dos servos
- Simulação solar pela hora real do dia — sem Arduino!
- Controle manual dos servos via sliders

</details>

<details>
<summary><b>💾 Histórico e SD Card</b></summary>
<br/>

- **Aba Ao vivo:** gráfico da sessão com pico, média e horário mais eficiente
- **Aba Histórico SD:** importa dados do cartão via `SD:READ`
- **Aba Comparativo:** energia com tracker vs sem tracker em %
- Gravação automática no SD Card a cada 1 minuto
- Ganho do tracker calculado pelo Arduino com os LDRs

</details>

<details>
<summary><b>🔧 Calibração dos sensores pelo app</b></summary>
<br/>

- Sliders para ajustar **Zero da corrente** dos ACS712 sem recompilar o Arduino
- Ajuste do **fator do divisor de tensão** em tempo real
- Envio via Serial com confirmação — valores persistem entre sessões

</details>

<details>
<summary><b>🖥️ Modo Apresentação</b></summary>
<br/>

- Atalho **F5** ou botão na barra lateral
- **Tela cheia automática** ao entrar — cobre a barra de tarefas
- Sidebar some, **KPIs gigantes com animação** — valores pulsam a cada leitura
- Gráfico com **gradiente animado** e tooltip estilizado
- **Botão PDF direto na barra** — salva o relatório sem sair da tela cheia
- **Auto-rotação** entre abas: Dashboard → Tracker → Histórico
- **QR Code do GitHub** para os espectadores escanearem
- Barra superior com relógio, status e badge v1.6
- **ESC** para sair e restaurar a janela

</details>

<details>
<summary><b>♿ Acessibilidade — Modo Daltônico</b></summary>
<br/>

- Atalho **Ctrl+D** ou toggle na aba Sobre
- Troca toda a paleta para cores **safe para deuteranopia e protanopia**
- Linhas dos gráficos ganham **padrões tracejados e pontilhados** para distinção sem depender de cor
- Cobre: cards, gauge, sparklines, alertas, notificações e todos os 7 gráficos
- Configuração salva entre sessões

</details>

<details>
<summary><b>⌨️ Atalhos de teclado</b></summary>
<br/>

| Tecla | Ação |
|-------|------|
| F1 | Dashboard |
| F2 | Simulação |
| F3 | Histórico |
| F4 | Tracker |
| F5 | Modo Apresentação |
| F6 | Alertas |
| F7 | Configurações |
| F8 | Hardware |
| F9 | Montagem |
| F10 | Sobre |
| Ctrl+P | Exportar PDF |
| Ctrl+D | Modo daltônico |
| ESC | Sair/Fechar tour |

</details>

<details>
<summary><b>🔔 Notificações e sons</b></summary>
<br/>

- **Som ao conectar Arduino** — bip duplo de confirmação
- **Alerta de bateria baixa** — bip de aviso (configurável)
- Sons nas notificações do dashboard via Web Audio API
- Toggle de sons nas Configurações

</details>

<details>
<summary><b>🎯 Tour guiado — 38 passos</b></summary>
<br/>

Cobre todas as funcionalidades do app em **9 seções**: Dashboard, Simulação, Histórico, Alertas, Configurações, Hardware, Montagem, Tracker e Sobre. Totalmente atualizado para a v1.6.

</details>

---

## 🔧 Requisitos

| | |
|--|--|
| **Sistema** | Windows 10 ou superior (64 bits) |
| **Hardware** | Opcional — Arduino Uno/Nano com sensores |
| **Sem Arduino** | Use o Modo Simulação normalmente |
| **Instalação** | Nenhuma — basta executar o `.exe` |

---

## 📋 Novidades da v1.6.0

```
✅ Uptime da sessão — cronômetro em tempo real no topbar
✅ Contador de leituras e taxa Hz no rodapé do gráfico de potência
✅ Previsão de geração do dia baseada na taxa atual
✅ Notificação de meta de energia atingida com animação especial
✅ Botão PDF no Modo Apresentação — sem sair da tela cheia
✅ Gráfico do Modo Apresentação com gradiente, animações e tooltip
✅ Animação nos KPI cards — valores pulsam a cada leitura
✅ Exportar histórico de ângulos H/V do tracker (CSV)
✅ Modo Daltônico completo — paleta safe + padrões de linha nos gráficos
✅ Atalho Ctrl+D para modo daltônico
✅ Aba "Sobre" com F10, GitHub links (releases + reportar problemas)
✅ Serial monitor com altura fixa — layout nunca quebra
✅ Botão Limpar no serial monitor
✅ Limite de linhas configurável no serial (20–500)
✅ Reconexão WebSocket com contador regressivo visual
✅ Fechamento correto — processo não fica zumbi no gerenciador
✅ Tour guiado atualizado — 38 passos em 9 seções
```

<details>
<summary>Ver versões anteriores</summary>
<br/>

**v1.5.0**
- Modo noturno do tracker, alerta de bateria baixa
- Reconexão automática ao Arduino, Modo Apresentação com QR Code
- Sons de notificação, atalhos F1–F8

**v1.4.0**
- Servo MG996R, calibração ACS712 pelo app
- Sparklines, badge ganho tracker, saldo pulsa vermelho

**v1.3.0**
- Dashboard redesenhado, tour 31 passos

**v1.2.0**
- Seguidor solar 2 eixos, histórico SD Card, relatório PDF

**v1.1.0**
- Tour guiado, modo claro/escuro, notificações toast

</details>

---

<div align="center">

**Feito com ☀️ por Lucas Mauril**

[![GitHub](https://img.shields.io/badge/GitHub-LucasMauril-181717?style=flat-square&logo=github)](https://github.com/LucasMauril)
[![X](https://img.shields.io/badge/X-lukinnhas-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/lukinnhas)
[![Discord](https://img.shields.io/badge/Discord-lukinnhass-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.com/users/lukinnhass)

<sub>⭐ Se o projeto te ajudou, deixa uma estrela!</sub>

</div>
