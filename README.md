# FlexHackathon2020

Projeto em RPA realizado pelo time Uchiha para apresentação no Flex Hackathon 2020.
<br>
O projeto em questão tem como objetivo automatizar o processo manual de extração dos participantes incritos no evento do Sympla e enviar um invite no outlook para a live.
<br>
Assim, o robô acessa a plataforma Sympla com as credenciais do criador do evento, extrai todos os participantes inscritos, distingue os participantes aprovados dos cancelados e envia para os aprovados o convite para o evento.

## Iniciando

Estas instruções fornecerão uma cópia do projeto instalado e funcionando em sua máquina local para fins de desenvolvimento e teste. 

### Pré-requisitos

Softwares/Contas necessárias:

```
UiPath Studio
UiPath Web Automation (Extensão web)
Excel
Sympla Account (necessidade de ter evento criado)
```

### Definição de Variáveis

Para que o robô funcione corretamente, é preciso alterar algumas variáveis, visto que de acordo com o usuário/máquina as informações podem ser divergentes.
* **strEmail - Workflow LoginSympla:** Email usado para logar no Sympla.
* **strPassword - Workflow LoginSympla:** Senha usada para logar no Sympla.
* **strCurso - Workflow GetData:** Nome do evento cadastrado no Sympla.
* **strDoc - Workflow GetData:** Pasta onde o arquivo extraído do Sympla será salvo.

## Possíveis melhorias

* UiPath Form para pegar informação de email/senha/curso do usuário para que não haja necessidade de altração no código.
* Criar um padrão para preenchimento do corpo do email.
* Afim de confirmar a presença do usuário no evento, programar o robô para o envio de emails questionando a presença do participante, evintando o envio manual.

## Feito com

* [UiPath Studio] (https://www.uipath.com/developers/studio-download)

## Autores

* **Andreina Oliveira** - *Programação do Robô* - [GitHub](https://github.com/andreinaoliveira)
