<div align="center">

<img src="https://raw.githubusercontent.com/LucasMauril/Monitor-Solar-App/main/icon.svg" width="100" height="100" alt="Monitor Solar"/>

<h1>Monitor Solar</h1>

<p><strong>Dashboard em tempo real para painéis solares com Arduino</strong></p>

<a href="https://github.com/LucasMauril/Monitor-Solar-App/releases/latest/download/Monitor.Solar.exe">
  <img src="https://img.shields.io/badge/⬇%20BAIXAR%20AGORA-Monitor%20Solar%20v1.4.0-6c8aff?style=for-the-badge&logoColor=white" alt="Download"/>
</a>

<br/><br/>

<img src="https://img.shields.io/badge/Windows_10%2B-0078D6?style=flat-square&logo=windows&logoColor=white"/>
<img src="https://img.shields.io/badge/versão-1.4.0-34cba4?style=flat-square"/>
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
<td>Clique em <strong>Iniciar tour</strong> para conhecer todas as funcionalidades em 33 passos</td>
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
- **Gauge de eficiência** com zona verde e temperatura do painel integrada
- Badge de **ganho do tracker** em tempo real (+X%)
- Card de Saldo que **pulsa em vermelho** quando o consumo supera a geração
- Temperatura do painel (DS18B20) com alerta de cor acima de 55°C/70°C
- Animações de entrada suaves nos cards ao trocar de aba
- Exportar **CSV** e **relatório PDF** completo

</details>

<details>
<summary><b>☀️ Tracker Solar 2 eixos — Servo MG996R</b></summary>
<br/>

- Servo **MG996R** (11kg/cm) para painéis maiores e mais pesados
- Diagrama SVG animado que segue os dados em tempo real
- **Eixo vertical:** LDR Topo (A3) vs LDR Base (A4)
- **Eixo horizontal:** expansível com 3º LDR no Arduino Nano
- **Simulação solar pela hora real do dia** — sem Arduino!
- Controle manual dos servos via sliders
- Gráfico histórico dos ângulos H e V

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
- Sidebar some, KPIs gigantes (48px) centralizados
- 4 cards: Potência, Tensão, Saldo e Temperatura
- Gráfico grande de potência ao vivo
- Barra superior com relógio, status e badge v1.4
- **ESC** para sair

</details>

<details>
<summary><b>🔬 Simulador Wokwi integrado</b></summary>
<br/>

- Botão na aba Hardware abre o Wokwi automaticamente
- **diagram.json copiado para o clipboard** ao clicar
- Circuito completo: Arduino Uno + ACS712 ×2 + LDR ×2 + DHT22 + Servo ×2
- Modal com passo a passo para carregar o diagrama

</details>

<details>
<summary><b>🎯 Tour guiado — 33 passos em 7 seções</b></summary>
<br/>

| Seção | Passos | O que mostra |
|-------|--------|-------------|
| Dashboard | 7 | Gráfico, sparklines, saldo, temperatura, Modo Apresentação |
| Simulação | 4 | Iniciar, cenários com temperatura/umidade, sliders |
| Histórico | 5 | 3 abas, importar SD, comparativo tracker |
| Alertas | 3 | Limites, cooldown 30s, saldo negativo |
| Configurações | 5 | Porta serial, LDR, calibração ACS712, fator tensão |
| Hardware | 3 | Wokwi, componentes v1.4, diagrama |
| Tracker | 5 | Diagramas, simulação solar, controle manual |

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

## 📋 Novidades da v1.4.0

```
✅ Servo MG996R (11kg/cm) para painéis maiores
✅ Calibração dos sensores ACS712 pelo app — sem recompilar
✅ Sparklines nos cards de tensão, corrente, potência e consumo
✅ Badge de ganho do tracker no card de potência
✅ Card de saldo pulsa em vermelho quando negativo
✅ Temperatura integrada no gauge de eficiência
✅ Modo Apresentação com KPIs gigantes e gráfico ao vivo
✅ Botão Wokwi com animação e cópia automática do diagram.json
✅ Tour atualizado para 33 passos com todas as novidades
✅ Simulação completa: temperatura, umidade, LDRs e tracker por hora
✅ Proteção IP65 e bateria 18650 documentadas na aba Hardware
✅ Alertas movidos para canto inferior direito, máx 3 visíveis
✅ Cooldown de 30s entre alertas do mesmo tipo
✅ Design das telas de verificação completamente renovado
```

<details>
<summary>Ver versões anteriores</summary>
<br/>

**v1.3.0**
- Dashboard redesenhado com gradiente animado e tooltip interativo
- Tour guiado expandido: 31 passos em 7 seções
- Tracker com indicador de decisão LDR em tempo real
- Simulação solar funciona pela hora real do dia

**v1.2.0**
- Seguidor solar 2 eixos com diagrama SVG animado
- Histórico offline via SD Card com 3 abas
- Relatório PDF completo
- Comparativo de eficiência com/sem tracker

**v1.1.0**
- Tour guiado interativo
- Modo claro/escuro
- Notificações toast
- Alertas automáticos de limites

</details>

---

<div align="center">

**Feito com ☀️ por Lucas Mauril**

[![GitHub](https://img.shields.io/badge/GitHub-LucasMauril-181717?style=flat-square&logo=github)](https://github.com/LucasMauril)
[![X](https://img.shields.io/badge/X-lukinnhas-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/lukinnhas)
[![Discord](https://img.shields.io/badge/Discord-lukinnhass-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.com/users/lukinnhass)

<sub>⭐ Se o projeto te ajudou, deixa uma estrela!</sub>

</div>
