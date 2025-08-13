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
- Frontend: [Repositório](https://github.com/LLS-2024/Frontend_zebrao) e [Publicação](https://zebrao-sorveteria.surge.sh/)


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

![MER Workbench](/imgs/bancodedados.png "Modelagem do Banco de Dados")


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


# 7. Diagrama de Caso de Uso
![MER Workbench](/imgs/casosUso.jpeg "Diagrama de Caso de Uso")


