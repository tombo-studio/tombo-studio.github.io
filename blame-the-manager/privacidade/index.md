# Política de privacidade do Blame the Manager

Versão: 2026-09-29

Read in English: https://tombo-studio.github.io/blame-the-manager/privacy/

O Blame the Manager só envia alguma coisa para fora do seu computador se você
aceitar. Esta página diz o que sai, o que fica, para onde vai e como mudar de
ideia.

O envio tem duas finalidades: achar e consertar travamentos e defeitos, e medir
onde as pessoas se perdem no jogo para melhorá-lo.

## 1. Quem é o responsável pelos dados?

A JMC Tecnologia da Informação Ltda., CNPJ 54.004.699/0001-97, com sede no
Brasil, que opera o label Tombo Studio e publica o jogo. Ela é a controladora
dos dados para a LGPD (Lei 13.709/2018) e para o GDPR. Contato:
juliano@jmcoimbra.eng.br.

## 2. O que o jogo envia, e o que ele deixa de fora?

Nada sai sem o seu consentimento. O registro completo de cada sessão fica
sempre no seu computador, na pasta de logs do jogo, com ou sem consentimento.

Se você aceitar, sai o seguinte:

| Sai | Fica fora do registro enviado |
|---|---|
| Um identificador de sessão de 8 caracteres, sorteado de novo a cada sessão (cada abertura do jogo e cada carreira começada ou carregada), e um número aleatório da mesma sessão que só separa, no armazenamento, duas sessões com o mesmo identificador; com eles, a versão do jogo, a semente do mundo, o sistema operacional, o idioma e a origem da sessão | Seu nome, seu e-mail e sua conta Steam ou itch.io |
| Os eventos da sessão: telas abertas, decisões tomadas, resultados das partidas | Os nomes que você digita para o presidente, o clube ou a carreira, e os nomes de jogadores, técnicos e comissão, inclusive os de um pacote de nomes que você importou: o jogo os apaga do registro da sessão antes de enviar |
| A mensagem e a pilha de um erro, com o caminho das pastas do seu computador apagado | O caminho das pastas, o nome da máquina e o seu nome de usuário no sistema |
| Uma linha por sessão com a versão do sistema, a placa de vídeo e o fabricante dela, a resolução, a escala de tela e o renderizador | Qualquer identificador de instalação, de conta ou de pessoa |
| Num travamento, o relatório técnico do instante da falha (minidump), com o sistema e o dispositivo | O minidump é a exceção desta coluna: ele copia trechos da memória do jogo naquele instante e pode carregar qualquer texto que estava nela, inclusive um nome que você digitou ou um caminho de pasta |

O identificador muda a cada sessão. A semente do mundo vai em toda
linha porque é ela que reproduz um defeito, e ela é a mesma em todas as sessões
de uma carreira: por isso as sessões de uma mesma carreira se ligam entre si.
A linha do dispositivo também se repete entre as sessões de um mesmo
computador. Nada disso diz quem você é, e não usamos os dados para tentar
descobrir quem jogou.

Como em qualquer conexão com a internet, o seu endereço IP chega aos
fornecedores abaixo para que o envio aconteça. Nós não o guardamos (seção 3).

## 3. Para onde vai?

- **Relatórios de travamento:** Sentry, na região da União Europeia
  (Frankfurt, Alemanha). O jogo não põe o seu endereço IP no relatório, e o
  projeto está configurado para não guardar o endereço da conexão.
- **Registro das sessões:** Cloudflare, num armazenamento R2 próprio do jogo,
  criado na jurisdição da União Europeia: os registros ficam guardados em
  data centers dentro da União Europeia. O servidor que recebe o envio não
  grava o seu endereço IP; a rede da Cloudflare o processa em trânsito para
  entregar a conexão.

O Sentry e a Cloudflare são empresas dos Estados Unidos. Os dois guardam os
dados fora do Brasil, na União Europeia: o Sentry na Alemanha, a Cloudflare na
jurisdição da União Europeia. Ninguém além dos dois fornecedores
recebe esses dados, e eles não são vendidos nem usados para publicidade.

## 4. Por quanto tempo fica guardado?

- **Registro das sessões:** 12 meses, apagado automaticamente por uma regra do
  armazenamento.
- **Relatórios de travamento:** o prazo configurado no projeto do Sentry, 30
  dias.

## 5. Com que base legal?

Consentimento: LGPD art. 7º, I, e GDPR art. 6(1)(a). Você o dá no cartão que o
jogo mostra na primeira abertura, e pode retirá-lo a qualquer momento com o
mesmo esforço.

## 6. Como desligar?

Em Ajustes, no cartão Privacidade, desligue a chave de envio. O jogo para na
hora de enviar o registro e os relatórios de erro e apaga o que estava na fila;
o relatório de um travamento que fecha o jogo deixa de sair a partir da
abertura seguinte. O registro local continua no seu computador, e a lista dos
ids das sessões já enviadas também (seção 7). Recusar ou desligar não muda
nada no jogo.

## 7. Como pedir acesso ou exclusão?

Escreva para juliano@jmcoimbra.eng.br com os ids das sessões. Em Ajustes, no
cartão Privacidade, o jogo mostra o id da sessão aberta, e o botão Copiar ids
das sessões enviadas copia os ids de todas as sessões que já chegaram ao Tombo
Studio a partir deste computador. Essa lista fica guardada só no seu
computador, com o id e a data em que cada sessão chegou e nada além disso, e desligar o
envio não a apaga, porque é ela que permite pedir a exclusão do que já foi
enviado. Como nenhum dado liga a sessão a você, esses ids são o único jeito de
achar o que foi enviado. O id tem 8 caracteres e outra sessão pode ter o
mesmo: um pedido de exclusão apaga todas as sessões guardadas com aquele id.

Você pode pedir confirmação do tratamento, acesso, correção, anonimização,
bloqueio ou exclusão, portabilidade, restrição do tratamento e a informação
sobre com quem os dados foram compartilhados; pode se opor ao tratamento e
revogar o consentimento a qualquer momento (LGPD art. 18; GDPR arts. 7(3) e
15 a 21). Você também pode reclamar à ANPD, no Brasil, ou à autoridade de
proteção de dados do seu país.

A JMC é agente de tratamento de pequeno porte e, pela Resolução CD/ANPD nº
2/2022, art. 11, está dispensada de indicar encarregado. O e-mail acima é o
canal de comunicação com o titular.

## 8. E quando esta política mudar?

A data no topo é a versão. O jogo mostra a versão em vigor em Ajustes, no
cartão Privacidade, e volta a pedir o seu consentimento quando ela muda. As
versões anteriores ficam no histórico desta página.
