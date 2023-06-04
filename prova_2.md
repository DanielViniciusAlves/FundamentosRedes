# Resumo para prova de Redes dia 7 de Maio de 2023

## Camada de Redes 

1. Endereços IP

No contexto de Camada de Redes o IP serve para identificar um host ou um roteador. Teoricamente esse valor deveria ser único, não podendo haver mais de uma máquina com o mesmo endereço IP, além disso todos endereços IPs devem ter 32bits. Porém para evitar o esgotamento de enderços IPs dentro de uma rede (que possui um endereço IP único), é feito uma repetição de IPs dentro da rede, o que isso quer dizer? Quer dizer que dentro da sua rede de casa cada máquina conectada possui um endereço único, mas esse endereço pode ser repetido em outra rede.

**Importante lembrar que o endereço IP se refere não ao host, mas sim a interface de rede da máquina.**

1.1. Endereçamento de classe

Durante muito tempo foi usado categorias para poder alocar os tipos de rede possíveis, sendo definido cinco categorias. Esse tipo de alocação foi chamado de **Endereçamento de classe completo**. Nele são definidas as seguintes classes:

- Classe A:
    - Definida pelos endereços de 1.0.0.0 até 127.255.255.255.
- Classe B:
    - Definida pelos endereços de 128.0.0.0 até 191.255.255.255.
- Classe C:
    - Definida pelos endereços de 192.0.0.0 até 223.255.255.255.
- Classe D:
    - Definida pelos endereços de 224.0.0.0 até 239.255.255.255.
- Classe E:
    - Definida pelos endereços de 240.0.0.0 até 247.255.255.255.

**Importante notar que as classe vai possuir 32bits, ou seja 4 bytes. Que em notação decimal pode ser escrito indo de 0 a 255, como demonstrado acima.**

O endereço IP 0.0.0.0 é utilizado pelos hosts ao serem inicializados, além disso o a faixa de endereço: 127.x.x.x, é utilizada como loopcallback. Loopcallback é utilizado para processar localmente os pacotes sem ser necessário que o transmissor saiba o IP do host local.

1.2 Sub-redes


