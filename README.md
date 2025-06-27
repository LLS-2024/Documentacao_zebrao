# Zebrão Sorveteria


O Zebrão Sorvetes é uma sorveteria física real, porém ela não possui um site de vendas online. Então, nosso objetivo é criar um site que eles poderiam utilizar para suas vendas, incluindo um sistema de delivery para facilitar.

 No projeto, pretendemos incluir uma enorme variação de doces gelados, como sorvetes de pote, casquinhas, açaís, geladinhos e picolés, além de adicionais como caldas, granulados e balas.

 O usuário terá a possibilidade de pedir via delivery, assim paga direto no próprio site e precisa informar seu endereço ou de retirar na loja, onde fica a cargo do funcionário na loja física.


Professor: [Marco André Mendes](github.com/marcoandre)

Equipe:
- [Leila da Silva Souza](github.com/aluno1)
- [Luiza Escarban da Silva](https://github.com/Luizaescarban)
- [Sarah Letícia de Jesus](https://github.com/SarahLJesus)

Links do projeto:
- [Documentação (esse documento)](https://github.com/LLS-2024/Documentacao_zebrao)
- Backend: [Repositório](https://github.com/LLS-2024/Backend_zebrao) e [Publicação](https://pi-backend.herokuapp.com/)
- Frontend: [Repositório](https://github.com/LLS-2024/Frontend_zebrao) e [Publicação](https://pi-frontend.herokuapp.com/)


# 1. Desenvolvimento
  O Zebrão Sorvetes é uma sorveteria física real, porém ela não possui um site de vendas online. Então, nosso objetivo é criar um site que eles poderiam utilizar para suas vendas, incluindo um sistema de delivery para facilitar.

 No projeto, pretendemos incluir uma enorme variação de doces gelados, como sorvetes de pote, casquinhas, açaís, geladinhos e picolés, além de adicionais como caldas, granulados e balas.

 O usuário terá a possibilidade de pedir via delivery, assim paga direto no próprio site e precisa informar seu endereço ou de retirar na loja, onde fica a cargo do funcionário na loja física.
 
# 2. Situação Problema


 O problema a ser trabalhado, é o fato do Zebrão Sorvetes(loja física real) não possuir um site de vendas bom, o que pode dificultar a comercialização de seus produtos. Mesmo tendo atualmente um site, o mesmo não possui imagens chamativas, nem nada atrativo.


Eles provavelmente perdem muitos clientes por não terem um site chamativo de divulgação com seus principais produtos.


O funcionamento da sorveteria é convencional, onde as pessoas apenas vão, escolhem o pote de sorvete, casquinha ou picolé desejado, pagam pelo produto e ou consomem no local, ou levam para casa por si próprios e mesmo tendo sistema de delivery, quase nenhum cliente o usa por ser meio desconhecido,


 Zebrão Sorvetes, fazem a comercialização de sorvetes, açaís, casquinhas e picolés, fundada em 21/11/1977, dono e funcionários desconhecidos.


 A empresa funciona todos os dias da semana, das 10:00 às 21:00 horas.

 Possuem loja física, onde o cliente mesmo se serve.

 Possuem um sistema de delivery pouco conhecido.


 Concluindo, o nosso projeto poderia ajudá-los a melhorar suas vendas, atraindo mais o público e incentivando mais os pedidos de delivery. 



# 3. Descrição da proposta


“O nosso software vai ajudar você, dono da Zebrão Sorvetes a vender muito mais e otimizar o tempo dos seus clientes que não tem conhecimento do serviço delivery. Será um site mais atrativo e moderno com propostas empreendedoras de vendas.

 Ele poderá receber pedidos no horário de atendimento, mostrar as opções do cardápio, formas de pagamento, etc.

Além disso, tanto os funcionários terão acesso para cadastrar produtos, quanto os clientes para comprar.”


# 4. Modelagem de Dados

![MER Workbench](/imgs/bancodedados.png "Diagrama de Caso de Uso")


# 4. Regras de negócio

RN001: A entidade Pessoa deve conter os dados: id, nome, cpf e email. Ela representa tanto funcionários quanto clientes. Além disso, deve se associar a tabelas que armazenem múltiplos telefones e múltiplos endereços, sendo que o endereço deve conter: cep, número e complemento.

RN002: O carrinho deve conter o id dos produtos adicionados, a quantidade de cada produto e o id do cliente responsável.

RN003: O pagamento deve conter um id próprio, o nome do banco, o código do banco e o tipo de pagamento.

RN004: Cada produto deve conter: um id, descrição, valor de venda, valor de compra (que não deve ser exibido ao cliente), validade e categoria correspondente.

RN005: A categoria é dependente da existência de produtos. Caso não haja produtos relacionados a uma categoria, ela deve ser automaticamente removida para evitar redundância.

RN006: A venda deve conter: um id, a data da venda e o id do cliente que realizou a compra.

RN008: A tabela Produto_venda deve conter a quantidade de produtos vendidos, além dos ids relacionados à venda, ao cliente e aos produtos.


# 5. Requisitos funcionais

RF001: O sistema deve manter Pessoa.

RF002: O sistema deve manter Carrinho.

RF003: O sistema deve manter Pagamento.

RF004: O sistema deve manter Produtos.

RF005: O sistema deve manter Categoria.

RF006: O sistema deve manter Venda.

RF008: O sistema deve manter Produto_venda.


# 6. Requisitos não funcionais

RNF001: O frontend da aplicação deve ser desenvolvido utilizando o framework VueJS.

RNF002: A linguagem de programação utilizada no frontend deve ser JavaScript.

RNF003: A interface do frontend deve utilizar o framework CSS Bootstrap ou Tailwind, na versão mais recente disponível.

RNF004: O backend da aplicação deve ser programado na linguagem Python.

<!-- *( --- 
# 7. Diagrama de Caso de Uso

**7.1 Introdução**

O diagrama de caso de uso é uma ferramenta de modelagem que descreve o comportamento de um sistema a partir da perspectiva do usuário. Ele é usado para capturar os requisitos funcionais de um sistema.

- Especificam a visão externa do sistema.
- Descrevem como o sistema é percebido por seus usuários.
- Descrevem as interações entre os usuários e o sistema.

![Diagrama de Caso de Uso](img/dcu1.png "Diagrama de Caso de Uso")

**Os casos de uso:**
- Descrevem como os **usuários interagem com o sistema** (as funcionalidades do sistema)
- Facilitam a **organização dos requisitos** de um sistema.
- Dão uma **visão externa** do sistema
- O conjunto de casos de uso deve ser capaz de comunicar a **funcionalidade** e o **comportamento** do sistema para o cliente.
- Descrevem **o que** o sistema faz, mas **não** especificam **como** isso deve ser feito.

**7.2 Elementos do diagrama de caso de uso**

7.2.1 **Atores**

- Representam os papéis desempenhados por **elementos externos** ao sistema
  - Ex: humano (usuário), dispositivo de hardware ou outro sistema (cliente)
- Elementos que **interagem** com o sistema

Notação:

![Atores Notação](img/dcu_atores_notacao.png "Atores Notação")

**Exemplo: Loja de CDs**

**Identificando os atores**
- Uma loja de CDs possui discos para venda. Um cliente pode comprar uma quantidade ilimitada de discos para isto ele deve se dirigir à loja.
- A loja possui um **atendente** cuja função é atender os clientes durante a venda dos discos. A loja também possui um **gerente** cuja função é administrar o estoque para que não faltem discos. Além disso é ele quem dá folga ao atendente, ou seja, ele também atende os clientes durante a venda dos discos.

![Identificando os atores](img/dcu_identificando_atores.png "Identificando os atores")

**E o cliente?**
- Não é ator pois ele **não interage** com o sistema!

**7.2.2 Casos de uso**

- Representam **funcionalidades** do sistema (requisitos funcionais).
- São iniciados por **atores** ou por outros casos de uso.

> **Dica**: nomeie os casos de uso com **verbos** no **infinitivo**.

Notação:

![Casos de uso Notação](img/dcu_casos_de_uso_notacao.png "Casos de uso Notação")

**Exemplo: Loja de CDs**

**Identificando os casos de uso**

- Uma loja de CDs possui discos para venda. Um cliente pode comprar uma quantidade ilimitada de discos para isto ele deve se dirigir à loja. A loja possui um atendente cuja função é atender os clientes durante a **venda dos discos**.
- A loja também possui um gerente cuja função é **administrar o estoque** para que não faltem discos. Além disso é ele quem dá folga ao atendente, ou seja, ele também atende os clientes durante a **venda dos discos**.

![Identificando os casos de uso](img/dcu_identificando_casos_de_uso.png "Identificando os casos de uso")

**7.2.3 Relacionamentos**

**7.2.3.1 Relacionamento de associação**

- Indica que um ator **participa** de um caso de uso, ou seja, o ator **interage** (comunica-se) com o caso de uso.
- É representado por uma **linha sólida**.
- Um ator pode se relacionar com **um ou mais casos de uso**.

> Dicas:
> - Não use setas nas linhas de associação.
> - Associações não representam fluxo de informação.

![Relacionamento de associação](img/dcu_relacionamento_de_associacao.png "Relacionamento de associação")

**Exemplo: Loja de CDs**

**Identificando os relacionamentos de associação**

- Uma loja de CDs possui discos para venda. Um cliente pode comprar uma quantidade ilimitada de discos para isto ele deve se dirigir à loja. A loja possui um _atendente_ cuja função é atender os clientes durante a **venda dos discos**.
- A loja também possui um _gerente_ cuja função é **administrar o estoque** para que não faltem discos. Além disso é ele quem dá folga ao _atendente_, ou seja, ele também atende os clientes durante a **venda dos discos**.

![Identificando os relacionamentos de associação](img/dcu_identificando_relacionamentos_de_associacao.png "Identificando os relacionamentos de associação")

**7.2.3.2 Relacionamento de generalização/especialização**

**Generalização de atores**

- Quando dois ou mais atores podem se **comunicar com o mesmo conjunto de casos de uso**.
- Indica que um ator **herda** as características de outro ator.
– Um filho (herdeiro) pode se comunicar com todos os casos de uso que seu pai se comunica.

> **Dica:** coloque os herdeiros **embaixo**.

**Notação:**

![Relacionamento de generalização/especialização de atores - notação](img/dcu_relacionamento_de_generalizacao_especializacao_notacao_de_atores.png "Relacionamento de generalização/especialização de atores - notação")
￼


**Exemplo: Loja de CDs**

**Identificando os relacionamentos de generalização/especialização de atores**

![Identificando os relacionamentos de generalização/especialização de atores](img/dcu_identificando_relacionamentos_de_generalizacao_especializacao_de_atores.png "Identificando os relacionamentos de generalização/especialização de atores")

**Generalização de casos de uso**

– O caso de uso filho herda o comportamento e o significado do caso de uso pai.
– O caso de uso filho pode incluir ou sobrescrever o comportamento do caso de uso pai.
– O caso de uso filho pode substituir o caso de uso pai em qualquer lugar que ele apareça.

> **Dica:** deve ser aplicada quando uma condição resulta na definição de
diversos fluxos alternativos.

Notação:

![Relacionamento de generalização/especialização de casos de uso - notação](img/dcu_relacionamento_de_generalizacao_especializacao_notacao_de_casos_de_uso.png "Relacionamento de generalização/especialização de casos de uso - notação")

**Exemplo: Loja de CDs**

**Identificando os relacionamentos de generalização/especialização de casos de uso**

**Novos requisitos:**

￼

- As vendas podem ser **à vista** ou **a prazo**. Em ambos os casos o estoque é
atualizado e uma nota fiscal, entregue ao consumidor.
- No caso de uma **venda à vista**, clientes cadastrados na loja e que compram mais de 5 CDs de uma só vez ganham um desconto de 1% para cada ano de cadastro.
- No caso de uma **venda a prazo**, ela pode ser parcelada em 2 pagamentos com um
acréscimo de 20%. As vendas a prazo podem ser pagas no **cartão** ou no **boleto**.
  - Para pagamento com **boleto**, são gerados boletos bancários que são entregues ao cliente e armazenados no sistema para lançamento posterior no caixa.
  - Para pagamento com **cartão**, os clientes com mais de 10 anos de cadastro na loja ganham o mesmo desconto das compras à vista.

![Identificando os relacionamentos de generalização/especialização de casos de uso](img/dcu_identificando_relacionamentos_de_generalizacao_especializacao_de_casos_de_uso.png "Identificando os relacionamentos de generalização/especialização de casos de uso")

**Identificando mais relacionamentos de generalização/especialização de casos de uso**

![Identificando mais relacionamentos de generalização/especialização de casos de uso](img/dcu_identificando_mais_relacionamentos_de_generalizacao_especializacao_de_casos_de_uso.png "Identificando mais relacionamentos de generalização/especialização de casos de uso")

**7.2.3.3 Relacionamento de dependência**

**Extensão**

- Representa uma variação/extensão do comportamento do caso de uso base.
- O caso de uso estendido só é executado sob certas circunstâncias.
- Separa partes obrigatórias de partes opcionais.
  - Partes obrigatórias: caso de uso base.
  - Partes opcionais: caso de uso estendido.
- Fatorar comportamentos variantes do sistema (podendo reusar este comportamento
em outros casos de uso).

**Notação:**

![Relacionamento de dependência (extensão) - notação](img/dcu_relacionamento_de_dependencia_extensao_notacao.png "Relacionamento de dependência (extensão) - notação")

**Exemplo: Loja de CDs**

**Identificando os relacionamentos de dependência (extensão)**

**Novos requisitos:**
- No caso de uma venda à vista, clientes cadastrados na loja e que compram mais
de 5 CDs de uma só vez ganham um **desconto** de 1% para cada ano de cadastro.
- No caso de uma venda a prazo...
  - ...Para pagamento com cartão, os clientes com mais de 10 anos de cadastro na loja ganham o mesmo **desconto** das compras à vista.

![Identificando os relacionamentos de dependência (extensão)](img/dcu_identificando_relacionamentos_de_dependencia_extensao.png "Identificando os relacionamentos de dependência (extensão)")

**Inclusão**

- Evita repetição ao fatorar uma atividade
comum a dois ou mais casos de uso.
- Um caso de uso pode incluir vários casos de uso.

**Notação:**

![Relacionamento de dependência (inclusão) - notação](img/dcu_relacionamento_de_dependencia_inclusao_notacao.png "Relacionamento de dependência (inclusão) - notação")

**Exemplo: Loja de CDs**

**Novos requisitos:**
Para efetuar vendas ou administrar estoque, atendentes e gerentes terão que **validar** suas respectivas senhas de
acesso ao sistema.
￼


![Identificando os relacionamentos de dependência (inclusão)](img/dcu_identificando_relacionamentos_de_dependencia_inclusao.png "Identificando os relacionamentos de dependência (inclusão)")

**7.2.4 Fronteira do sistema**

- Elemento opcional (mas essencial para um bom
entendimento).
- Serve para definir a área de atuação do sistema, ou seja, seus limites.

**Identificando a fronteira do sistema**

![Identificando a fronteira do sistema](img/dcu_identificando_a_fronteira_do_sistema.png "Identificando a fronteira do sistema")

---
)*


