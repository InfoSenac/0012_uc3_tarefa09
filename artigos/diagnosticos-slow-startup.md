# Diagnóstico de inicialização em máquinas

- **Autor(a):** Felipe Alves Soares
- **Categoria:** Inicialização lenta ou Startup com problemas.

> **Alerta de Segurança:** É sempre bom se assegurar de ter a certeza sobre as máquinas terem um bom anti-vírus e uma boa quantia de espaço livre nos discos rígidos.

## 1. Sintoma e Diagnóstico Inicial

Na maioria das vezes a inicialização pode vir a ser lenta ou acabando à ter lags no meio do uso da máquina graças ao excesso de aplicativos já abertos junto da inicialização da máquina, o que pode ser mudado pelo gerenciador de tarefas na quarta opção da esquerda com o nome de "Aplicativos de Inicialização", essa parte será responsável por informar o usuário do computador quais aplicativos estão inicializando junto com o dispositivo, alguns como Discord e Spotify que já ficam de primeiro plano o que consome ainda mais memória ou como a Steam que já inicializa em segundo plano para acelerar a facilidade e agilidade do dono à acessar o aplicativo, mas caso tenha muitos aplicativos na inicialização seria essencial a atenção e organização.

## 2. Ferramentas e Recursos Necessários

- **Hardware / Bancada:** SSD (Armazenamento), Memória RAM e Processador CPU
- **Software / Utilitário:** Gerenciador de tarefas para a verificação dos aplicativos de inicialização, Configurações do sistema e Limpeza de discos.

## 3. Procedimento de Solução (Passo a Passo)

1. Primeiro passo: Fazer um teste de como está a inicialização e startup das máquinas reiniciando-as de forma segura e prática, assim verificando se a inicialização continua lenta ou não;

2. Segundo passo: Verificar o gerenciador de tarefas e organizar os aplicativos de inicialização, assim fornecendo um início mais rápido à máquina já que ela não terá que se preocupar com vários aplicativos abrindo ao mesmo tempo;

    ```bash
    # Ctrl + Shift + ESC Pode ser utilizado para acessar o Gerenciador de tarefas.
    ```

3. Terceiro passo: Verificar o espaço do disco rígido pelo Windows Explorer e acessando o "Meu Computador";
    ```bash
    # Windows Explorer pode ser acessado utilizando Windows+E.
    ```

4.  Quarto passo: Verificar as atualizações pesadas de inicialização da máquina pelas Configurações do Sistema, Serviços, Ocultar todos os serviços da Microsoft e desmarque atualizadores pesados, como Steam, Adobe, Etc...
    ```bash
    # Windows+R abre uma aba de pesquisa, digitar msconfig abrirá as configurações do sistema.
    ```

5. Quinto passo: Verifique se a máquina tem um anti-vírus confiável ou ativo, como anti-malware e instale, sempre fazendo uma análise antes e depois do download de algum arquivo

## 4. Checklist de Validação (Teste Final)

- Faça uma reinicialização da máquina e teste se o início continua lento, sempre verificando com o gerenciador de tarefas se os aplicativos continuam em segundo plano.