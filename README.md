# Prometheus service-discovery with json file

Este playground possui o Prometheus e o node-exporter em um ***docker-compose***.

The Prometheus Node Exporter exposes a wide variety of hardware- and kernel-related metrics.

As configurações do Prometheus estão no arquivo: ***prometheus/prometheus-config.yaml***

Já as configurações de service-discovery para o node-experter estão no arquivo json: ***prometheus/targets.json***

### Instruções de execução:


* Execute: ***docker-compose up***


* Acesse o link para verificar o node-exporter: http://localhost:9100/metrics


* Acesse o link para verificar o Prometheus: http://localhost:9090/


* Acesse o link para verificar se o Prometheus conectou-se ao node-exporter: http://localhost:9090/targets?search=


* Execute queries no Prometheus: http://localhost:9090/graph?g0.expr=go_info&g0.tab=1&g0.display_mode=lines&g0.show_exemplars=0&g0.range_input=1h
 
