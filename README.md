<div align="center">

<img src="https://raw.githubusercontent.com/LucasMauril/Monitor-Solar-App/main/icon.svg" width="100" height="100" alt="Monitor Solar"/>

<h1>🌞 Monitor Solar</h1>

<p><strong>Dashboard em tempo real para painéis solares com Arduino</strong></p>

<a href="https://github.com/LucasMauril/Monitor-Solar-App/releases/latest/download/Monitor.Solar.exe">
  <img src="https://img.shields.io/badge/⬇%20BAIXAR%20AGORA-Monitor%20Solar%20v1.3.0-6c8aff?style=for-the-badge&logoColor=white" alt="Download"/>
</a>

<br/><br/>

<img src="https://img.shields.io/badge/Windows_10%2B-0078D6?style=flat-square&logo=windows&logoColor=white"/>
<img src="https://img.shields.io/badge/versão-1.3.0-34cba4?style=flat-square"/>
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
<td width="60px" align="center">1️⃣</td>
<td><a href="https://github.com/LucasMauril/Monitor-Solar-App/releases/latest/download/Monitor.Solar.exe"><strong>Baixe o Monitor Solar.exe</strong></a> pelo botão acima</td>
</tr>
<tr>
<td align="center">2️⃣</td>
<td>Execute diretamente — <strong>não precisa instalar Python nem nada</strong></td>
</tr>
<tr>
<td align="center">3️⃣</td>
<td>Na primeira abertura, siga o assistente de configuração</td>
</tr>
<tr>
<td align="center">4️⃣</td>
<td>Clique em <strong>Iniciar tour</strong> para conhecer todas as funcionalidades em 31 passos</td>
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

- Gráfico de potência com **gradiente animado** e tooltip interativo
- Barras de estatísticas com **animação de mola** — atualizam suavemente
- **Gauge de eficiência** calculado em tempo real (potência ÷ capacidade máxima)
- Cards de tensão, corrente, consumo e saldo energético
- Temperatura do painel (DS18B20) + ambiente e umidade (DHT22)
- Luminosidade dos LDRs em tempo real
- Exportar **CSV** e **relatório PDF** completo

</details>

<details>
<summary><b>☀️ Tracker Solar 2 eixos</b></summary>
<br/>

- Diagrama SVG animado que segue os dados em tempo real
- **Eixo vertical:** LDR Topo (A3) vs LDR Base (A4) — inclina para cima/baixo
- **Eixo horizontal:** expansível com 3º LDR no Arduino Nano
- Indicador de decisão dos LDRs ao vivo: `→ subindo ↑` / `→ descendo ↓` / `→ estável`
- **Simulação solar pela hora do dia** — funciona sem Arduino!
- Controle manual dos servos via sliders
- Gráfico histórico dos ângulos H e V ao longo do dia

</details>

<details>
<summary><b>💾 Histórico e SD Card</b></summary>
<br/>

- **Aba Ao vivo:** gráfico da sessão atual com pico, média e horário mais eficiente
- **Aba Histórico SD:** importa dados do cartão via comando `SD:READ`
- **Aba Comparativo:** energia com tracker vs sem tracker em %
- Gravação automática no SD Card a cada 1 minuto
- Ganho do tracker calculado pelo Arduino usando os LDRs

</details>

<details>
<summary><b>🔔 Alertas automáticos</b></summary>
<br/>

- Potência mínima — alerta se a geração cair abaixo do esperado
- Potência máxima — alerta se ultrapassar a capacidade
- Tensão mínima — indica sombreamento ou problema no circuito
- **Consumo superando geração** — saldo energético negativo
- Notificações toast em tempo real + histórico dos últimos 20 alertas

</details>

<details>
<summary><b>🎯 Tour guiado — 31 passos em 7 seções</b></summary>
<br/>

O tour entra automaticamente em cada página e destaca os elementos com spotlight:

| Seção | Passos | O que mostra |
|-------|--------|-------------|
| Dashboard | 5 | Gráfico, potência, modo, serial |
| Simulação | 4 | Iniciar, cenários, sliders |
| Histórico | 5 | 3 abas, importar SD |
| Alertas | 3 | Limites, saldo negativo |
| Configurações | 4 | Porta serial, LDR, meta |
| Hardware | 4 | Componentes, diagrama, passo a passo |
| Tracker | 6 | Diagramas, eixos, simular, toggle |

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

## 📋 Novidades da v1.3.0

```
✅ Dashboard redesenhado com gradiente animado e tooltip interativo
✅ Barras de estatísticas com animação de mola — sem piscar
✅ Tour guiado expandido: 31 passos em 7 seções (era 8 passos)
✅ Tracker com indicador de decisão LDR em tempo real
✅ Simulação solar funciona pela hora real do dia
✅ Página de alertas completamente reescrita com explicações
✅ Configurações: novas seções de Tracker e SD Card
✅ Transições suaves entre todas as páginas
✅ Gauge de eficiência real baseado nos dados do painel
```

<details>
<summary>Ver versões anteriores</summary>
<br/>

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
