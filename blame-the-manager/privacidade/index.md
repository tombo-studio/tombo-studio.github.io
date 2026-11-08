# Política de privacidade do Blame the Manager

Versão: 2026-11-08

Read in English: https://tombo-studio.github.io/blame-the-manager/privacy/

O Blame the Manager só envia alguma coisa para fora do seu computador se você
aceitar. Esta página diz o que sai, o que fica, para onde vai e como mudar de
ideia.

O jogo faz duas perguntas separadas, uma por nível de envio. Os relatórios de
travamento servem para achar e consertar travamentos e defeitos. Como você joga
serve para medir onde as pessoas se perdem no jogo e melhorá-lo, e também para
reproduzir um defeito. Cada resposta vale só para o seu nível: quem aceita um e
recusa o outro envia só o que aceitou.

## 1. Quem é o responsável pelos dados?

A JMC Tecnologia da Informação Ltda., CNPJ 54.004.699/0001-97, com sede no
Brasil, que opera o label Tombo Studio e publica o jogo. Ela é a controladora
dos dados para a LGPD (Lei 13.709/2018) e para o GDPR. Contato:
juliano@jmcoimbra.eng.br.

## 2. O que o jogo envia, e o que ele deixa de fora?

Nada sai sem o seu consentimento, e cada nível tem o seu. O registro completo
de cada sessão fica sempre no seu computador, na pasta de logs do jogo, com ou
sem consentimento.

### Relatórios de travamento

Se você aceitar este nível, quando o jogo trava ou dá erro sai o seguinte:

| Sai | Fica fora do relatório enviado |
|---|---|
| A mensagem e a pilha do erro, com o caminho das pastas do seu computador e o nome de uma carreira salva apagados | O caminho das pastas, o nome da máquina e o seu nome de usuário no sistema |
| Num erro do jogo e numa parada, os nomes dos 20 últimos eventos do jogo antes dela, cada um com a hora em que aconteceu | O conteúdo desses eventos: decisões, números e nomes ficam no seu computador |
| O identificador da sessão (8 caracteres, sorteado de novo a cada sessão), quando a sessão já abriu, a versão do jogo e a origem da sessão | Qualquer identificador de instalação, de conta ou de pessoa: o identificador de usuário do relatório vai zerado |
| Num erro do jogo, o nome do sistema operacional e o fabricante e a família da placa de vídeo; num erro do motor do jogo, também a versão do sistema e o modelo do aparelho, como o sistema os informa | Num erro do jogo, a versão do sistema, o modelo e o nome do aparelho, a resolução da tela e os identificadores e a versão do driver da placa de vídeo |
| Quando o jogo fica 30 segundos sem responder, a tela aberta, a temporada, a semana e quantos segundos ele ficou parado | A pilha: nesse caso o jogo não a manda |
| Num travamento que fecha o jogo, o relatório técnico do instante da falha (minidump), com o sistema e o aparelho, enviado na abertura seguinte | O minidump é a exceção desta coluna: ele copia trechos da memória do jogo naquele instante e pode carregar qualquer texto que estava nela, inclusive um nome que você digitou ou um caminho de pasta |

O identificador da sessão de um relatório só se liga a um registro guardado
quando você aceita também o segundo nível. Com só este nível aceito, o
registro daquela sessão fica no seu computador.

### Como você joga

Se você aceitar este nível, durante a carreira sai o seguinte:

| Sai | Fica fora do registro enviado |
|---|---|
| Um identificador de sessão de 8 caracteres, sorteado de novo a cada sessão (cada abertura do jogo e cada carreira começada ou carregada), e um número aleatório da mesma sessão que só separa, no armazenamento, duas sessões com o mesmo identificador; um identificador de carreira, sorteado quando a carreira começa e gravado no save dela (numa carreira começada numa versão do jogo que ainda não o gravava, calculado no carregamento a partir da semente e do clube de partida, sem ser gravado), que sai em toda linha depois que a carreira abre; com eles, a versão do jogo, a semente do mundo, o sistema operacional, o idioma e a origem da sessão | Seu nome, seu e-mail e sua conta Steam ou itch.io |
| Os eventos da sessão: telas abertas, momentos que você marcou com F8 ou M (a tela, a semana e o minuto; a nota que você digita fica só no seu computador), decisões tomadas, resultados das partidas, e os erros, com a mensagem e a pilha sem o caminho das pastas | Os nomes que você digita para o presidente, o clube ou a carreira, e os nomes de jogadores, técnicos e comissão, inclusive os de um pacote de nomes que você importou: o jogo os apaga do registro da sessão antes de enviar |
| Uma linha por sessão com a versão maior do sistema, o fabricante e a família da placa de vídeo, a resolução padrão mais próxima (ou nenhuma, quando a tela está longe de todas), a escala de tela, o renderizador e se o aparelho é um Steam Deck (deduzido do nome da placa de vídeo, sem nenhum identificador) | Qualquer identificador de instalação, de conta ou de pessoa |
| Para cada trecho, o que disparou o corte para o envio e o número dele | Suas respostas a estas duas perguntas: elas ficam só no registro do seu computador |

