## Reparo do Windows com DISM e SFC

Este guia mostra como reparar arquivos corrompidos do Windows utilizando as ferramentas DISM e SFC pelo Prompt de Comando.

### Passo 1: Abrir o Prompt de Comando como Administrador

1. Clique no menu Iniciar, digite `cmd`.
2. Clique com o botão direito em **Prompt de Comando** e selecione **Executar como administrador**.

### Passo 2: Executar o DISM

Digite o comando abaixo e pressione Enter:

```sh
DISM /Online /Cleanup-Image /RestoreHealth
```

Espere o processo terminar. Pode demorar alguns minutos.

### Passo 3: Executar o SFC

Após o DISM, digite o comando abaixo e pressione Enter:

```sh
sfc /scannow
```

O SFC irá verificar e reparar arquivos corrompidos do sistema.

### Observações

- Reinicie o computador após a conclusão dos comandos.
- Se persistirem erros, repita os comandos ou busque suporte especializado.
