# lista-ips

Script Python para varredura de IPs em uma rede, salvando resultados em CSV. Faz ping, resolve DNS e suporta Windows/Linux.

## Descrição

Este script realiza a varredura de uma rede IPv4, verifica quais IPs estão ativos (respondendo ao ping), resolve nomes DNS e salva os resultados em arquivos CSV. É compatível com Windows e Linux.

## Funcionalidades
- Varredura de todos os IPs de uma rede (ex: 192.168.1.0/24)
- Verificação de resposta ICMP (ping)
- Resolução de hostname e DNS reverso
- Resultados salvos em arquivos CSV (todos os IPs e apenas ativos)
- Execução paralela para maior velocidade

## Como usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/jacoisrael2/lista-ips.git
   cd lista-ips
   ```
2. Execute o script:
   ```bash
   python lista-ips.py
   ```
3. Siga as instruções no terminal para informar a rede a ser escaneada.

## Exemplo de uso
```
Digite a rede a ser verificada (ex: 192.168.1.0/24) ou 'sair' para encerrar: 192.168.1.0/24
```

## Requisitos
- Python 3.7+
- Permissão para executar ping no sistema

## Observações
- O script pode demorar em redes grandes.
- Em sistemas Unix/Linux, pode ser necessário rodar como sudo para ping ICMP.

## Licença
MIT
