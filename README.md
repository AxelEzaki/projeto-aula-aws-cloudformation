# projeto-aula-aws-cloudformation
Criação de uma Stack com CloudFormation

## Etapas para Criação
1 - Entrar na conta AWS como um administrador (não como root);
2 - Pesquisar por "CloudFormation" na barra de pesquisa presente no Console;
3 - Entrando na página de CloudFormation, clicar em "Criar pilha"
4 - Selecionado o "Escolher um modelo existente" e, na parte de "Especificar modelo", selecionar "Fazer upload de um arquivo de modelo";
5 - Fazer upload do arquivo .yaml, no caso, selecionei o arquivo 01-EC2.yaml presente na aula e cliquei em botão Próximo;
6 - Digitei um nome para a stack;
7 - Concluir a criação de stack;

## Estudos

### CloudWatch
Responsável por monitorar os recursos da conta na AWS, toda a aplicação é monitorada em tempo real, coletando e monitorando métricas.
Monitorar os eventos que estão acontecendo dentro dos recursos.
As métricas auxiliam na medição do serviço, quanto tempo demora para ocorrer e como melhorá-lo, se são os recursos ou a aplicação.
Conseguimos também habilitar alertas sobre as métricas, atingindo um determinado nível de processamento, uso de CPU, por exemplo. Pode automatizar também para alterar os recursos que está sendo monitorado quando um limite é violado.

### CloudTrail
Ajuda na auditoria operacional e de risco, a governança e a conformidade com a conta AWS.
Toda ação realizada por um usuário, função ou serviço serão registradas como eventos no CloudTrail.
Registra o caminho, quem acessou determinado recurso, quais alterações foram feitas, data e hora.
Dá para mandar para o CloudWatch com um alarme, notificando o usuário da conta.
Se excluir um bucket da qual o CloudTrail está configurado, será excluído todos os logs até outro ser configurado.

### CloudFormation
Automação de criação de recursos por meio de templates JSON ou YAML.
Paga apenas as stacks criadas.
