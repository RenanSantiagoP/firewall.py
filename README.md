Este é um script Python simples que simula a verificação de regras de um firewall. Ele gera endereços de IP aleatórios e verifica se eles devem ser permitidos ("allow") ou bloqueados ("block") 
com base em um conjunto pré-definido de regras.


Como Funciona:
O script principal executa um loop 12 vezes, realizando as seguintes ações em cada iteração:

Gera um IP Aleatório: A função generate_random_ip() cria um endereço de IP no intervalo de 192.168.10.0 a 192.168.10.20.

Define Regras: Um dicionário estático firewall_rules contém os IPs específicos que devem ser bloqueados.

Verifica o IP: A função check_firewall_rules() compara o IP gerado com a lista de regras.

Se o IP for encontrado na lista, a ação "block" é retornada.

Se o IP não for encontrado, a ação padrão "allow" é retornada.

Exibe o Resultado: O script imprime o IP testado, a ação (allow/block) e um número aleatório adicional.


Como Usar:
Pré-requisitos - Você precisa ter o Python 3 instalado em sua máquina.

Executando o Script
Salve o código em um arquivo (por exemplo, firewall.py).

Abra seu terminal ou prompt de comando.

Navegue até o diretório onde você salvou o arquivo.

Execute o script usando o comando:

Bash

python firewall.py
Exemplo de Saída
A saída será semelhante a esta (os IPs e números aleatórios mudarão a cada execução):

IP: 192.168.10.10, Action: block, Random: 4582

IP: 192.168.10.7, Action: allow, Random: 901

IP: 192.168.10.15, Action: block, Random: 7763

IP: 192.168.10.1, Action: allow, Random: 1234

IP: 192.168.10.4, Action: block, Random: 8842

IP: 192.168.10.18, Action: allow, Random: 3021
...
