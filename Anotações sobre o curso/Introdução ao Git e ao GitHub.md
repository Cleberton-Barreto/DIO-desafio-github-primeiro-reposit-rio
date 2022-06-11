# Comandos básicos de navegação!

## Comandos no Linux

- ##### cd (para navegar nos diretórios)

- ##### ls (para listar o que tem no diretório)

- ##### mkdir (para criar um diretório)

- ##### rm (para arquivo) / rf (para diretório)






## Comandos no Windows

- ##### cd (para navegar nos diretórios)

- ##### cd .. (Para voltar ao diretório anterior)

- ##### dir ou ls (para listar o que tem no diretório)

- ##### ls -a (Para listar pastas ocultas)

- ##### mkdir (para criar um diretório)

- ##### del (para arquivo) / -rmdir (para diretório)

- ##### pwd (para mostrar o caminho do diretório)

- ##### git init (Para iniciar um repositório no git)

- ##### git add (Para mover um único arquivo e move-lo para o modo staged)

- ##### git add * (Para mover tudo que está em tracked e Untracked  para staged)

- ##### git commit (Para criar um commit)

- ##### git status (Para mostrar o status)

- ##### git config --list (Para listar todas as configurações em nosso git)

- ##### git config --global --unset “nome do que deseja mudar” (alterar dados já configurados)

- ##### git remote add “nome/apelido” e cola o link Https (para adicionar esse link ao apelido)

- ##### git remote -v (Para ver se o apelido recebeu o link como atributo)

- ##### gid push “apelido” master (Para empurrar nosso repositório ao gitHub)

- ##### git pull (Para puxar um repositório)

- ##### mv (Para mover arquivos de um lugar para outro, sua syntax é --> mv (nome do arquivo) ./(nome da pasta para onde quer mover o arquivo))






# Git - Por baixo dos panos

## Tópicos:
- #### SHA1

- #### Objetos fundamentais

- #### Sistema distribuído

- #### Segurança


## SHA1:
1. #### A sigla SHA significa Secure Hash Algorithm (Algoritmo de Hash Seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA). A grosso modo, é um encriptador muito usado hoje em dia, usando o comando direto no Git (openssl sha1 “nome do arquivo que deseja encriptar”) ele vai lhe gerar uma chave única de 40 dígitos, permitindo você saber,  quê,  se houver alteração em uma vírgula do arquivo ou objeto que você encriptou ele  já gera uma chave de 40 dígitos diferente, permitindo saber que houve alterações no conteúdo.






## Objetos Fundamentais:
- #### COMMITS --> TREES --> BLOBS


## Criando um Commit:
- ##### git add * (Passo 1)

- ##### git commit -m "Dar um nome que faça sentido ao seu commit"  (Passo 2)

##### Após esses 2 passos, teremos o seguinte padrão abaixo;

- ##### Chave sha1 --> [master (root-commit) 97e8ffa] commit inicial

- ##### Quantas linhas possui o arquivo --> 1 file changed, 21 insertions(+)

- ##### Nome do arquivo --> create mode 100644 strgonoff.md

- #### git push origin main  (Passo 3/fim)


#### Tracked --> Arquivos rastreáveis
- ##### Unmodified --> Arquivos que não sofreram alterações

- ##### Modified --> Arquivos que sofreram algum tipo de modificação

- ##### Staged --> Arquivos que estão se preparando para fazer alguma coisa

#### Untracked --> Arquivos não rastreáveis
- ##### Todo arquivo quando vira um commit, volta a ser Untracked.
