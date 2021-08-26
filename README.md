# Comandos úteis para o GIT


### Setar usuário

- git config --global user.name "teste da silva"

### Setar email

- git config --global user.email "teste@gmail.com"

#### Git -a
- Exibe arquivos e diretórios ocultos

#### history
- Histórico de comandos

#### history -c 
- Limpa o histórico de comandos

#### mkdir 
- Cria diretórios

#### rm meu_arquivo.txt 
- Remove arquivos 

#### git rm -r diretorio 
- Remove diretórios

#### mv + nome atual + novo nome 
- altera o nome de um arquivo

#### mv dir (que eu quero mover)/ dir(diretório que quero colocar)/
-Move um diretório para outro

#### cp (exemplo.txt) (exemplo2.txt)
- Faz a cópia de um arquivo para um diretório

#### ls 
- Mostra o que tem dentro de cada diretório

#### nl 
- Mostra o que tem detro de um arquivo e o numero de linhas

#### touch
- Cria arquivos ou echo > Cria arquivos

#### cd + dir 
- Entra em um diretório

#### cd / 
- Muda para o diretório raíz

#### cd ~ 
- Muda para o diretório pessoal

#### cd .. 
- Retorna

#### comando + --help
- Ajuda

#### Nano
- Edita o conteúdo de um arquivo

#### pwd 
- Mostra o caminho até onde estou 
-----------------
#### Cat + nome do arquivo 
- Exibe o conteúdo do arquivo 

#### Cat + nome do arquivo |More - |Less 
- Arquivos grandes (Paginação)
-----------------
#### Head 
- Mostra as 10 primeiras linhas de um arquivo

#### Tail 
- Mostra as 10 últimas linhas de um arquivo

#### cal
- exibe o calendário

#### Date
- Exibe a data

#### clear 
- limpa o terminal ou cntrl L

#### exit 
- fecha o terminal

#### git init 
- Inicia o git
-----------------
#### git status 
- Mostra o estado atual dos arquivos e diretórios

#### git show 
- Mostra o que foi modificado dentro de um arquivo ou diretório (O que era antes e como está atualmente)
-----------------
#### git log 
- Traz informações sobre as alterações realizadas em um diretório, traz um histórico

#### git log (exemplo.txt) 
- Traz o histórico de um arquivo ou pasta em específico

#### git log --oneline (exemplo.txt) 
- Traz o histórico de um arquivo ou pasta específica de forma resumida

#### gitk 
- Traz todo o histórico de forma gráfica e "mastigada"
-----------------
#### git add 
- Move o arquivo de untracked para unstage (Pronto para um novo commit)
-----------------
#### Comitar um arquivo
- git commit meu_arquivo.txt

#### Comitar vários arquivos:
- git commit meu_arquivo.txt meu_outro_arquivo.txt

#### Comitar informando mensagem:
- git commit meuarquivo.txt -m "minha mensagem de commit"
-----------------
#### git reset --soft head~1 
- Comando inverso do git add, reseta o último commit feito, e retorna ele para a área de staging/index, ou seja, antes do commit

#### git reset --mixed head~1 
- Reseta o útimo commit e retorna ele para área working dir, ou seja, antes de rodar o comando git add 
-----------------
#### git push origin 
- Empurra o repositorio local para o github

#### git clone + link 
- Pega/Clona o repositório remoto para o
repositório local

#### git remote -v
- Lista as conecções existentes ou para onde 
o servidor local está apontando

#### git checkout -b + nome 
- Cria uma branch e se move para ela

#### git checkout -d + nome 
- Deleta uma branch

#### git checkout + nome 
- Se move para uma branch

#### git branch
- Lista todas as branchs

#### git branch -m + novo nome da branch + nome antigo 
- Altera o nome da branch (Fora da branch a ser alterada)

#### git branch -m 
- Altera o nome da branch dentro da própria

#### git merge 
- Funde uma branch a branch atual
(Junta seus conteúdos) 
-----------------
#### | 
- Envia a saída de um comando para a entrada de outro comando permitindo a execução de dois comandos

#### > 
- Redireciona a saída de com comando para outro comando ou arquivo

#### >> 
- Redireciona a saída e adiciona a mesma para um comando ou arquivo 

#### < 
- Direciona a entrada de um arquivo para a saída de um comando 

#### & 
- Permite usar dois comandos e separar suas saídas no terminal 

#### && 
- Usado para que dois comandos sejam executados se o primeiro for executado com sucesso
-----------------
#### git stash save 
- Armazena os arquivos em uma branch enviando que eles acompanhem o usuario assim que mudar para uma nova branch

#### git stash list 
- Mostra uma lista contendo os stashs que foram feitos em uma branch

#### git stash pop (E o número do array que está armazenando as informações, verificar usando git stash list) 
- Abre o armazenamento e traz para fora as informações armazenadas

#### git stash clear 
- Limpar tudo que está contido no stash
-----------------

------------------------------------------------------------

# Estrutura dos commits
- Assunto    
- Corpo
- Rodapé

-----------------

#### Assunto: 
Curto e compreensível | Até 50 caracteres | Começo com letra maiúscula | 
Não terminar com ponto | Escrito de forma imperativa |

-----------------

#### Corpo:
Adicionar detalhes ao commit | Quebrar linha em até 75 caracteres | Explicar o commit | Usar markdown

-----------------

#### Rodapé:
Referenciar os assuntos relacionados |

#### Exemplo:
Adiciona mensagem de boas vindas
(Quebra linha)
Escrevendo mensagem de teste para que se tenha um parametro sobre 
como escrever um commit de forma correta. Esse commit faz uso de:
- Editor de código vscode
- Gith bash
(Quebra linha)
Closes #1 (Ou seja, referencia o commit a um "Issues" direto do github, pedido de alteração 
ou ideia que um usuario qualquer impôs)

-----------------



