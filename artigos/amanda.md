# Dagnóstico de Superaquecimento e Throttling

- **Autor(a):** Amanda
- **Categoria:** Hardware

> **Alerta de Segurança:** Desligue o computador da tomada, espere e use pulseira ESD antes de abrir. Nunca abra a fonte e nunca use aspirador para limpar o interior.

## 1. Sintoma e Diagnóstico Inicial

O computador fica lento do nada, trava em jogos ou programas pesados, desliga sozinho e o cooler faz muito barulho. Isso acontece porque quando a temperatura sobe demais, o processador diminui a velocidade sozinho para não queimar. Isso se chama thorottling.

## 2. Ferramentas e Recursos Necessários

- **Hardware / Bancada:** Chave Phillips, pincel macio, ar comprimido, pasta térmica nova, pulseira ESD, álcool isopropílico
- **Software / Utilitário:** HWMonitor, HWiNFO, Gerenciador de tarefas

## 3. Procedimento de Solução (Passo a Passo)

1. Abra o HWMonitor ou o HWiNFO e anote a temperatura da CPUem repouso e depois com algum programa pesado aberto.
2. Abra o Gerenciador de Tarefas com Ctrl + Shift + Esc e veja se a velocidade da CPU cai quando a temperatura sobe. Se cair, é thottling.
3. Desligue o computador, tire da tomada e espere 10 minutos para esfriar.
4. Abra o gabinete e limpe o pó dos coolers, do dissipador e das saídas de ar com pincel macio e ar comprimido, em um lugar ventilado.
5. Se continuar quante, tire o cooler do processador, limpe a pasta térmica velha com álcool isopropílico e coloque uma gotinha de pasta nova no centro do processador.
6. Remote o cooler, ligue o computador e deixe monitorando po 15 minutos.

    ```bash
   vwic /namespace:\\root\wmi PATH MSAcpi_ThermalZoneTemperature get CurrentTemperature
    ```


## 4. Checklist de Validação (Teste Final)

- [ ] Temperatura da CPU abaixo de 85°C em uso pesado por 15 minutos
- [ ] Computador não trava, não desliga sozinho e mantém o desempenho
- [ ] Cooler girando normal e sem barulho estranho