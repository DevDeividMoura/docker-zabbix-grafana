# Docker Zabbix-Grafana Compose

Este repositório contém um conjunto de configurações do Docker Compose para instalar e executar o Zabbix, Grafana e MySQL em contêineres Docker. O Zabbix é uma solução de monitoramento de rede de código aberto, enquanto o Grafana é uma plataforma de análise e visualização de métricas. O MySQL é utilizado como banco de dados para o Zabbix.

## Pré-requisitos

Antes de começar, você precisará ter o Docker e o Docker Compose instalados em sua máquina. Para instruções de instalação, consulte a documentação oficial do Docker:

- [Instalar Docker](https://docs.docker.com/get-docker/)

## Como Usar

Para colocar o Zabbix, Grafana e MySQL em funcionamento, siga estes passos:

1. **Clone o Repositório**

Primeiramente, clone este repositório para sua máquina local:

```bash
git clone https://github.com/DevDeividMoura/docker-zabbix-grafana.git
cd docker-zabbix-grafana
```

2. **Configure o Ambiente**

Revise o arquivo `docker-compose.yml` e ajuste as configurações de acordo com suas necessidades, especialmente as senhas do banco de dados e outras variáveis de ambiente.

3. **Inicie os Contêineres**

Execute o seguinte comando para iniciar todos os serviços definidos no arquivo Docker Compose:

```bash
docker compose up -d
```

4. **Acesse a Interface Web**

Após alguns momentos, você poderá acessar as interfaces web do Zabbix e do Grafana nos seguintes endereços:

- Zabbix: `http://localhost:8888`
- Grafana: `http://localhost:3000`

## Configuração

- **Zabbix**: A primeira vez que acessar o Zabbix, você precisará seguir o assistente de configuração na web para concluir a instalação.
- **Grafana**: Faça login no Grafana usando o usuário e senha padrões (`admin`/`admin`), e então conecte o Zabbix como fonte de dados usando as credenciais configuradas.

## Contribuindo

Sinta-se à vontade para forkar o repositório, fazer melhorias, e submeter pull requests. Estamos sempre abertos a melhorar este projeto.

## Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## Contato

Para dúvidas e sugestões, abra uma issue neste repositório ou entre em contato diretamente.
