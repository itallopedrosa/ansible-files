**ELK**
=========

Instalação elasticsearch, logstash e kibana com Ansible

**Variaveis**
--------------

Variaveis declaradas em default/main e vars/main    
    
**Dependências**
------------

Ambiente com Rhel/Debian disponibilizado.

Variaveis de instalação:

- elasticsearch
- logstash
- kibana
- rsyslogd

**Modo de execução**
----------------

Com usuário que possui chave entre os servidores executar da seguinte forma:

   $ ansible-playbook /etc/ansible/elk.yml
   
Via git:

   $ ansible-pull -f -C master -d /tmp -U git@gitlab.com:giulianocdomingues/elk.git elk.yml

A execução deste playbook realizará as seguintes ações:

- Atualizar Sistema Operacional;
- Instalar Dependencias para execução do projeto;
- Instalar e configurar elasticsearch 7.x;
- Instalar e configurar kibana 7.x;
- Instalar e configurar logstash 7.x;
- Instalar e configurar filebeat 7.x;
- Instalar e configurar rsyslog server;
- Instalar e configura o Apache;
- Iniciar os serviços e validar funcionamento;

**License**
-------

Elasticsearch-2

**Author Information**
------------

- [Giuliano Caixeta Domingues](@giulianocdomingues) - CentralIT
