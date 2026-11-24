# [Título Técnico do Diagnóstico ou Reparo]

- **Autor(a):** Matheus Santana
- **Categoria:** Sistema Operacional / Armazenamento

> **Alerta de Segurança:** Realize um backup prévio dos arquivos críticos antes de executar parâmetros de reparo (/f ou /r), pois a realocação de clusters corrompidos pode resultar em perda pontual de dados fragmentados. Nunca interrompa a alimentação elétrica do equipamento durante a execução do utilitário, sob risco de corromper gravemente a tabela de partições.

## 1. Sintoma e Diagnóstico Inicial

O sistema apresenta lentidão extrema ao acessar diretórios, falhas ao abrir ou salvar arquivos específicos, mensagens de erro como "O arquivo ou pasta está corrompido e ilegível" ou telas azuis (BSOD) relacionadas a NTFS_FILE_SYSTEM. A causa mais provável é a corrupção lógica na tabela de alocação de arquivos (MFT), desligamentos abruptos ou a presença de setores defeituosos (bad blocks) na unidade de armazenamento.

## 2. Ferramentas e Recursos Necessários

- **Hardware / Bancada:** Não se aplica (procedimento lógico)
- **Software / Utilitário:** Prompt de Comando (CMD) ou Windows Terminal executado com privilégios de Administrador, e utilitário nativo

## 3. Procedimento de Solução (Passo a Passo)

1. Clique no menu **Iniciar**, digite cmd, clique com o botão direito sobre **Prompt de Comando** e selecione **Executar como administrador**.
2. Execute primeiramente uma varredura em modo somente leitura na unidade desejada (ex.: C:) para identificar erros sem alterar o disco:

    ```bash
    chkdsk C:
    ```

3. Caso o relatório aponte erros no sistema de arquivos, execute o comando de correção lógica e recuperação de setores físicos (substitua C: pela letra da unidade alvo, se necessário):

    ```bash
    chkdsk C: /f /r
    ````

4. Se a unidade estiver em uso pelo sistema operacional, o terminal exibirá a mensagem "Não é possível executar o Chkdsk porque o volume está em uso por outro processo". Digite **S** e pressione Enter para agendar a verificação na próxima inicialização.]

5. Reinicie o computador e aguarde a conclusão automática das etapas de verificação antes de o Windows carregar a tela de login.

## 4. Checklist de Validação (Teste Final)

- [x] O utilitário concluiu todas as etapas sem travamentos e exibiu a mensagem "O Windows verificou o sistema de arquivos e não encontrou problemas" (ou confirmou que as correções foram aplicadas).
- [x] Os diretórios e arquivos que apresentavam erro de leitura abrem normalmente sem alertas do sistema
- [x] O Visualizador de Eventos do Windows (em Logs do Windows > Aplicativo, fonte Wininit ou Chkdsk) registra a conclusão limpa sem novos erros críticos de disco.