O identificador de sessão muda a cada sessão. O de carreira é o mesmo em
todas as sessões de uma carreira, e só serve para ligá-las entre si: duas
carreiras com o identificador gravado têm identificadores diferentes, e
ele não diz nada do computador nem de quem joga. A semente do mundo vai em
toda linha porque é ela que reproduz um defeito, e ela também é a mesma em
todas as sessões de uma carreira. A linha do dispositivo também se repete
entre as sessões de um mesmo computador. Nada disso diz quem você é, e não
usamos os dados para tentar descobrir quem jogou.

Como em qualquer conexão com a internet, o seu endereço IP chega aos
fornecedores abaixo para que o envio aconteça, nos dois níveis. Nós não o
guardamos (seção 3).

## 3. Para onde vai?

- **Relatórios de travamento:** Sentry, na região da União Europeia
  (Frankfurt, Alemanha). O jogo não põe o seu endereço IP no relatório, e o
  projeto está configurado para não guardar o endereço da conexão.
- **Como você joga:** Cloudflare, num armazenamento R2 próprio do jogo,
  criado na jurisdição da União Europeia: os registros ficam guardados em
  data centers dentro da União Europeia. O servidor que recebe o envio não
  grava o seu endereço IP; a rede da Cloudflare o processa em trânsito para
  entregar a conexão.

O Sentry e a Cloudflare são empresas dos Estados Unidos. Os dois guardam os
dados fora do Brasil, na União Europeia: o Sentry na Alemanha, a Cloudflare na
jurisdição da União Europeia. Ninguém além dos dois fornecedores
recebe esses dados, e eles não são vendidos nem usados para publicidade.

## 4. Por quanto tempo fica guardado?

- **Relatórios de travamento:** o prazo configurado no projeto do Sentry, 30
  dias.
- **Como você joga:** 12 meses, apagado automaticamente por uma regra do
  armazenamento.

## 5. Com que base legal?

Consentimento, um para cada nível: LGPD art. 7º, I, e GDPR art. 6(1)(a), e,
para quem joga na União Europeia, a Diretiva 2002/58/CE (ePrivacy), art.
5(3). Você o dá na tela que o jogo mostra na primeira abertura, antes da carta
da diretoria: as duas perguntas vêm sem resposta marcada, Enviar e Não enviar
têm o mesmo tamanho, e o jogo só segue com as perguntas da tela respondidas. O jogo não tem
conta, cadastro nem login. Você pode retirar cada consentimento a qualquer momento,
com o mesmo esforço (seção 6).

## 6. Como desligar?

Em Configurações (o botão ⚙), no cartão Privacidade, há uma chave para cada nível, e cada uma
para só o seu.

- **Enviar relatórios de travamento:** desligada, o jogo para na hora de
  enviar os relatórios de erro; o relatório de um travamento que fecha o jogo
  deixa de sair a partir da abertura seguinte.
- **Enviar como você joga:** desligada, o jogo para na hora de enviar o
  registro e apaga o que estava na fila. Ligada, o envio começa na próxima
  carreira que você começar, continuar ou carregar.

O que já chegou ao servidor fica até o prazo da seção 4 ou até um pedido de
exclusão (seção 7). O registro local continua no seu computador, e a lista dos
ids das sessões já enviadas também. Recusar ou desligar não muda nada no jogo.

## 7. Como pedir acesso ou exclusão?

Escreva para juliano@jmcoimbra.eng.br com os ids das sessões. Em Configurações, no
cartão Privacidade, o jogo mostra o id da sessão aberta, e o botão Copiar ids
das sessões enviadas copia os ids de todas as sessões cujo registro o jogo já
começou a enviar ao Tombo Studio a partir deste computador. Essa lista fica
guardada só no seu computador, com o id e a data do primeiro envio de cada
sessão e nada além disso, e desligar o envio não a apaga, porque é ela que
permite pedir a exclusão do que já foi enviado. Como nenhum dado liga a sessão
a você, esses ids são o único jeito de achar o que foi enviado. O id tem 8
caracteres e outra sessão pode ter o mesmo: um pedido de exclusão apaga todas
as sessões guardadas com aquele id.

A lista não guarda as sessões que mandaram só relatórios de travamento, e o
jogo não guarda o id delas em lugar nenhum. Esses relatórios se apagam
sozinhos em 30 dias (seção 4). Para pedir a exclusão antes disso, mande o id
da sessão aberta, que Configurações mostra: ele só serve enquanto a sessão
do erro está aberta, e um travamento que fecha o jogo leva a sessão junto.

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

A data no topo é a versão do texto, e o jogo a mostra em Configurações, no cartão
Privacidade. Cada nível tem também a data do seu escopo, a última vez em que
mudou o que ele envia:

Escopo dos relatórios de travamento: 2026-10-31

Escopo de como você joga: 2026-10-31

O jogo volta a perguntar um nível só quando o escopo dele muda, e o escopo
muda quando aquele nível passa a enviar um dado novo, para um destino novo ou
por um prazo maior. Uma correção de texto, de endereço ou de tradução muda só
a data no topo, e a pergunta não volta. Quem respondeu à pergunta única da
versão 2026-10-31 segue com a mesma resposta nos dois níveis; quem respondeu
numa versão anterior vê a pergunta de novo.

As versões anteriores ficam no histórico desta página.
