# IC-Projects
in this repository I will publish my advancement in the reseach project about technological mapping. 
This project is coordinated by professor Leomar and developed at UFPEL.



CHECK POINT LAYOUT CODE: PORTA INVERSOR 

(OK) 1. IMPLEMENTAR A DESCIDA DO OUT          
(OK) 2.IMPLEMENTAR A SUBIDA DO OUT 			  
(OK) 3. ESCRITA ENTRE UM RANGE DE LINHAS OU COLUNAS 
(OK) 4. VERIFICAR E CONCATENAR COM A STRING ANT COM A ATUAL
     5. IDENTIFICAR QUANDO É POLY OU NÓ [USANDO PAR OU IMPAR]
	 
NÓ - ALIMENTAÇÃO OU N1 POSICAO PAR 
POLY - INDICES POSICOES IMPARES 

6. CONEXAO-LIGAR PONTOS: APÓS IDENTIFICAR QUEM SAO OS ELEMENTOS DO EULER 
LIGAR OS PONTOS com o comportamento de cada um. 

NAND
	PU: VDD A OUT B VDD
	PD: GND A N1 B OUT

NOR
	PU: VDD A N1 B OUT
	PD: GND A OUT B GND



_________________________________________________________
PRÓXIMA TASK 04/04/2023
ENTREGA SEGUNDA (09/04)							FEITO

# exemplos biblioteca networkx					
1. CRIA GRAFO NÃO ORIENTADO, ADC NÓ, REMOVER NÓ  (OK)
2. PRINTAR GRAFO (OK)
3. USAR BIBLIOTECA PARA ISSO (OK)
4. PLOTANDO GRAFICAMENTE (OK)


# FUNÇÃO PARA REMOVER ARESTA (USANDO 2 PONTOS)
def remove_aresta(G):
    print("As arestas são: ")
    print(G.edges())
    edge_to_remove = input("Digite a aresta que deseja excluir (no formato 'nó1 nó2'): ")
    node1, node2 = edge_to_remove.split()
    if G.has_edge(node1, node2):
        G.remove_edge(node1, node2)
    else:
        print("A aresta não existe no grafo.")


_________________________________________________________
PRÓXIMA TASK 09/04
ENTREGA 17/04

1. IMPLEMENTAR REMOÇÃO, ADIÇÕES DENTRO CÓDIGO (NOT IMPUT)
2. CRIAR MATRIZ [X][Y]
3. TRANSFORMAR MATRIZ > GRAFO
4. FUNÇÃO TRANSFORMA MATRIZ EM GRAFO: CRIAR NÓ E ARESTAS, MAPEANDO A MATRIZ 
5. CRIA CLASSE PONTO (pos  x, pos y, metal1 = true, poly = false, contato = true)
6. CRIAR VETOR COM TAMANHO X vezes Y 
criar_vetor [x*y] de pontos 


7. FAZER UM ALGORITMO QUE CRIE O NP.ARRAY DA MATRIZ ADJACENTE. 
BASICAMENTE, # Criar matriz de adjacência
matriz_adj = np.array([[0, 1, 1], 
                        [1, 0, 1], 
                        [1, 1, 0]])

neste caso aqui, é uma matriz 3x3
 

    0  1  2  3 
_________________
0 | x  x  x  x
1 | x  x  x  x 
2 | x  x  x  x
3 | x  x  x  x

A representação do NP.array como matriz adjacente significa um true or false, indicando se há
aresta entre os indices da matriz. 


Necessário criar um array com true or false para cada um dos elementos, indicando os possiveis viznhos.
Exemplo: 

M = 3x3
elemento zero [[0,1,0,1,0,0,0,0,0]]
significa que este elemento zero tem 2 arestas, representados pelo 1. 

# MATRIZ 3X3
    0  1  2   
________________
0 | x  x  x  
1 | x  x  x   
2 | x  x  x  


# GRAFO DA MATRIZ 3X3
0   3   6
  
1   4   7                      

2   5   8

_________________________________________________________
SEARCH: 
algoritmo Astar em matriz 
algoritmo onda (busca)


