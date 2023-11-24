99840 - Carlos Augusto Campos Ganzerli
99403 - Giovanna Saori Arata


## Descrição do Projeto
O SmartWear é um inovador dispositivo de vestuário que integra tecnologia avançada para monitorar a temperatura corporal e os batimentos cardíacos dos usuários. Com o design discreto de anéis, pulseiras ou colares, o SmartWear oferece uma solução elegante e eficiente para o acompanhamento contínuo da saúde.

## Visão Geral da Solução Proposta
O SmartWear utiliza sensores de alta precisão para monitorar a temperatura corporal do usuário em tempo real. Essa funcionalidade é especialmente útil para identificar variações significativas que podem indicar febres ou outros distúrbios térmicos. Os dados de temperatura são registrados e podem ser acessados por meio de um aplicativo dedicado.

### Funcionalidades Principais:
1. **Medição de Batimentos Cardíacos:**
   - Além do monitoramento da temperatura, o SmartWear incorpora tecnologia de monitoramento cardíaco para avaliar os batimentos cardíacos do usuário. Essa funcionalidade permite um acompanhamento preciso da saúde cardiovascular, proporcionando informações valiosas para quem busca manter um estilo de vida ativo e saudável.

2. **Conectividade e Aplicativo:**
   - O SmartWear é facilmente integrado a dispositivos móveis por meio de conectividade Bluetooth. Os usuários podem visualizar os dados coletados em tempo real, históricos de monitoramento e receber alertas personalizados diretamente no aplicativo associado. Isso proporciona uma experiência completa e personalizada para o acompanhamento da saúde.

3. **Design Moderno e Confortável:**
   - Com atenção especial ao design, o SmartWear combina funcionalidade e estilo. Disponível em diferentes formas, como anéis, pulseiras ou colares, o dispositivo é desenvolvido com materiais duráveis e confortáveis para garantir uma experiência agradável ao usuário.

## Instruções de Configuração e Uso:

### Requisitos Prévios:
1. Certifique-se de ter uma instância do Node-RED em execução.
2. Garanta que o MQTT Broker esteja configurado e acessível.

### Configuração do Node-RED:
1. Importe o fluxo fornecido no arquivo `flow.json` para o seu ambiente Node-RED.

2. Conecte o bloco MQTT In ao seu broker MQTT. Certifique-se de configurar o tópico adequado para receber os valores.

3. Configure o bloco Trigger para fornecer a mensagem de boas-vindas ao iniciar o sistema. Ajuste o tempo de duração conforme necessário.

4. Configuração do Telegram:
   - Configure o bloco Telegram Sender com as credenciais do seu bot Telegram.
   - Ajuste o bloco Function 1 para definir as opções do teclado inline.

### Configuração Adicional:
1. Se necessário, ajuste os parâmetros do bloco Function 3 para personalizar a lógica de verificação de lotação, chamada do próximo da fila, etc.

2. Certifique-se de que as bibliotecas e dependências necessárias estejam instaladas no ambiente Node-RED.

### Uso do Bot Telegram:
1. Inicie o bot no Telegram digitando `/start` para receber a mensagem de boas-vindas.

2. Utilize os botões de comando disponíveis para verificar a lotação do hospital, chamar o próximo da fila, verificar a hora atual ou o status do paciente.

### Simulação do Projeto:
Acesse a [simulação do projeto no Wokwi](https://wokwi.com/projects/382041761295119361) para visualizar a interação com o bot e testar as funcionalidades disponíveis.

Essas instruções guiarão você na configuração e uso inicial do sistema de Fila Virtual. Personalize conforme necessário para atender às especificidades do seu ambiente e requisitos.