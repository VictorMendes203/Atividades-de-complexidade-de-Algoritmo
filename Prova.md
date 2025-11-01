🧠 Questionário — Complexidade de Algoritmos
--------------------------------------------------------

📘 Versão Fácil

1. O que significa a palavra *complexidade* quando falamos de um algoritmo?
   Resposta: Complexidade de algoritmo realiza a medição de consumo de tempo e memoria de acordo com o aumento da entrada

2. Qual é a diferença entre *tempo de execução* e *uso de memória* em um algoritmo?
   Resposta: O tempo de algoritmo está relacionado a quanto tempo o algoritmo demora para terminar de rodar, em quanto o uso de memoria e a quantidade de espaço aquele algoritmo está utilizando durante sua execução
   
3. Para que serve a *notação Big O (O-grande)*?
   Resposta: A notação Big O é usada para classificar algoritmos de acordo com como seus requisitos de tempo de execução ou espaço em relação ao tamanho de entrada
   
4. O que representa o termo *n* dentro da notação O(n)?
   Resposta: O termo "n" representa o tamanho da entrada, como por exemplo a quantidade de paginas de um livro
   
5. Cite um exemplo de algoritmo com complexidade *O(1)*.
   Resposta: Inserir ou remover um item de uma fila (Queue) ou pilha (Stack). As operações de push e pop em uma pilha geralmente envolvem apenas a manipulação de um ponteiro ou índice, o que é uma operação de tempo constante.
    
6. Cite um exemplo de algoritmo com complexidade *O(n)*.
   Resposta: Contar o número total de elementos em uma lista ligada (linked list) requer percorrer a lista do início ao fim, visitando cada um dos "n" nós exatamente uma vez, resultando em complexidade O(n). 
    
7. Qual a complexidade de tempo do algoritmo de *Bubble Sort*?
    Resposta: "Bubble Sort" tem complexidade *O(n²)*.
   
8. Qual a complexidade de tempo do algoritmo de *Busca Linear*?
   Resposta: "Busca Linear" é *O(n)*.
   
9. O que significa dizer que um algoritmo tem complexidade *O(log n)*?
    Resposta: Dizer que um algoritmo tem complexidade "O(log n)" significa que o tempo de execução ou a quantidade de recursos cresce proporcionalmente ao logaritmo do tamanho da entrada "n"
   
10. Qual a diferença entre *melhor caso* e *pior caso* de um algoritmo?
    Resposta: "Melhor caso" e quando e executado o mais rapido possivel, já no caso do "Pior caso" e quando o algoritmo executa o mais devagar possivell
    
11. Em qual tipo de problema geralmente encontramos complexidades *exponenciais (O(2ⁿ))*?
    Resposta: Complexidades exponenciais (O(2ⁿ)) são geralmente encontradas em problemas considerados "difíceis" ou intratáveis, para os quais os algoritmos conhecidos frequentemente utilizam a estratégia de força bruta ou tentam explorar todas as possíveis combinações ou permutações para encontrar a solução. 
    
12. O que é *complexidade polinomial*?
    Resposta: "Complexidade polinomial" é quando o tempo cresce como uma potência de n (ex: n², n³). 
    
13. Qual a complexidade do *Merge Sort* no pior caso?
    Resposta: A complexidade do Merge Sort no pior caso é *O(log n)*
    
14. Em um algoritmo que possui *dois loops for aninhados*, qual costuma ser sua complexidade?
    Resposta: A complexidade de tempo de um algoritmo com dois loops for aninhados costuma ser quadrática, ou O(n²)
      
15. Por que os programadores buscam algoritmos com menor complexidade?
    Resposta: Os programadores buscam algoritmos com menor complexidade para garantir que os programas sejam mais rápidos, eficientes e escaláveis, ou seja, que consumam menos recursos computacionais, como tempo de processamento e memória, especialmente ao lidar com grandes volumes de dados. 
    
16. Um algoritmo que analisa cada elemento de uma lista apenas uma vez é O(n). Isso é considerado eficiente?
    Resposta: Sim, pois um algoritmo com complexidade de tempo O(n) é considerado eficiente, especialmente para conjuntos de dados de tamanho moderado a grande. 
    
17. A notação *Θ (teta)* indica o quê em relação ao crescimento da função?
    Resposta: A notação assintótica Θ (teta) indica o limite assintótico exato (ou "justo") do crescimento de uma função. 
    
18. Qual é a complexidade de tempo de um algoritmo que executa *três loops aninhados* sobre n elementos?
    Resposta: Três loops aninhados → "O(n³)". 
    
19. O que significa dizer que um algoritmo é *in-place*?
    Resposta: Dizer que um algoritmo é in-place (no local, em português) significa que ele opera diretamente na estrutura de dados de entrada, modificando-a no seu próprio local de memória, sem a necessidade de alocar uma quantidade significativa de memória adicional que dependa do tamanho da entrada. 

20. Cite um exemplo de *estrutura de dados* que pode melhorar a eficiência de um algoritmo.
    Resposta: Heaps (Pilhas/Montes): São estruturas de dados baseadas em árvores especializadas que suportam operações eficientes de fila de prioridade, onde o elemento máximo ou mínimo pode ser localizado e removido rapidamente (O(log n)).

-----------------------------------------------------------------------------------------

