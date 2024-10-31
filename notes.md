# Linux Notes 
## Definições
> GUI - Graphical User Interface 
>
> CLI - Command Line Interface

## **Comandos**
> `sudo`
>> - Permite executar programas com previlégios de outro user
>> - por padrão, como o superuser -root. sudo significa "substitute user do"

`CTRL + L` -> Limpa o Terminal 

`clear` -> Limpa o Terminal  

`open` -> Abre o explorador de ficheiros gráfico 

`nano` -> Editor de textos

`file` -> mostra o tipo do arquivo

`history` -> Histórico de comandos já digitados 

`pkill` -> mata processos

`whoami` -> mostra user

`hostname` -> mostra o nome do computador

`uname` -> mostra dados sobre o sistema

`ps aux` -> mostra todos os processos ativos no sistema no momento da execução

## Navegação
> pwd.
>> print working directory (mostra o caminho do diretótio atual)

> ls.
>> lista tudo no diretório atual 
- -a -> inclui entradas que o nome começa por ponto (ocultos)
- -l -> lista em formato longo
- - -la -> compõe as duas flags 
- -h -> com -l sufixo de tamanho para facilitar a leitura
- -@ -> mostra com atributos extendidos
> cd
>> change directory 
- . -> Diretório atual
- .. -> Diretório acima
- / -> Diretório root ou a separação de diretórios
- ~ -> home (cd sem nada vai para a home)
- '-' -> (menos volta para o diretório anterior)
> tree
>> mostra a árvore do diretório atual 
- -d -> Diretórios
- -a -> arquivos ocultos
> cat
>> concatena e mostra o conteúdo de um arquivo
- -n -> enumera as linhas
> tail
>> list as últimas linhas do arquivo
- -NÚMERO -> mostra a quantidade de linhas que for adicionado em NÚMERO
- -f -> continua assistindo o arquivo em busca de novos dados.
> wc
>> conta linhas, palavras e carateres
- -l -> linhas
- -m -> caracteres
- -w -> palavras
## Manipular Arquivos
- `cp` - copia arquivos ou diretórios
  - R -> copia o diretório em modo recursivo
    ###### Obs.: Segundo o man (manual) dp cp, se tiver uma barra (/) no final do
    ###### diretório original, cp pode copiar apenas o conteúdo do diretório e não o
    ###### diretório em si (não observado em testes)
- `mv` - move os arquivos ou diretórios (com mv pode renomear arquivos ou diretórios)

- `mkdir` - cria um diretório (use aspas ou barra invertida para separar caracteres     invalidos)
    - -p -> cria uma estrutura inteira sem gerar error
    ###### Obs.: pose usar chaves para criar múltiplos sub-diretórios
- `rm` - apaga arquivos e diretórios
    - -R -> modo recursivo para directórios
    - -f -> modo forçado e silencioso
- `touch` - muda os tempos de acesso e modificação de um arquivo. Grande parte dos casos, usamos este comando para criar um arquivo vazio.
## Símbolos (Operadores) úteis
- `;` -> permite executar vários comandos na mesma linha. Executa todos os comandos, mesmo se ocorrer algum erro.                    
- `&&` -> permite executar vários comandos na mesma linha. Se o comando anterior não gerar nenhum erro, continua a corrente de comandos, caso contrário, pára no momento que ocorrer um erro
- `||` -> permite executar vários comandos na mesma linha. Funciona de maneira oposta ao anterior, ou seja, se ocorrer algum erro no comando anterior, executa o próximo comando, caso contrário, pára no primeiro comando que não gerar um erro.
- `|` -> envia a saída (output) de um comando para a entrada (input) de outro.



