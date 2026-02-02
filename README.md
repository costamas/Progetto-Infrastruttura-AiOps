Il presente repository contiene l'insieme dei manifest e dei file yaml necessari per il deploy di un'infrastruttura AiOps basata su microservizi.
Si riporta di seguito l'alberatura del repository: 


Modulo-AWX (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pods e dei services del modulo AWX).

    |_ Deploy-Awx-Installation.yml (Manifest per il rilascio e configurazione dei pods Kubernetes associati al modulo AWX). 
    |_ Deploy-Awx-Operator.yml (Manifest per il rilascio e configurazione dell'operator Kubernetes associato al modulo AWX). 
    |_ Deploy-Awx-ServiceAccount.yml (Manifest per il rilascio e configurazione dei ServiceAccount Kubernetes associati al modulo AWX). 
    
Modulo-Ansible-Automation-Platform (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pods e dei services del modulo Ansible Automation Platform).

    |_ Deploy-Modulo-Ansible.yml (Manifest per il rilascio e configurazione dei pods Kubernetes associati al modulo Ansible Automation Platform). 
    |_ Playbook-Ansible (Cartella contenente tutti i plybook Ansible necessari alla risoluzione automatica delle problematiche).
       |_ Block_IP.yml (Playbook Ansible per la gestione di problematiche relative a potenziali attacchi DDoS).
       |_ Cleanup_Space.yml (Playbook Ansible per la gestione di problematiche relative alla saturazione dello spazio disco).
       |_ DNS_Recovery.yml (Playbook Ansible per la gestione di problematiche relative alla risoluzione DNS).
       |_ Disk_Remount.yml (Playbook Ansible per la gestione di problematiche relative al mount dei dischi).
       |_ Kill_Process.yml (Playbook Ansible per la gestione di problematiche relative al blocco dei processi).
       |_ Manage_Swap.yml (Playbook Ansible per la gestione di problematiche relative alla Swap Memory).
       |_ Restart_Services.yml (Playbook Ansible per la gestione di problematiche relative al malfunzionamento di servizi).
       |_ Rotate_Logs.yml (Playbook Ansible per la gestione di problematiche relative alla rotazione dei logs).
Modulo-Dify-AI (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pods e dei services del modulo Dify-AI).

    |_ Deploy-Modulo-AI-Engine.yml (Manifest per il rilascio e configurazione deipodsPod Kubernetes associati al modulo Dify-AI). 
    
Modulo-Grafana (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pods e dei services del modulo Grafana).

    |_ Deploy-Grafana-Installation.yml (Manifest per il rilascio e configurazione dei pods Kubernetes associati al modulo Grafana).
    |_ Deploy-Grafana-Prerequisites.yml (Manifest per il rilascio e configurazione dei prerequisiti necessari al corretto deploy del modulo Grafana). 
    |_ Deploy-Grafana-Service.yml (Manifest per il rilascio e configurazione dei services associati al modulo Grafana). 

Modulo-Network (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pod e dei services del modulo di Networking e instradamento del routing tra i Pod).

    |_ Configurazione-MetaLB.yml (Manifest per il rilascio e configurazione dei pods Kubernetes associati al modulo di networking). 
    |_ Deploy-Ingress-Controller.yml (Manifest per il rilascio e configurazione dell'Ingress Controller Kubernetes per il corretto instradamento del traffico). 
    |_ Load-Balancer.yml (Manifest per il rilascio e configurazione dei pods Kubernetes associati al bilanciatore di rete in ingresso). 

Modulo-Storage-Distribuito-Longhorn (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pod e dei services del modulo di storage distribuito Longhorn).

    |_ Deploy-Storage-Class-Longhorn.yml (Manifest per il rilascio e configurazione dei pods Kubernetes associati al modulo di storage distribuito).

Modulo-Zabbix-Client (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pod e dei services del modulo Zabbix-Client).

    |_ configure.yml
    |_ hosts.ini
    |_ install.yml
    |_ install_zabbix_agent.yml
    |_ update.yml
    |_ update_zabbix_agent.yml
    |_ zabbix_agent2.man
    |_ zabbix_agentd.man
    |_ zabbix_get.man

Modulo-Zabbix-Database (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pod e dei services del modulo Zabbix-Database).

    |_ postgres-cluster.yml (Manifest per il rilascio e configurazione del cluster PostgreSQL con N°2 nodi - Master e Replica).
    |_ postgres-pod.yml (Manifest per il rilascio e configurazione dei pods Kubernetes associati al modulo di storage distribuito).
    |_ Schema-Zabbix (Cartella contenente gli script SQL per la configurazione iniziale del database 
       |_ data.sql (Script SQL per la corretta inizializzazione delle tabelle associate a Zabbix in PostgreSQL).
       |_ images.sql (Script SQL per la corretta inizializzazione delle tabelle associate a Zabbix in PostgreSQL).
       |_ schema.sql (Script SQL per la corretta inizializzazione delle tabelle associate a Zabbix in PostgreSQL).
       
Modulo-Zabbix-Front-End (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pod e dei services del modulo Zabbix-FrontEnd).

    |_ Deploy-Zabbix-FrontEnd.yml
    |_ zabbix_web_service.man
    
Modulo-Zabbix-Server (Insieme dei file .yml necessari al corretto rilascio e alla corretta configurazione dei pod e dei services del modulo Zabbix-Server).

    |_ Deploy-Zabbix-Server.yml
    |_ zabbix_sender.man
    |_ zabbix_server.conf
    |_ zabbix_server.man