🔬 Versão Difícil
----------------------------------------------
1. Explique por que analisamos a complexidade de tempo *em função do tamanho da entrada (n)*.
   Resposta: porque o principal interesse é entender como o desempenho do algoritmo escala à medida que o volume de dados aumenta, independentemente de fatores externos como o hardware utilizado. 
     
2. Dê um exemplo de algoritmo cuja complexidade muda dependendo da escolha da estrutura de dados.
   Resposta: Algoritmo de Inserção e Remoção de Elementos
   
3. Mostre como se calcula a complexidade assintótica da função *f(n) = 4n² + 3n + 10*.
   Resposta: "f(n) = 4n² + 3n + 10 → O(n²)", pois o termo de maior grau domina o crescimento. 
   
4. Prove que *O(n² + n) = O(n²)*.
   Resposta:  Como n² cresce mais rápido que *n, o termo n é desprezável — logo, O(n² + n) = O(n²).  
   
5. Qual é a diferença entre as notações *O(n)* e *Ω(n)* em termos de limites de crescimento?
   Resposta: A principal diferença é que O(n) (Big O) representa um limite superior (pior caso) e Ω(n) (Big Omega) representa um limite inferior (melhor caso) para o crescimento de uma função.
   
6. Escreva a relação de recorrência do algoritmo *Merge Sort* e resolva-a usando o *Teorema Mestre*.
   Resposta: "T(n) = 2T(n/2) + n" → pelo "Teorema Mestre, temos "O(n log n)".  
   
7. Mostre um exemplo de algoritmo cuja complexidade é *O(n log n)* e explique por que esse comportamento ocorre.
   Resposta: O Quick Sort possui uma complexidade de tempo de O(n log n) no caso médio e melhor, mas pode degradar para O(n²) no pior caso. 
   
8. Explique o que significa o *custo amortizado* em operações de uma *tabela hash*.
   Resposta: Em operações de uma tabela hash, o custo amortizado refere-se ao custo médio de uma operação (como inserção ou remoção) calculada ao longo de uma sequência de muitas operações. 
   
9. Dado um algoritmo com complexidade *T(n) = 2T(n/2) + n*, determine sua ordem de crescimento.
    Resposta: 'T(n) = 2T(n/2) + n → O(n log n)" e o mesmo resultado do Merge Sort. 
    
10. Compare o desempenho de algoritmos com complexidade *O(n log n)* e *O(n²)* para valores grandes de n.
    Resposta: Para valores grandes de n, "O(n log n)" cresce muito mais lentamente que "O(n²)" logo, é mais eficiente.
     
11. Um algoritmo recursivo é definido por *T(n) = T(n-1) + n*. Qual é sua complexidade aproximada?
    Resposta: "T(n) = T(n-1) + n → O(n²)" a soma aritmética de 1 a n. 
    
12. Qual o impacto da escolha de pivô na complexidade média do *Quick Sort*?
    Resposta: A escolha do pivô não altera a complexidade média assintótica do Quick Sort, que é universalmente O(n log n). No entanto, ela tem um impacto crucial na probabilidade de ocorrência do pior caso (O(n²)) e nas constantes multiplicativas do caso médio, afetando o desempenho prático do algoritmo. 
    
13. Explique o conceito de *limite inferior (lower bound)* para algoritmos de ordenação.
    Resposta: O limite inferior (lower bound) para algoritmos de ordenação baseados em comparações é a complexidade de tempo mínima possível que qualquer algoritmo pertencente a essa categoria deve atingir para garantir que a ordenação seja concluída corretamente em todos os casos. 
     
14. Dê um exemplo de problema *NP-difícil* e explique o que isso significa em termos de complexidade.
    Resposta: O problema consiste em, dado um conjunto de cidades e as distâncias entre cada par delas, encontrar a rota mais curta possível que visita cada cidade exatamente uma vez e retorna à cidade de origem. 
    
15. Por que não é possível encontrar algoritmos polinomiais conhecidos para resolver todos os problemas *NP-completos*?
    Resposta: Não foi possível encontrar algoritmos polinomiais para problemas NP-completos porque isso implicaria que P = NP, o que é um problema em aberto não resolvido na ciência da computação.
    
16. Mostre um exemplo prático em que a análise de complexidade *pode orientar o design de software*.
    Resposta: A escolha do algoritmo de ordenação para uma grande quantidade de dados em um sistema de banco de dados ou em uma aplicação de e-commerce
     
17. Explique a diferença entre *complexidade no caso médio* e *complexidade no pior caso*.
    Resposta: No caso medio o comportamento e tipico em quanto no pior caso, a execução e mais demorada
  
18. Um algoritmo que compara todos os pares de elementos em uma lista de tamanho n possui qual complexidade?
    Resposta: Um algoritmo que compara todos os pares de elementos em uma lista de tamanho "n" tem complexidade quadrática, representada como O(n²).
    
19. Mostre por que *f(n) = n!* cresce mais rapidamente do que *f(n) = 2ⁿ*.
    Resposta: "n!" cresce mais rápido porque *multiplica por números cada vez maiores, enquanto "2ⁿ" apenas dobra a cada passo.  

    
20. Se um algoritmo tem tempo de execução *T(n) = n² log n + 5n*, qual é sua complexidade em notação O?
    Resposta: "T(n) = n² log n + 5n → O(n² log n)" e o termo dominante.
