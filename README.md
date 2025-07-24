# 📡 Monitoramento de Rede com Docker, Prometheus e Grafana

Este projeto fornece uma stack de monitoramento de rede utilizando **Docker**, **Prometheus**, **Grafana** e **Blackbox Exporter**, com dashboards customizados e provisionamento automático.

## 📦 Tecnologias Utilizadas

- [Docker](https://www.docker.com/)
- [Prometheus](https://prometheus.io/)
- [Grafana](https://grafana.com/)
- [Blackbox Exporter](https://github.com/prometheus/blackbox_exporter)
- [SNMP Exporter (opcional)](https://github.com/prometheus/snmp_exporter)
- [Zabbix Data Source for Grafana](https://grafana.com/grafana/plugins/alexanderzobnin-zabbix-app/)

---

## 🚀 Como Executar

### Pré-requisitos

- Docker e Docker Compose instalados

### Passos

1. Clone o repositório:

```bash
git clone https://github.com/BarretoEng/monitoramento-rede.git
cd monitoramento-rede
```

2. Suba os containers:

```
docker-compose up -d
```

3. Acesse o Grafana:
```
http://localhost:3000
```

### Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

