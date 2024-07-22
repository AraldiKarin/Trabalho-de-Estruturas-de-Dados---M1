Este Trabalho foi feito pelos alunos Karin Araldi, Ana Beatriz da Conceição e Kauan Borges Kuball, este trabalho foi feito na matéria de Estruturas de Dados com o professor Eduardo Alves da Silva.
O objetivo deste trabalho é implementar a sistemática de atualização de 3 listas de filmes para cada usuário no sistema.
As listas que cada usuário possui são:
(a) lista de filmes assistidos;
(b) lista de filmes salvos para assistir depois;
(c) lista de filmes recomendados

Definições:
1. O catálogo de filmes disponíveis é composto por 500 itens;
2. A lista de filmes que o usuário assistiu pode chegar a 50 itens;
3. A lista de filmes salvos para assistir depois é de no máximo 20 itens; 
4. A lista de filmes recomendados para o usuário assistir é de exatamente 10 itens; e
5. O sistema pode ter no máximo 100 usuários.

Cada filme possui as informações: Título, Gênero, Elenco;

Cada usuário possui as informações: Nome, Idade, Gêneros de filmes que mais gosta (até 3).

O sistema não possuirá a opção de cadastrar filmes no catálogo. Logo, os filmes do catálogo devem ser gerados empiricamente (ex.: aleatoriamente ou lidos de um arquivo de texto ou CSV – Comma Separated Values – Valores Separados por Vírgula).
A lista de filmes assistidos por cada usuário deve ser passível de atribuição via funcionalidade no sistema E deve haver uma opção de auto processamento. Por exemplo, eu como usuário 1 quero adicionar o filme X na minha lista de assistidos
(funcionalidade de escolher o filme), mas também, eu como testador quero ter uma opção para adicionar 23 filmes a minha lista (pode ser 23 opções aleatórias do catálogo) = OBS: como testador quero poder escolher quantos filmes adiciono no 
auto processamento (ex. 23, 12, 5, etc). Após um filme ser adicionado como assistido, ele não pode ser removido desta lista (não há como desassistir).
A lista de filmes salvos para assistir depois deve seguir a mesma sistemática da lista de filmes assistidos, atribuição manual via sistema ou auto processamento para fins de testes. Porém, o usuário pode ter a opção de remover um ou vários
filmes da lista de salvos para depois (por interação ou auto processamento).
A lista de filmes recomendados para o usuário assistir deve ser montada a critério de cada grupo (ex. aleatoriamente, com base nos gêneros que o usuário gosta, com base nos gêneros dos filmesassistidos pelo usuário, com base nos gêneros dos
filmes da lista de filmes salvos para assistir depois, com base em filmes assistidos por outros usuários, etc).

O sistema deve possuir opção para visualizar:
a. As 3 listas de filmes de um usuário em particular; 
b.  A lista de filmes do catálogo.

Deve ser implementado:
• TAD de Lista Estática Genérica (5 pontos), com as seguintes operações:
o Inicializar lista;
o Inserir na lista (início, posição, fim);
o Remover da lista (início, posição, fim);
o Obter item da lista – recebe a posição como parâmetro e retorna o dado daquela posição (se existir);
o Contém item – recebe o dado e verifica se ele está na lista. Se estiver, retorna verdadeiro, falso caso contrário;
o Descobrir índice – recebe o dado e busca-o na lista. Se estiver na lista, retorna à posição do dado na lista, caso contrário, retorna -1.
o Imprimir lista;
• TADs do Problema/contexto/domínio (2 pontos): Recomendador Flix.
• Correto funcionamento dos requisitos do trabalho (3 pontos)
o 1,5 para interação manual; e
o 1,5 para as opções de auto processamento.
OBS: O auto processamento referido no enunciado do trabalho é apenas para emular (automaticamente, sem interação do usuário) o comportamento de várias interações (ex. adicionar 5 filmes na lista de assistidos do usuário 1) para facilitar o processo de testes.
