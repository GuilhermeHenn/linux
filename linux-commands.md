# Comandos Linux

Listar os arquivos contidos no diretório
```bash  
ls
```
<br>

Listar os arquivos contidos no diretório, incluindo os arquivos “ocultos”
```bash
ls -a
```
<br>

Exibir um manual do comando
```bash
man "comando"
```
<br>

Resumo do que o comando é capaz de fazer
```bash
"comando" --help
```
<br>

Limpar o terminal
```bash
clear 
```
<br>

Criar um novo diretório/pasta
```bash  
mkdir "nomePasta"
```
<br>

Mover-se entre diretórios
```bash
cd "./Pasta/OutraPasta/diretórioDestino"
```
<br>

Mostrar o caminho completo até o diretório atual
```bash
pwd
```
<br>

Mostrar o nome do usuário logado
```bash
whoami
```
<br>

Jogar a saída de um comando para dentro de um arquivo
```bash
whoami >> "user.txt"
```
<br>

Criar um novo arquivo
```bash
touch "arquivo.txt"
```
<br>

Abrir arquivo de texto por meio do editor nano 
```bash
nano "arquivo.txt"
```
<br>

Mostrar o conteúdo de um arquivo 
```bash
cat "arquivo.txt"
```
<br>

Alterar o nome de um arquivo
```bash
mv "nomeAntigo.txt" "nomeNovo.txt"
```
<br>

Copiar um arquivo para algum diretório
```bash
cp "arquivo.js" "~/Pasta01/Pasta01/PastaDestino"
```
<br>

Buscar o diretório no qual determinado arquivo se encontra
```bash
find -name "arquivo.md"
```
<br>

Listar as primeiras linhas de um arquivo
```bash
head "arquivo.txt"
```
<br>

Listar as últimas linhas de um arquivo
```bash
tail "arquivo.txt"
```
<br>

Carregar o conteúdo de um arquivo conforme a rolagem do scroll
```bash
less "arquivo.txt"
```
<br>

Apagar um arquivo
```bash
rm "arquivo.txt"
```
<br>

Apagar um diretório/pasta
```bash
rmdir "Pasta"
```
<br>

Apagar uma pasta que possui conteúdo dentro **(utilizar com cuidado!)**
```bash
rm -rf "Pasta"
```
<br>

Descobrir o nome da máquina
```bash
hostname
```
<br>

Listar os IPs da máquina
```bash
hostname -I
```
<br>

Listar os IPs da máquina de forma detalhada
```bash
ip a
```
<br>

Pegar a saída de um comando e jogar para algum outro programa, por meio do `|` <br>
No exemplo abaixo, a saída do comando `ip a` é jogada para o programa `grep`. O programa `grep`, por sua vez, foi utilizado para filtrar o conteúdo obtido pelo comando `ip a`, listando apenas o que há "inet"
```bash
ip a | grep inet
```
<br>

Descobrir se um IP/URL/domínio está acessível, listando quanto tempo leva para receber um *response* do servidor após o *request* feito <br>
O comando retorna o IP do domínio "pingado" e também quantos pacotes foram transmitidos, recebidos e perdidos
```bash
ping "IP/URL/domínio"
```
<br>

Listar informações referentes a determinado domínio
```bash
nslookup "domínio"
```
<br>

Listar informações sobre a memória RAM:
- Memória total
- Memória em uso
- Memória livre
- Memória compartilhada
- Memória em *swap* 
```bash
free -h
```
<br>

Monitorar e derrubar processos do SO <br>
Semelhante ao Task Manager do Windows, porém no terminal
```bash
htop 
top 
```
<br>

Listar os processos que estão rodando no SO
```bash
ps aux
```
<br>

Descobrir o PID de um processo. Após descoberto o PID, pode-se derrubar este processo utilizando o comando `kill "PID"`
```bash
pgrep "processo-exemplo"
```
<br>

Listar informações sobre o armazenamento da máquina
```bash
df -h
```
<br>

Utilitário que "scanneia" os arquivos e mostra quais diretórios/pastas mais ocupam espaço de armazenamento. Com ele também é possível apagar arquivos
```bash
ncdu
```
<br>

Mostrar informações do disco, no formato de “árvore”
```bash
lsblk
```
<br>

Descobrir a versão do kernel 
```bash
uname -r
```
<br>

Listar informações sobre o processador da máquina
```bash
lscpu
```
<br>

Listar informações sobre conexões/dispositivos USB
```bash
lsusb
```
<br>

Listar o que está se comunicando com as linhas PCI da máquina
```bash
lspci
```
<br>

Listar um histórico de comandos já utilizados no terminal
```bash
history
```
<br>

## Outros

- Para selecionar ou navegar entre diretórios de nome composto, utilizar `' '`
- Ctrl + L “limpa” o terminal. É um atalho para o comando `clear`
- Ctrl + C cancela o que está sendo processado no terminal
