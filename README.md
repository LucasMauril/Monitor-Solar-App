## 🌞 Monitor Solar v1.3.0

Dashboard em tempo real para painéis solares com Arduino — completamente redesenhado.

---

### 📥 Como instalar
1. Baixe o **Monitor.Solar.exe** abaixo
2. Execute diretamente — **não precisa instalar nada**
3. Na primeira abertura, siga o assistente de configuração
4. Use o **tour guiado** para conhecer todas as funcionalidades

> ⚠️ O Windows Defender pode alertar sobre o arquivo. Clique em **"Mais informações" → "Executar assim mesmo"**. É um falso positivo comum em apps feitos com PyInstaller.

---

### ✨ Novidades desta versão

**🎨 Dashboard redesenhado**
- Gráfico com gradiente animado sob a linha de potência e tooltip interativo
- Barras de estatísticas com animação de mola — sem mais "piscar" a cada atualização
- Escala do gráfico dinâmica: ajusta automaticamente com base nos dados reais
- Gauge de eficiência real (potência atual ÷ capacidade máxima configurada)
- Card de saldo com borda colorida: verde quando gerando mais, vermelho quando consumindo mais

**☀️ Tracker Solar melhorado**
- Indicador de decisão dos LDRs ao vivo: `→ subindo ↑`, `→ descendo ↓` ou `→ estável`
- Diferença Topo−Base em tempo real com explicação visual
- Aviso explicativo no topo da página com resumo de como o tracker funciona
- Ponto de status animado: "Tracker ativo", "Desligado" ou "Simulação solar ativa"

**🎯 Tour guiado expandido: 31 passos em 7 seções**
O tour agora entra automaticamente em cada página e destaca os elementos importantes:
Dashboard → Simulação → Histórico → Alertas → Configurações → Hardware → Tracker

**🔔 Página de Alertas reescrita**
- 4 cards explicativos sobre como o sistema funciona
- Contador de alertas em tempo real no topo
- Cada limite com descrição do que ele detecta
- Alerta de saldo negativo em destaque

**⚙️ Configurações expandidas**
- Nova seção: Seguidor Solar (tolerância LDR, passo do servo, liga automático)
- Nova seção: Histórico e SD Card (intervalo de gravação, importação automática)

**🌐 Transições entre páginas**
- Efeito suave de entrada com `opacity` + `translateY` em 220ms
- Páginas inativas completamente ocultas — sem conteúdo "vazando"

**🧹 Projeto limpo**
- Removidos arquivos desnecessários (`bridge.py`, `decode.py`, `compilar.bat` hardcoded, etc.)
- `compilar.bat` recriado sem caminho fixo — funciona em qualquer PC
- Zero erros de lint no VS Code

---

### 🔧 Requisitos
- Windows 10 ou superior (64 bits)
- Opcional: Arduino Uno/Nano com sensores para dados reais
- Sem Arduino: use o **Modo Simulação** normalmente
