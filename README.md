# Exercício proposto em sala de aula 
- Matéria: Programção Orientada a Objeto

<h5>Neste exercício, você irá ajudar a criar um MVP para uma fintech que deseja desenvolver um aplicativo de transferência de dinheiro por meio de QR Codes. O objetivo é permitir que os usuários realizem operações básicas, como abrir uma conta bancária, verificar o saldo, fazer depósitos, saques e transferências entre contas, de maneira rápida e simples.

Para tornar o processo de abertura de conta mais fácil para os usuários, é importante que a aplicação seja intuitiva, com telas claras e fáceis de usar. Além disso, o saldo da conta deve ser atualizado em tempo real após cada transação, garantindo assim que os usuários tenham acesso às informações atualizadas.

Para realizar transferências de dinheiro de uma conta para outra, os usuários devem ser capazes de escanear o QR Code gerado pelo destinatário e inserir o valor a ser transferido. É importante lembrar que, de acordo com a lei, a coleta de dados pessoais dos clientes é obrigatória para a abertura de uma conta bancária. Para clientes empresariais, informações sobre a empresa também devem ser coletadas.

Para cada transação bancária, informações como o valor da transação, a data e o tipo de transação (depósito, saque ou transferência) devem ser registradas, assim como as informações das contas envolvidas na transação (número da conta, nome do titular e número de identificação pessoal). Todos esses dados devem ser armazenados de forma segura e em conformidade com as leis e regulamentos aplicáveis, garantindo a privacidade e segurança das informações pessoais dos clientes.

Durante o desenvolvimento da aplicação, é importante considerar possíveis problemas que podem surgir, como a possibilidade de um cliente fornecer informações incorretas ou falsas, ou falhas técnicas que podem levar a perda de dados ou atrasos no processamento das transações. Para minimizar esses problemas, é necessário implementar medidas de segurança e contingência adequadas, como verificações e validações de informações, backups regulares dos dados armazenados e políticas claras e processos bem definidos para lidar com problemas quando eles ocorrem.

Para garantir a satisfação dos clientes, é importante ter uma equipe de suporte disponível para ajudar a resolver quaisquer problemas que possam surgir. E, em caso de violação de dados, um plano de resposta a incidentes deve ser implementado para minimizar os danos e proteger a privacidade dos clientes.

Lembre-se de que ao lidar com informações financeiras sensíveis, é fundamental garantir a segurança dos dados dos clientes e ter planos claros para lidar com quaisquer problemas que possam surgir. Esperamos que este exercício ajude a desenvolver suas habilidades em engenharia de software e a entender a importância da segurança da informação em aplicações financeiras.

Com base no texto anterior listar:<br>
Classes<br>
Atributos<br>
Métodos<br>
Relacionamentos<br>

</h5><br>
<h4>Resposta do exercício:</h4>

- Classes:<br>
> ContaBancaria (double)<br>
Cliente (String)<br>
Transacao (double)<br>
QRCode (String)<br>
EquipeSuporte (String)<br>
PlanoRespostaIncidentes (String)<br>

- Atributos:

> ContaBancaria: número da conta (int), saldo (double)<br>
Cliente: nome (String), sobrenome (String), CPF/CNPJ (String), email (String), telefone (String), endereço (String)<br>
Transacao: valor (double), data (String), tipo de transação (String), número da conta (int), nome do titular (String), número de identificação pessoal (String)<br>
QRCode: informações da conta do destinatário (String) (número da conta, nome do titular)<br>
EquipeSuporte: nome (String), sobrenome (String), email (String), telefone (String)<br>
PlanoRespostaIncidentes: procedimentos e políticas (String) para lidar com violações de dados e outros problemas de segurança<br>

- Métodos:

> ContaBancaria: abrirConta(), verificarSaldo(), fazerDeposito(valor), fazerSaque(valor), fazerTransferencia(valor, contaDestino)<br>
Cliente: fornecerInformacoes(), atualizarInformacoes()<br>
Transacao: registrarTransacao()<br>
QRCode: gerarQRCode()<br>
EquipeSuporte: fornecerSuporte()<br>
PlanoRespostaIncidentes: implementarPlano()<br>


- Relacionamentos:

> Cliente possui uma ContaBancaria<br>
Transacao envolve duas ContasBancarias<br>
QRCode contém informações da ContaBancaria do destinatário<br>
EquipeSuporte é responsável por fornecer suporte ao usuário<br>
PlanoRespostaIncidentes é uma política de segurança implementada pela empresa<br>

