Il presente repository contiene l'insieme dei manifest e dei file yaml necessari per il deploy di un'infrastruttura AiOps basata su microservizi.
Si riporta di seguito l'alberatura del repository: 


Modulo-AWX 

    |_ Deploy-Awx-Installation.yml
    |_ Deploy-Awx-Operator.yml
    |_ Deploy-Awx-ServiceAccount.yml
    
Modulo-Ansible-Automation-Platform

    |_ Deploy-Modulo-Ansible.yml
    |_ Playbook-Ansible
       |_ Block_IP.yml
       |_ Cleanup_Space.yml
       |_ DNS_Recovery.yml
       |_ Disk_Remount.yml
       |_ Kill_Process.yml
       |_ Manage_Swap.yml
       |_ Restart_Services.yml
       |_ Rotate_Logs.yml
Modulo-Dify-AI

    |_ Deploy-Modulo-AI-Engine.yml
    
Modulo-Grafana

    |_ Deploy-Grafana-Installation.yml
    |_ Deploy-Grafana-Prerequisites.yml
    |_ Deploy-Grafana-Service.yml

Modulo-Network

    |_ Configurazione-MetaLB.yml
    |_ Deploy-Ingress-Controller.yml
    |_ Load-Balancer.yml

Modulo-Storage-DIstribuito-Longhorn

    |_ Deploy-Storage-Class-Longhorn.yml

Modulo-Zabbix-Client

    |_ configure.yml
    |_ hosts.ini
    |_ install.yml
    |_ install_zabbix_agent.yml
    |_ update.yml
    |_ update_zabbix_agent.yml
    |_ zabbix_agent2.man
    |_ zabbix_agentd.man
    |_ zabbix_get.man

Modulo-Zabbix-Database

    |_ postgres-cluster.yml
    |_ postgres-pod.yml
    |_ Schema-Zabbix
       |_ Makefile.am
       |_ Makefile.in
       |_ data.sql
       |_ images.sql
       |_ schema.sql
Modulo-Zabbix-Front-End

    |_ Deploy-Zabbix-FrontEnd.yml
    |_ zabbix_web_service.man
Modulo-Zabbix-Server

    |_ Deploy-Zabbix-Server.yml
    |_ zabbix_sender.man
    |_ zabbix_server.conf
    |_ zabbix_server.man
