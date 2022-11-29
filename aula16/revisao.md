# Resumo da Aula - 16 Mineração de regras de decisões

## Problema de Classificação / Regreção 

O objetivo da classificação/ Regreção é buscar a função. Dado um conjutos de dados (x1,x2,x3,....,xn mais conhecido como <b>Preditores</b>) quero saber qual (classe/desfecho) irá me retorna. 

## Regras de associação

-> Classificação : Temos atributo-alvo

-> Mineração de regras : Descobrir a possibilidade de qual será a proxima escolha, assim somente associando os itens  

## Na regra de Associação

Como funciona a regra de associação, vamos buscar o padrão entre os item onde varios itens em um conjuto se repete com a mesma sequencia em determinados conjuntos.

Exemplo itens de mercados 

    ``` 
        t1("leite","arroz","carne")
        t2("carne","oleo","alface")
        t3("arroz","leite","oleo)  
    ```
Classificação:
    1) classificar se pessoa pode receber financiamento

Na regra de associação a gente tem os Itens > Antecedentes > conssequentes

Também utilizamos a frequencia dos itens. Sem precisa de uma base previa de conheciento.

exemplo:
    Transações
                        O que é suporte ? Suprote é o item que se mais repete
                        sup é o suporte
                        O item A tem uma frequência 4 vezes na tabela abaixo.
                        O suporte relativo de (A) = rsup(A) = 4/6 = 0.66

"<i>Nosso objetivo é encontrar quais são essas associações entre itens pode ser um ou mais itens de origem para um item de destino, um ou mais antecedentes para um consequente, assim usando essa ideias de frequências e quantas vezes os itens aparecem juntos.</i>"      
    _____________      
    |_t_| i(t)  |      suporte(A) = sup(A) = 4
    | 1 |_ABDE__|
    | 2 |_BCE __|
    | 3 |_ABDE__|
    | 4 |_ABCE__|
    | 5 |_ABCDE_|
    | 6 |__BDC__|
    
Confiança é suporte de AB sobre o suporte de A. 

    exemplo: 
        A = 4
        B = 3
     conf = 4/4
     conf = 1

    sup(AB)/sup(A)

reposta é 1 então a gente pode dizer que, toda vez que encontramos A achamos o B em conjuto. 
