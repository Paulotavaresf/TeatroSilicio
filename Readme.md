# Sistema de Reserva de Assentos do Teatro do Silício

Bem-vindo ao Sistema de Reserva de Assentos do Teatro do Silício! Este programa permite que você reserve e cancele reservas de assentos no teatro. Abaixo estão as instruções de uso e uma descrição detalhada das funcionalidades do código.

## Funcionalidades

1. **Reservar Assento**
2. **Cancelar Reserva**
3. **Encerrar Atendimento**

## Instruções de Uso

### Executando o Programa

Ao iniciar o programa, você verá o menu principal com três opções:

```
Seja Bem-Vindo, ao Teatro do Silício
<<<<<<<<<<<<>>>>>>>>>>>>
1- Reservar assento.
2- Cancelar Reserva.
3- Encerrar Atendimento.
<<<<<<<<<<<<>>>>>>>>>>>>
Qual seu desejo? 
```

### Reservar Assento

1. Digite `1` para reservar um assento.
2. O programa exibirá a lista de assentos disponíveis e ocupados (`X` representa um assento ocupado).
3. Digite o número do assento que deseja reservar (entre 1 e 5).
4. Se o assento já estiver ocupado, uma mensagem será exibida solicitando que você escolha outro assento.
5. Se o assento estiver disponível, você será solicitado a inserir seu nome e ID para concluir a reserva.
6. Uma mensagem de confirmação será exibida após a conclusão da reserva.

### Cancelar Reserva

1. Digite `2` para cancelar uma reserva.
2. O programa exibirá a lista de assentos disponíveis e ocupados.
3. Digite o número do assento que deseja cancelar.
4. Se o assento não estiver reservado, uma mensagem será exibida informando que o assento não foi reservado.
5. Se o assento estiver reservado, você será solicitado a inserir o nome e ID usados na reserva.
6. Se as informações estiverem corretas, a reserva será cancelada e o assento ficará disponível novamente.
7. Uma mensagem de confirmação será exibida após o cancelamento da reserva.

### Encerrar Atendimento

1. Digite `3` para encerrar o atendimento.
2. O programa exibirá uma mensagem de encerramento e terminará a execução.

### Mensagens de Erro

- Se todos os assentos estiverem ocupados ao tentar reservar, uma mensagem será exibida informando que não há assentos disponíveis.
- Se um assento reservado for solicitado novamente, uma mensagem será exibida informando que o assento já está reservado.
- Se as informações fornecidas ao cancelar uma reserva não coincidirem com as da reserva original, uma mensagem de erro será exibida.
- Se uma opção inválida for escolhida no menu principal, uma mensagem será exibida solicitando que uma opção válida seja digitada.

## Estrutura do Código

O código está estruturado em um loop `while True`, que continua a executar até que a opção de encerrar atendimento seja escolhida. A cada iteração do loop, o programa exibe o menu principal e solicita uma ação do usuário. Dependendo da ação escolhida (reservar, cancelar ou encerrar), o código segue diferentes caminhos para executar a ação desejada.

### Variáveis e Funções

- `cadeira_X` e `caX` representam os assentos e seus estados (True para disponível, False para ocupado).
- `nomeX` e `idX` armazenam o nome e ID dos usuários que reservam os assentos.
- Mensagens de confirmação e erro são exibidas conforme necessário para orientar o usuário durante o uso do programa.

## Contribuições

Se você deseja contribuir com melhorias ou correções para este programa, sinta-se à vontade para abrir um pull request ou relatar problemas.

Esperamos que você tenha uma ótima experiência no Teatro do Silício!