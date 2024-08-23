# Infra-Web CloudFormation Template

Questo repository contiene un template CloudFormation chiamato `infra-web.yaml` per creare l'infrastruttura necessaria a supportare un'applicazione web scalabile su AWS. Il template è scritto in formato YAML e automatizza la creazione delle risorse essenziali come VPC, Subnet, EC2 e Security Group.

## Descrizione del Template

Il template `infra-web.yaml` configura l'infrastruttura di base per un'applicazione web con le seguenti componenti:

- **VPC**: Una Virtual Private Cloud configurata per gestire il traffico di rete in modo sicuro.
- **Subnet Pubblica**: Una subnet pubblica che ospita l'istanza EC2, permettendo l'accesso dall'esterno.
- **Security Group**: Un security group che permette il traffico HTTP (porta 80), HTTPS (porta 443) e SSH (porta 22).
- **Istanza EC2**: Un'istanza EC2 configurata per ospitare un web server, come Nginx, per servire l'applicazione.
- **Internet Gateway**: Un gateway che consente alla VPC di connettersi a Internet.

## Come Usare il Template

### Usare la Console AWS

1. Accedi alla [console di CloudFormation](https://console.aws.amazon.com/cloudformation).
2. Clicca su **Create stack** e seleziona **With new resources (standard)**.
3. Scegli l'opzione **Upload a template file** e carica il file `infra-web.yaml`.
4. Segui i passaggi nella console per configurare eventuali parametri (se ce ne sono) e avviare lo stack.

### Usare l'AWS CLI

Se preferisci usare la CLI, puoi avviare lo stack con questo comando:

```bash
aws cloudformation create-stack --stack-name infra-web-stack --template-body file://infra-web.yaml --capabilities CAPABILITY_NAMED_IAM



### Cosa Include il Template YAML

Questo `README.md` riflette il template CloudFormation che avevo iniziato a descrivere in precedenza, il quale crea una VPC, subnet pubblica, istanza EC2, security group, internet gateway, e altro.

Se hai ulteriori domande o hai bisogno di aiuto per altre configurazioni, fammi sapere!
