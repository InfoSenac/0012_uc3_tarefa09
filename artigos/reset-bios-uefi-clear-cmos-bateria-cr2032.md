
# Diagnóstico e Reparo de BIOS/UEFI: Clear CMOS e Troca da Bateria CR2032

- **Autor(a):** Rone Max Fonseca e Brites
- **Categoria:** Hardware / BIOS-UEFI

> **Alerta de Segurança:** Antes de iniciar o procedimento, desligue o computador, desconecte o cabo de energia da tomada e aguarde alguns minutos. Utilize proteção contra descarga eletrostática (ESD). Consulte o manual do fabricante antes de remover a bateria ou utilizar o jumper Clear CMOS. Em notebooks, verifique as orientações específicas de desmontagem.

## 1. Sintoma e Diagnóstico Inicial

Quando a bateria CMOS está descarregada, o computador pode perder a data, a hora e algumas configurações da BIOS/UEFI após ser desligado da tomada. Também podem aparecer mensagens como "CMOS Checksum Error" durante a inicialização.

## 2. Ferramentas e Recursos Necessários

- **Hardware / Bancada:** Chave Philips, pulseira antiestática (ESD) e bateria CR2032 nova e compatível com a placa-mãe.
- **Software / Utilitário:** BIOS/UEFI do computador e manual técnico da placa-mãe ou do fabricante.

## 3. Procedimento de Solução (Passo a Passo)

1. Desligue o computador, desconecte o cabo de energia e consulte o manual da placa-mãe para localizar a bateria CMOS e o jumper Clear CMOS. Identifique os sintomas e verifique se a data e a hora estão sendo perdidas.

2. Para restaurar as configurações, execute o procedimento Clear CMOS conforme as orientações do fabricante. Se for necessário substituir a bateria, retire a CR2032 antiga cuidadosamente e instale uma nova compatível, respeitando a polaridade indicada no suporte.

3. Ligue o computador, acesse a BIOS/UEFI, configure novamente a data, a hora e a ordem de inicialização. Salve as alterações e inicie o sistema operacional para verificar se o equipamento voltou a funcionar normalmente.

## 4. Checklist de Validação (Teste Final)

- [ ] A data e a hora permanecem corretas após desligar e ligar novamente o computador.
- [ ] O computador inicia normalmente, reconhece o dispositivo de armazenamento e mantém as configurações da BIOS/UEFI.
