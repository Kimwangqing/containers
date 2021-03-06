---

copyright:
  years: 2014, 2018
lastupdated: "2018-12-05"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:deprecated: .deprecated}
{:download: .download}





# Referência de CLI para gerenciar clusters
{: #cs_cli_reference}

Consulte esses comandos para criar e gerenciar clusters no {{site.data.keyword.Bluemix_notm}}.
{:shortdesc}

## ibmcloud ks commands
{: #cs_commands}

**Dica:** para ver a versão do plug-in do {{site.data.keyword.containerlong_notm}}, execute o comando a seguir.

```
ibmcloud plugin list
```
{: pre}



<table summary="API commands table">
<caption>Comandos de API</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos de API</th>
 </thead>
 <tbody>
  <tr>
    <td>[ibmcloud ks api](#cs_api)</td>
    <td>[ibmcloud ks api-key-info](#cs_api_key_info)</td>
    <td>[ibmcloud ks api-key-reset](#cs_api_key_reset)</td>
    <td>[ibmcloud ks apiserver-config-get](#cs_apiserver_config_get)</td>
  </tr>
  <tr>
    <td>[ibmcloud ks apiserver-config-set](#cs_apiserver_config_set)</td>
    <td>[ibmcloud ks apiserver-config-unset](#cs_apiserver_config_unset)</td>
    <td>[ibmcloud ks apiserver-refresh](#cs_apiserver_refresh)</td>
    <td></td>
 </tr>
</tbody>
</table>

<br>

<table summary="CLI plug-in usage commands table">
<caption>Comandos de uso do plug-in da CLI</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos de uso do plug-in da CLI</th>
 </thead>
 <tbody>
  <tr>
    <td>[ibmcloud ks help](#cs_help)</td>
    <td>[ibmcloud ks init](#cs_init)</td>
    <td>[ibmcloud ks messages](#cs_messages)</td>
    <td></td>
  </tr>
</tbody>
</table>

<br>

<table summary="Cluster commands: Management table">
<caption>Comandos do cluster: Gerenciamento de comandos</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos do cluster: gerenciamento</th>
 </thead>
 <tbody>
  <tr>
    <td>[ibmcloud ks cluster-config](#cs_cluster_config)</td>
    <td>[ibmcloud ks cluster-create](#cs_cluster_create)</td>
    <td>[ibmcloud ks cluster-feature-enable](#cs_cluster_feature_enable)</td>
    <td>[ibmcloud ks cluster-get](#cs_cluster_get)</td>
  </tr>
  <tr>
    <td>[ibmcloud ks cluster-rm](#cs_cluster_rm)</td>
    <td>[ibmcloud ks cluster-update](#cs_cluster_update)</td>
    <td>[ibmcloud ks clusters](#cs_clusters)</td>
    <td>[ibmcloud ks kube-versions](#cs_kube_versions)</td>
  </tr>
</tbody>
</table>

<br>

<table summary="Comandos de cluster: tabela de serviços e integrações">
<caption>Comandos do cluster: serviços e integrações comandos</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos do cluster: serviços e integrações</th>
 </thead>
 <tbody>
  <tr>
    <td>[ibmcloud ks cluster-service-bind](#cs_cluster_service_bind)</td>
    <td>[ibmcloud ks cluster-service-unbind](#cs_cluster_service_unbind)</td>
    <td>[ibmcloud ks cluster-services](#cs_cluster_services)</td>
    <td>[ibmcloud ks va](#cs_va)</td>
  </tr>
    <td>[ibmcloud ks webhook-create](#cs_webhook_create)</td>
  <tr>
  </tr>
</tbody>
</table>

</br>

<table summary="Cluster commands: Subnets table">
<caption>Comandos do cluster: Subnets comandos</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos do cluster: Subnets</th>
 </thead>
 <tbody>
  <tr>
    <td>[ibmcloud ks cluster-subnet-add](#cs_cluster_subnet_add)</td>
    <td>[ibmcloud ks cluster-subnet-create](#cs_cluster_subnet_create)</td>
    <td>[ibmcloud ks cluster-user-subnet-add](#cs_cluster_user_subnet_add)</td>
    <td>[ibmcloud ks cluster-user-subnet-rm](#cs_cluster_user_subnet_rm)</td>
  </tr>
  <tr>
    <td>[ibmcloud ks subnets](#cs_subnets)</td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
</tbody>
</table>

</br>

<table summary="Infrastructure commands table">
<caption>Comandos do cluster: Comandos de infraestrutura</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos de infraestrutura</th>
 </thead>
 <tbody>
  <tr>
    <td>[ibmcloud ks credential-set](#cs_credentials_set)</td>
    <td>[ibmcloud ks credential-unset](#cs_credentials_unset)</td>
    <td>[ibmcloud ks machine-types](#cs_machine_types)</td>
    <td>[ibmcloud ks vlans](#cs_vlans)</td>
  </tr>
</tbody>
</table>

</br>

<table summary="Tabela de comandos do balanceador de carga do aplicativo (ALB) de Ingresso">
<caption>Comandos do balanceador de carga do aplicativo (ALB) Ingress</caption>
<col width = 25%>
<col width = 25%>
<col width = 25%>
  <thead>
    <tr>
      <th colspan=4>Comandos do balanceador de carga do aplicativo (ALB) Ingress</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>[ibmcloud ks alb-cert-deploy](#cs_alb_cert_deploy)</td>
      <td>[ibmcloud ks alb-cert-get](#cs_alb_cert_get)</td>
      <td>[ibmcloud ks alb-cert-rm](#cs_alb_cert_rm)</td>
      <td>[ibmcloud ks alb-certs](#cs_alb_certs)</td>
    </tr>
    <tr>
      <td>[ibmcloud ks alb-configure](#cs_alb_configure)</td>
      <td>[ibmcloud ks alb-get](#cs_alb_get)</td>
      <td>[ibmcloud ks alb-types](#cs_alb_types)</td>
      <td>[ibmcloud ks albs](#cs_albs)</td>
    </tr>
  </tbody>
</table>

</br>

<table summary="Tabela de comandos de criação de log">
<caption>Comandos de criação de log</caption>
<col width = 25%>
<col width = 25%>
<col width = 25%>
  <thead>
    <tr>
      <th colspan=4>Comandos de criação de log</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>[ibmcloud ks logging-config-create](#cs_logging_create)</td>
      <td>[ibmcloud ks logging-config-get](#cs_logging_get)</td>
      <td>[ibmcloud ks logging-config-refresh](#cs_logging_refresh)</td>
      <td>[ibmcloud ks logging-config-rm](#cs_logging_rm)</td>
    </tr>
    <tr>
      <td>[ibmcloud ks logging-config-update](#cs_logging_update)</td>
      <td>[ibmcloud ks logging-filter-create](#cs_log_filter_create)</td>
      <td>[ibmcloud ks logging-filter-update](#cs_log_filter_update)</td>
      <td>[ibmcloud ks logging-filter-get](#cs_log_filter_view)</td>
    </tr>
    <tr>
      <td>[ibmcloud ks logging-filter-rm](#cs_log_filter_delete)</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

</br>

<table summary="Region commands table">
<caption>Comandos de região</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos de região</th>
 </thead>
 <tbody>
  <tr>
    <td>[ibmcloud ks zones](#cs_datacenters)</td>
    <td>[ibmcloud ks region](#cs_region)</td>
    <td>[ibmcloud ks region-set](#cs_region-set)</td>
    <td>[ibmcloud ks regions](#cs_regions)</td>
  </tr>
</tbody>
</table>

</br>

<table summary="Worker node commands table">
<caption>Comandos de nó do trabalhador</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos de nó do trabalhador</th>
 </thead>
 <tbody>
    <tr>
      <td>Descontinuado: [ibmcloud ks worker-add](#cs_worker_add)</td>
      <td>[ibmcloud ks worker-get](#cs_worker_get)</td>
      <td>[ibmcloud ks worker-reboot](#cs_worker_reboot)</td>
      <td>[ibmcloud ks worker-reload](#cs_worker_reload)</td>
    </tr>
    <tr>
      <td>[ibmcloud ks worker-rm](#cs_worker_rm)</td>
      <td>[ibmcloud ks worker-update](#cs_worker_update)</td>
      <td>[ibmcloud ks workers](#cs_workers)</td>
      <td>[ibmcloud ks worker-get](#cs_worker_get)</td>
    </tr>
    <tr>
      <td>[ibmcloud ks worker-reboot](#cs_worker_reboot)</td>
      <td>[ibmcloud ks worker-reload](#cs_worker_reload)</td>
      <td>[ibmcloud ks worker-rm](#cs_worker_rm)</td>
      <td>[ibmcloud ks workers](#cs_workers)</td>
    </tr>
  </tbody>
</table>

<table summary="Tabela de comandos do conjunto do trabalhador">
<caption>Comandos do conjunto do trabalhador</caption>
<col width="25%">
<col width="25%">
<col width="25%">
 <thead>
    <th colspan=4>Comandos do conjunto do trabalhador</th>
 </thead>
 <tbody>
    <tr>
      <td>[ibmcloud ks worker-pool-create](#cs_worker_pool_create)</td>
      <td>[ibmcloud ks worker-pool-get](#cs_worker_pool_get)</td>
      <td>[ibmcloud ks worker-pool-rebalance](#cs_rebalance)</td>
      <td>[ibmcloud ks worker-pool-resize](#cs_worker_pool_resize)</td>
    </tr>
    <tr>
      <td>[ibmcloud ks worker-pool-rm](#cs_worker_pool_rm)</td>
      <td>[ibmcloud ks worker-pools](#cs_worker_pools)</td>
      <td>[ibmcloud ks zone-add](#cs_zone_add)</td>
      <td>[ibmcloud ks zone-network-set](#cs_zone_network_set)</td>
    </tr>
    <tr>
     <td>[ibmcloud ks zone-rm](#cs_zone_rm)</td>
     <td></td>
    </tr>
  </tbody>
</table>

## Comandos de API
{: #api_commands}

### ibmcloud ks api ENDPOINT [--insecure][--skip-ssl-validation] [--api-version VALUE][-s]
{: #cs_api}

Destine o terminal da API para o {{site.data.keyword.containerlong_notm}}. Se você não especificar um terminal, será possível visualizar informações sobre o terminal atual que está destinado.

Alternando regiões? Use o comando `ibmcloud ks region-set` [](#cs_region-set) como alternativa.
{: tip}

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>ENDPOINT</em></code></dt>
   <dd>O terminal da API do  {{site.data.keyword.containerlong_notm}} . Observe que esse terminal é diferente dos terminais do {{site.data.keyword.Bluemix_notm}}. Este valor é necessário para configurar o terminal de API. Os valores aceitos são:<ul>
   <li>Terminal global: https://containers.bluemix.net</li>
   <li>Terminal Norte AP: https://ap-north.containers.bluemix.net</li>
   <li>Terminal Sul AP: https://ap-south.containers.bluemix.net</li>
   <li>Terminal da UE Central: https://eu-central.containers.bluemix.net</li>
   <li>Terminal Sul do Reino Unido: https://uk-south.containers.bluemix.net</li>
   <li>Terminal do leste dos EUA: https://us-east.containers.bluemix.net</li>
   <li>Terminal Sul dos EUA: https://us-south.containers.bluemix.net</li></ul>
   </dd>

   <dt><code>-- inseguro</code></dt>
   <dd>Permitir uma conexão HTTP insegura. Este sinalizador é opcional.</dd>

   <dt><code>--validation-skip-ssl</code></dt>
   <dd>Permitir certificados SSL insegura. Este sinalizador é opcional.</dd>

   <dt><code>-- api-version VALUE</code></dt>
   <dd>Especifique a versão da API do serviço que você deseja usar. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**: visualize informações sobre o terminal de API atual que é destinado.
```
ibmcloud ks api
```
{: pre}

```
API Endpoint:          https://containers.bluemix.net   
API Version:           v1   
Skip SSL Validation:   false   
Region:                us-south
```
{: screen}


### ibmcloud ks api-key-info CLUSTER  [ -- json ][-s]
{: #cs_api_key_info}

Visualize o nome e o endereço de e-mail para o proprietário da chave API do IAM em uma região do {{site.data.keyword.containerlong_notm}}.

A chave API do Identity and Access Management (IAM) é configurada automaticamente para uma região quando a primeira ação que requer a política de acesso de administrador do {{site.data.keyword.containerlong_notm}} é executada. Por exemplo, um dos seus usuários administradores cria o primeiro cluster na região `us-south`. Ao fazer isso, a chave API do IAM para esse usuário é armazenada na conta para essa região. A chave API é usada para pedir recursos na infraestrutura do IBM Cloud (SoftLayer), como nós do trabalhador novo ou VLANs.

Quando um usuário diferente executa uma ação nessa região que requer interação com o portfólio da infraestrutura do IBM Cloud (SoftLayer), como a criação de um novo cluster ou o recarregamento de um nó do trabalhador, a chave API armazenada é usada para determinar se existem permissões suficientes para executar essa ação. Para certificar-se de que as ações relacionadas à infraestrutura em seu cluster possam ser executadas com sucesso, designe a seus usuários administradores do {{site.data.keyword.containerlong_notm}} a política de acesso de infraestrutura **Superusuário**. Para obter mais informações, veja [Gerenciando o acesso de usuário](cs_users.html#infra_access).

Se você descobrir que é necessário atualizar a chave API que está armazenada para uma região, será possível fazer isso executando o comando [ibmcloud ks api-key-reset](#cs_api_key_reset). Esse comando requer a política de acesso de administrador do {{site.data.keyword.containerlong_notm}} e armazena a chave API do usuário que executa esse comando na conta.

**Dica:** a chave de API retornada nesse comando poderá não ser usada se as credenciais de infraestrutura do IBM Cloud (SoftLayer) tiverem sido configuradas manualmente usando o comando [ibmcloud ks credential-set](#cs_credentials_set).

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks api-key-info my_cluster
  ```
  {: pre}


### ibmcloud ks api-key-reset [-s]
{: #cs_api_key_reset}

Substitua a chave API do IAM atual em uma região do {{site.data.keyword.containerlong_notm}}.

Esse comando requer a política de acesso de administrador do {{site.data.keyword.containerlong_notm}} e armazena a chave API do usuário que executa esse comando na conta. A chave API do IAM é necessária para pedir infraestrutura do portfólio da infraestrutura do IBM Cloud (SoftLayer). Quando armazenada, a chave API é usada para cada ação em uma região que requer permissões de infraestrutura independentemente do usuário que executa esse comando. Para obter mais informações sobre como as chaves API do IAM funcionam, consulte o comando [`ibmcloud ks api-key-info`](#cs_api_key_info).

**Importante:** antes de usar esse comando, certifique-se de que o usuário que executa esse comando tenha as permissões necessárias do [{{site.data.keyword.containerlong_notm}} e de infraestrutura do IBM Cloud (SoftLayer)](cs_users.html#users).

<strong>Opções de comando</strong>:

   <dl>
   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>


**Exemplo**:

  ```
  ibmcloud ks api-key-reset
  ```
  {: pre}


### ibmcloud ks apiserver-config-get
{: #cs_apiserver_config_get}

Obtenha informações sobre uma opção para a configuração do servidor de API do Kubernetes de um cluster. Esse comando deve ser combinado com um dos subcomandos a seguir para a opção de configuração sobre a qual você deseja informações.

#### ibmcloud ks apiserver-config-get audit-webhook CLUSTER
{: #cs_apiserver_api_webhook_get}

Visualize a URL para o serviço de criação de log remoto para o qual você está enviando logs de auditoria do servidor de API. A URL foi especificada quando você criou o backend de webhook para a configuração do servidor de API.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks apiserver-config-get audit-webhook my_cluster
  ```
  {: pre}

### ibmcloud ks apiserver-config-set
{: #cs_apiserver_config_set}

Defina uma opção para a configuração do servidor da API do Kubernetes de um cluster. Esse comando deve ser combinado com um dos seguintes subcomandos para a opção de configuração que você deseja definir.

#### ibmcloud ks apiserver-config-set audit-webhook CLUSTER [--remoteServer SERVER_URL_OR_IP][--caCert CA_CERT_PATH] [--clientCert CLIENT_CERT_PATH][--clientKey CLIENT_KEY_PATH]
{: #cs_apiserver_api_webhook_set}

Configure o backend de webhook para a configuração do servidor de API. O backend de webhook encaminha os logs de auditoria do servidor de API para um servidor remoto. Uma configuração de webhook é criada com base nas informações fornecidas nas sinalizações desse comando. Se você não fornecer nenhuma informação nas sinalizações, uma configuração de webhook padrão será usada.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>--remoteServer <em>SERVER_URL</em></code></dt>
   <dd>A URL ou o endereço IP para o serviço de criação de log remoto para o qual deseja enviar logs de auditoria. Se você fornecer uma URL insegura do servidor, todos os certificados serão ignorados. Esse valor é opcional.</dd>

   <dt><code>--caCert <em>CA_CERT_PATH</em></code></dt>
   <dd>O caminho de arquivo para o certificado de autoridade de certificação que é usado para verificar o serviço de criação de log remoto. Esse valor é opcional.</dd>

   <dt><code>--clientCert <em>CLIENT_CERT_PATH</em></code></dt>
   <dd>O caminho de arquivo para o certificado de cliente que é usado para autenticar com relação ao serviço de criação de log remoto. Esse valor é opcional.</dd>

   <dt><code>--clientKey <em> CLIENT_KEY_PATH</em></code></dt>
   <dd>O caminho de arquivo para a chave do cliente correspondente que é usada para se conectar ao serviço de registro remoto. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks apiserver-config-set audit-webhook my_cluster --remoteServer https://audit.example.com/audit --caCert /mnt/etc/kubernetes/apiserver-audit/ca.pem --clientCert /mnt/etc/kubernetes/apiserver-audit/cert.pem --clientKey /mnt/etc/kubernetes/apiserver-audit/key.pem
  ```
  {: pre}


### ibmcloud ks apiserver-config-unset
{: #cs_apiserver_config_unset}

Desative uma opção para a configuração do servidor de API do Kubernetes de um cluster. Esse comando deve ser combinado com um dos subcomandos a seguir para a opção de configuração que você deseja desconfigurar.

#### ibmcloud ks apiserver-config-unset audit-webhook CLUSTER
{: #cs_apiserver_api_webhook_unset}

Desativar a configuração de backend do webhook para o servidor de API do cluster. A desativação do backend do webhook para o encaminhamento de logs de auditoria do servidor de API para um servidor remoto.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks apiserver-config-unset audit-webhook my_cluster
  ```
  {: pre}

### ibmcloud ks apiserver-refresh CLUSTER [ -s ]
{: #cs_apiserver_refresh}

Reinicie o mestre do Kubernetes no cluster para aplicar as mudanças na configuração do servidor de API.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks apiserver-refresh my_cluster
  ```
  {: pre}


<br />


## Comandos de uso do plug-in da CLI
{: #cli_plug-in_commands}

### ibmcloud ks help
{: #cs_help}

Visualizar uma lista de comandos e parâmetros suportados.

<strong>Opções de comando</strong>:

   Nenhuma

**Exemplo**:

  ```
  ibmcloud ks help
  ```
  {: pre}


### ibmcloud ks init [--host HOST][--insecure] [-p][-u] [-s]
{: #cs_init}

Inicialize o plug-in do {{site.data.keyword.containerlong_notm}} ou especifique a região em que você deseja criar ou acessar clusters do Kubernetes.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code>--host <em>HOST</em></code></dt>
   <dd>O  {{site.data.keyword.containerlong_notm}}  terminal de API a ser usado.  Esse valor é opcional. [Visualize os valores de terminal de API disponíveis.](cs_regions.html#container_regions)</dd>

   <dt><code>-- inseguro</code></dt>
   <dd>Permitir uma conexão HTTP insegura.</dd>

   <dt><code>-p</code></dt>
   <dd>Sua senha do IBM Cloud.</dd>

   <dt><code>-u</code></dt>
   <dd>O IBM Cloud username.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:


```
ibmcloud ks init --host https://uk-south.containers.bluemix.net
```
{: pre}


### ibmcloud ks messages
{: #cs_messages}

Visualize as mensagens atuais para o usuário do IBMid.

**Exemplo**:

```
ibmcloud ks messages
```
{: pre}


<br />


## Comandos do cluster: gerenciamento
{: #cluster_mgmt_commands}


### ibmcloud ks cluster-config CLUSTER  [ -- admin ][--export]  [ -s ][--yaml]
{: #cs_cluster_config}

Após efetuar login, faça download dos dados de configuração e certificados do Kubernetes para se conectar ao seu cluster e execute comandos `kubectl`. Os arquivos são transferidos por download em `user_home_directory/.bluemix/plugins/container-service/clusters/<cluster_name>`.

**Opções de comando**:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>--admin</code></dt>
   <dd>Faça download dos certificados TLS e dos arquivos de permissão para a função de Super usuário. É possível usar os certificados para automatizar tarefas em um cluster sem precisar autenticar novamente. Os arquivos são transferidos por download para `<user_home_directory>/.bluemix/plugins/container-service/clusters/<cluster_name>-admin`. Esse valor é opcional.</dd>

   <dt><code>--export</code></dt>
   <dd>Faça download dos dados de configuração e certificados do Kubernetes sem nenhuma mensagem diferente do comando de exportação. Como nenhuma mensagem é exibida, é possível usar essa sinalização quando você cria scripts automatizados. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

  <dt><code>--yaml</code></dt>
  <dd>Imprime a saída de comando em formato YAML. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

```
ibmcloud ks cluster-config my_cluster
```
{: pre}


### ibmcloud ks cluster-create [--file FILE_LOCATION][--hardware HARDWARE] --zone ZONE --machine-type MACHINE_TYPE --name NAME [--kube-version MAJOR.MINOR.PATCH][--no-subnet] [--private-vlan PRIVATE_VLAN][--public-vlan PUBLIC_VLAN] [--workers WORKER][--disable-disk-encrypt] [--trusted][-s]
{: #cs_cluster_create}

Crie um cluster em sua organização. Para clusters gratuitos, você especifica o nome do cluster; tudo o mais é configurado com um valor padrão. Um cluster grátis é excluído automaticamente após 30 dias. É possível ter um cluster grátis de cada vez. Para aproveitar os recursos integrais do Kubernetes, crie um cluster padrão.

<strong>Opções de comandos</strong>

<dl>
<dt><code>--file <em>FILE_LOCATION</em></code></dt>

<dd>O caminho para o arquivo YAML para criar seu cluster padrão. Em vez de definir as características de seu cluster usando as opções fornecidas nesse comando, será possível usar um arquivo YAML.  Esse valor é opcional para clusters padrão e não está disponível para clusters livres.

<p><strong>Nota:</strong> se você fornecer a mesma opção no comando como parâmetro no arquivo YAML, o valor no comando terá precedência sobre o valor no YAML. Por exemplo, você define um local em seu arquivo do YAML e usa a opção <code>--zone</code> no comando; o valor inserido nessa opção substitui o valor no arquivo do YAML.

<pre class="codeblock">
<code>name: <em>&lt;cluster_name&gt;</em>
zone: <em>&lt;zone&gt;</em>
no-subnet: <em>&lt;no-subnet&gt;</em>
machine-type: <em>&lt;machine_type&gt;</em>
private-vlan: <em>&lt;private_VLAN&gt;</em>
public-vlan: <em>&lt;public_VLAN&gt;</em>
hardware: <em>&lt;shared_or_dedicated&gt;</em>
workerNum: <em>&lt;number_workers&gt;</em>
kube-version: <em>&lt;kube-version&gt;</em>
diskEncryption: <em>false</em>
trusted: <em>true</em>
</code></pre>


<table>
    <caption>Entendendo os componentes de arquivo YAML</caption>
    <thead>
    <th colspan=2><img src="images/idea.png" alt="Ícone de ideia"/> entendendo os componentes de arquivo do YAML</th>
    </thead>
    <tbody>
    <tr>
    <td><code><em>name</em></code></td>
    <td>Substitua <code><em>&lt;cluster_name&gt;</em></code> por um nome para seu cluster. O nome deve iniciar com uma letra, pode conter letras, números e hífen (-) e deve ter 35 caracteres ou menos. O nome do cluster e a região na qual o cluster está implementado formam o nome completo do domínio para o subdomínio do Ingress. Para assegurar que o subdomínio do Ingress seja exclusivo dentro de uma região, o nome do cluster pode ser truncado e anexado com um valor aleatório dentro do nome de domínio do Ingress.
</td>
    </tr>
    <tr>
    <td><code><em>zone</em></code></td>
    <td>Substitua <code><em>&lt;zone&gt;</em></code> pela zona na qual você deseja criar o seu cluster. As zonas disponíveis são dependentes da região na qual você efetuou login. Para listar as zonas disponíveis, execute <code>ibmcloud ks zones</code>. </td>
     </tr>
     <tr>
     <td><code><em>no-subnet</em></code></td>
     <td>Por padrão, uma sub-rede móvel pública e uma privada são criadas na VLAN associada ao cluster. Substitua <code><em>&lt;no-subnet&gt;</em></code> por <code><em>true</em></code> para evitar a criação de sub-redes com o cluster. É possível [criar](#cs_cluster_subnet_create) ou [incluir](#cs_cluster_subnet_add) sub-redes em um cluster posteriormente.</td>
      </tr>
     <tr>
     <td><code><em>machine-type</em></code></td>
     <td>Substitua <code><em>&lt;machine_type&gt;</em></code> pelo tipo de máquina na qual você deseja implementar os nós do trabalhador. É possível implementar os nós do trabalhador como máquinas virtuais em hardware compartilhado ou dedicado ou como máquinas físicas no bare metal. Os tipos de máquinas físicas e virtuais disponíveis variam de acordo com a zona na qual você implementa o cluster. Para obter mais informações, consulte a documentação para o comando `ibmcloud ks machine-type` [](cs_cli_reference.html#cs_machine_types).</td>
     </tr>
     <tr>
     <td><code><em>private-vlan</em></code></td>
     <td>Substitua <code><em>&lt;private_VLAN&gt;</em></code> pelo ID da VLAN privada que você deseja usar para os seus nós do trabalhador. Para listar VLANs disponíveis, execute <code>ibmcloud ks vlans <em>&lt;zone&gt;</em></code> e procure roteadores de VLAN que iniciem com <code>bcr</code> (roteador de backend).</td>
     </tr>
     <tr>
     <td><code><em>public-vlan</em></code></td>
     <td>Substitua <code><em>&lt;public_VLAN&gt;</em></code> pelo ID da VLAN pública que você deseja usar para os seus nós do trabalhador. Para listar VLANs disponíveis, execute <code>ibmcloud ks vlans <em>&lt;zone&gt;</em></code> e procure roteadores de VLAN que iniciem com <code>fcr</code> (roteador de front-end).</td>
     </tr>
     <tr>
     <td><code><em>hardware</em></code></td>
     <td>Para tipos de máquinas virtuais: o nível de isolamento de hardware para seu nó do trabalhador. Use dedicated se desejar que os recursos físicos disponíveis sejam dedicados somente a você ou shared para permitir que os recursos físicos sejam compartilhados com outros clientes IBM. O padrão é <code>shared</code>.</td>
     </tr>
     <tr>
     <td><code><em>workerNum</em></code></td>
     <td>Substitua <code><em>&lt;number_workers&gt;</em></code> pelo número de nós do trabalhador que você deseja implementar.</td>
     </tr>
     <tr>
      <td><code><em>kube-version</em></code></td>
      <td>A versão do Kubernetes para o nó principal do cluster. Esse valor é opcional. Quando a versão não for especificada, o cluster será criado com o padrão de versões do Kubernetes suportadas. Para ver as versões disponíveis, execute <code>ibmcloud ks kube-versions</code>.
</td></tr>
      <tr>
      <td><code>diskEncryption: <em>false</em></code></td>
      <td>Nós do trabalhador apresentam criptografia de disco por padrão; [saiba mais](cs_secure.html#encrypted_disk). Para desativar a criptografia, inclua essa opção e configure o valor para <code>false</code>.</td></tr>
      <tr>
      <td><code>trusted: <em>true</em></code></td>
      <td>**Somente bare metal**: ative [Cálculo confiável](cs_secure.html#trusted_compute) para verificar os nós do trabalhador do bare metal com relação à violação. Se você não ativar a confiança durante a criação do cluster, mas desejar posteriormente, será possível usar o comando `ibmcloud ks feature-enable` [](cs_cli_reference.html#cs_cluster_feature_enable). Depois de ativar a confiança, não é possível desativá-la posteriormente.</td></tr>
     </tbody></table>
    </p></dd>

<dt><code>--hardware <em>HARDWARE</em></code></dt>
<dd>O nível de isolamento de hardware para seu nó do trabalhador. Use dedicado para disponibilizar recursos físicos disponíveis apenas para você ou compartilhado para permitir que os recursos físicos sejam compartilhados com outros clientes da IBM. O padrão é shared.  Esse valor é opcional para clusters padrão e não está disponível para clusters livres.</dd>

<dt><code>--zone <em>ZONE</em></code></dt>
<dd>A zona na qual você deseja criar o cluster. As zonas disponíveis para você dependem da região do {{site.data.keyword.Bluemix_notm}} na qual você está com login efetuado. Selecione a região fisicamente mais próxima de você para melhor desempenho.  Esse valor é necessário para clusters padrão e opcional para clusters livres.

<p>Revise [zonas disponíveis](cs_regions.html#zones).</p>

<p><strong>Nota:</strong> quando você seleciona uma zona que está localizada fora de seu país, tenha em mente que você pode precisar de autorização legal antes que os dados possam ser armazenados fisicamente em um país estrangeiro.</p>
</dd>

<dt><code>--machine-type <em>MACHINE_TYPE</em></code></dt>
<dd>Escolha um tipo de máquina. É possível implementar os nós do trabalhador como máquinas virtuais em hardware compartilhado ou dedicado ou como máquinas físicas no bare metal. Os tipos de máquinas físicas e virtuais disponíveis variam de acordo com a zona na qual você implementa o cluster. Para obter mais informações, consulte a documentação para o comando `ibmcloud ks machine-types` [](cs_cli_reference.html#cs_machine_types). Esse valor é necessário para clusters padrão e não está disponível para clusters livres.</dd>

<dt><code>--name <em>NAME</em></code></dt>
<dd>O nome para o cluster.  Este valor é obrigatório. O nome deve iniciar com uma letra, pode conter letras, números e hífen (-) e deve ter 35 caracteres ou menos. O nome do cluster e a região na qual o cluster está implementado formam o nome completo do domínio para o subdomínio do Ingress. Para assegurar que o subdomínio do Ingress seja exclusivo dentro de uma região, o nome do cluster pode ser truncado e anexado com um valor aleatório dentro do nome de domínio do Ingress.
</dd>

<dt><code>--kube-version <em>MAJOR.MINOR.PATCH</em></code></dt>
<dd>A versão do Kubernetes para o nó principal do cluster. Esse valor é opcional. Quando a versão não for especificada, o cluster será criado com o padrão de versões do Kubernetes suportadas. Para ver as versões disponíveis, execute <code>ibmcloud ks kube-versions</code>.
</dd>

<dt><code>--no-subnet</code></dt>
<dd>Por padrão, uma sub-rede móvel pública e uma privada são criadas na VLAN associada ao cluster. Inclua a sinalização <code>--no-subnet</code> para evitar a criação de sub-redes com o cluster. É possível [criar](#cs_cluster_subnet_create) ou [incluir](#cs_cluster_subnet_add) sub-redes em um cluster posteriormente.</dd>

<dt><code>--private-vlan <em>PRIVATE_VLAN</em></code></dt>
<dd>

<ul>
<li>Esse parâmetro não está disponível para clusters livres.</li>
<li>Se esse cluster padrão for o primeiro cluster padrão que você criar nessa zona, não inclua essa sinalização. Uma VLAN privada é criada para você quando o cluster é criado.</li>
<li>Se você criou um cluster padrão antes nessa zona ou criou uma VLAN privada na infraestrutura do IBM Cloud (SoftLayer) antes, deverá especificar essa VLAN privada.

<p><strong>Nota:</strong> os roteadores de VLAN privada sempre iniciam com <code>bcr</code> (roteador de backend) e os roteadores de VLAN pública sempre iniciam com <code>fcr</code> (roteador de front-end). Ao criar um cluster e especificar as VLANs públicas e privadas, o número e a combinação de letras após esses prefixos devem corresponder.</p></li>
</ul>

<p>Para descobrir se você já tem uma VLAN privada para uma zona específica ou para localizar o nome de uma VLAN privada existente, execute <code>ibmcloud ks vlans <em>&lt;zone&gt;</em></code>.</p></dd>

<dt><code>--public-vlan <em>PUBLIC_VLAN</em></code></dt>
<dd>
<ul>
<li>Esse parâmetro não está disponível para clusters livres.</li>
<li>Se esse cluster padrão for o primeiro cluster padrão que você criar nessa zona, não use essa sinalização. Uma VLAN pública é criada para você quando o cluster é criado.</li>
<li>Se você criou um cluster padrão antes nessa zona ou criou uma VLAN pública na infraestrutura do IBM Cloud (SoftLayer) antes, especifique essa VLAN pública. Se você deseja conectar seus nós do trabalhador somente a uma VLAN privada, não especifique esta opção.

<p><strong>Nota:</strong> os roteadores de VLAN privada sempre iniciam com <code>bcr</code> (roteador de backend) e os roteadores de VLAN pública sempre iniciam com <code>fcr</code> (roteador de front-end). Ao criar um cluster e especificar as VLANs públicas e privadas, o número e a combinação de letras após esses prefixos devem corresponder.</p></li>
</ul>

<p>Para descobrir se você já tem uma VLAN pública para uma zona específica ou para localizar o nome de uma VLAN pública existente, execute <code>ibmcloud ks vlans <em>&lt;zone&gt;</em></code>.</p></dd>



<dt><code>--workers WORKER</code></dt>
<dd>O número de nós do trabalhador que
você deseja implementar em seu cluster. Se não
especificar essa opção, um cluster com 1 nó do trabalhador será criado. Esse valor é opcional para clusters padrão e não está disponível para clusters livres.

<p><strong>Nota:</strong> a cada nó do trabalhador é designado um ID de nó do trabalhador e um nome de domínio exclusivos que não devem ser mudados manualmente após a criação do cluster. Mudar o ID ou o nome do domínio evita que o mestre do Kubernetes gerencie o cluster.</p></dd>

<dt><code>--disable-disk-encrypt</code></dt>
<dd>Nós do trabalhador apresentam criptografia de disco por padrão; [saiba mais](cs_secure.html#encrypted_disk). Para desativar a criptografia, inclua essa opção.</dd>

<dt><code>--trusted</code></dt>
<dd><p>**Somente bare metal**: ative [Cálculo confiável](cs_secure.html#trusted_compute) para verificar os nós do trabalhador do bare metal com relação à violação. Se você não ativar a confiança durante a criação do cluster, mas desejar posteriormente, será possível usar o comando `ibmcloud ks feature-enable` [](cs_cli_reference.html#cs_cluster_feature_enable). Depois de ativar a confiança, não é possível desativá-la posteriormente.</p>
<p>Para verificar se o tipo de máquina bare metal suporta confiança, verifique o campo `Trustable` na saída do `ibmcloud ks machine-types <zone>` [Comando](#cs_machine_types). Para verificar se um cluster está ativado para confiança, visualize o campo **Pronto para confiança** na saída do comando `ibmcloud ks cluster-get` [](#cs_cluster_get). Para verificar se um nó do trabalhador bare metal está ativado para confiança, visualize o campo **Confiança** na saída do comando `ibmcloud ks worker-get` [](#cs_worker_get).</p></dd>

<dt><code>-s</code></dt>
<dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Exemplos**:

  

  **Criar um cluster grátis**: especifique somente o nome do cluster, todo o resto é configurado para um valor padrão. Um cluster grátis é excluído automaticamente após 30 dias. É possível ter um cluster grátis de cada vez. Para aproveitar os recursos integrais do Kubernetes, crie um cluster padrão.

  ```
  ibmcloud ks cluster-create --name my_cluster
  ```
  {: pre}

  **Criar o seu primeiro cluster padrão**: o primeiro cluster padrão que é criado em uma zona também cria uma VLAN privada. Portanto, não inclua a sinalização `--public-vlan`.
  {: #example_cluster_create}

  ```
  ibmcloud ks cluster-create --zone dal10 --private-vlan my_private_VLAN_ID --machine-type b2c.4x16 --name my_cluster --hardware shared --workers 2
  ```
  {: pre}

  **Criar clusters padrão subsequentes**: se você já criou um cluster padrão nessa zona ou criou uma VLAN pública na infraestrutura do IBM Cloud (SoftLayer) antes, especifique essa VLAN pública com a sinalização `--public-vlan`. Para descobrir se você já tem uma VLAN pública para uma zona específica ou para localizar o nome de uma VLAN pública existente, execute `ibmcloud ks vlans <zone>`.

  ```
  ibmcloud ks cluster-create --zone dal10 --public-vlan my_public_VLAN_ID --private-vlan my_private_VLAN_ID --machine-type b2c.4x16 --name my_cluster --hardware shared --workers 2
  ```
  {: pre}

  **Crie um cluster em um {{site.data.keyword.Bluemix_dedicated_notm}} ambiente**:

  ```
  ibmcloud ks cluster-create --machine-type machine-type --workers number --name cluster_name
  ```
  {: pre}

### ibmcloud ks cluster-feature-enable [ -f ] CLUSTER  [ -- trusted ][-s]
{: #cs_cluster_feature_enable}

Ative um recurso em um cluster existente.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>-f</code></dt>
   <dd>Use esta opção para forçar a opção <code>--trusted</code> sem prompts de usuário. Esse valor é opcional.</dd>

   <dt><code><em>--trusted</em></code></dt>
   <dd><p>Inclua a sinalização para ativar o [Cálculo confiável](cs_secure.html#trusted_compute) para todos os nós do trabalhador bare metal suportados que estiverem no cluster. Depois de ativar a confiança, não é possível desativá-la posteriormente para o cluster.</p>
   <p>Para verificar se o tipo de máquina bare metal suporta confiança, verifique o campo **Confiável** na saída do `ibmcloud ks machine-types <zone>` [Comando](#cs_machine_types). Para verificar se um cluster está ativado para confiança, visualize o campo **Pronto para confiança** na saída do comando `ibmcloud ks cluster-get` [](#cs_cluster_get). Para verificar se um nó do trabalhador bare metal está ativado para confiança, visualize o campo **Confiança** na saída do comando `ibmcloud ks worker-get` [](#cs_worker_get).</p></dd>

  <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Comando de exemplo**:

  ```
  ibmcloud ks cluster-feature-enable my_cluster -- trusted=true
  ```
  {: pre}

### ibmcloud ks cluster-get CLUSTER  [ -- json ][--showResources]  [ -s ]
{: #cs_cluster_get}

Visualizar informações sobre um cluster em sua organização.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

   <dt><code><em>--showResources</em></code></dt>
   <dd>Mostre mais recursos de cluster, como complementos, VLANs, sub-redes e armazenamento.</dd>


  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>



**Comando de exemplo**:

  ```
  ibmcloud ks cluster-get my_cluster --showResources
  ```
  {: pre}

**Saída de exemplo**:

  ```
  Name:                 my_cluster
  ID:                   abc1234567
  State:                normal
  Trust ready:          false
  Created:              2018-01-01T17:19:28+0000
  Zone:                 dal10
  Master URL:           https://169.xx.xxx.xxx:xxxxx
  Master Location:      Dallas
  Ingress subdomain:    my_cluster.us-south.containers.appdomain.cloud
  Ingress secret:       my_cluster
  Workers:              3
  Worker Zones:         dal10
  Version:              1.12.3
  Owner:                name@example.com
  Monitoring dashboard: https://metrics.ng.bluemix.net/app/#/grafana4/dashboard/db/link
  Resource Group ID:    a8a12accd63b437bbd6d58fb6a462ca7
  Resource Group Name:  Default

  Addons
  Name                   Enabled
  customer-storage-pod   true
  basic-ingress-v2       true
  storage-watcher-pod    true

  Subnet VLANs VLAN ID Subnet CIDR Public User-managed 2234947 10.xxx.xx.xxx/29 false false 2234945 169.xx.xxx.xxx/29 true false

  ```
  {: screen}

### ibmcloud ks cluster-rm [ -f ] CLUSTER [ -s ]
{: #cs_cluster_rm}

Remover um cluster de sua organização.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>-f</code></dt>
   <dd>Use esta opção para forçar a remoção de um cluster sem avisos do usuário. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-rm my_cluster
  ```
  {: pre}


### ibmcloud ks cluster-update [-f] CLUSTER [--kube-version MAJOR.MINOR.PATCH][--force-update] [-s]
{: #cs_cluster_update}

Atualize o mestre do Kubernetes para a versão de API padrão. Durante a atualização, não é possível acessar nem mudar o cluster. Nós do trabalhador, apps e recursos que foram implementados pelo usuário não são modificados e continuam a ser executados.

Pode ser necessário mudar seus arquivos YAML para implementações futuras. Revise essa [nota sobre a liberação](cs_versions.html) para obter detalhes.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>--kube-version <em>MAJOR.MINOR.PATCH</em></code></dt>
   <dd>A versão do Kubernetes do cluster. Se você não especificar uma versão, o mestre do Kubernetes será atualizado para a versão de API padrão. Para ver as versões disponíveis, execute [ibmcloud ks kube-versions](#cs_kube_versions). Esse valor é opcional.</dd>

   <dt><code>-f</code></dt>
   <dd>Use esta opção para forçar a atualização do mestre sem avisos do usuário. Esse valor é opcional.</dd>

   <dt><code>--force-update</code></dt>
   <dd>Tente a atualização mesmo se a mudança for maior que duas versões secundárias. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-update my_cluster
  ```
  {: pre}


### ibmcloud ks clusters [--json][-s]
{: #cs_clusters}

Visualizar uma lista de clusters em sua organização.

<strong>Opções de comando</strong>:

  <dl>
  <dt><code>--json</code></dt>
  <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

**Exemplo**:

  ```
  ibmcloud ks clusters
  ```
  {: pre}


### ibmcloud ks kube-versions [--json][-s]
{: #cs_kube_versions}

Visualize uma lista de versões do Kubernetes suportadas no {{site.data.keyword.containerlong_notm}}. Atualize o seu [cluster mestre](#cs_cluster_update) e [nós do trabalhador](cs_cli_reference.html#cs_worker_update) para a versão padrão para os recursos mais recentes, estáveis.

**Opções de comando**:

  <dl>
  <dt><code>--json</code></dt>
  <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

**Exemplo**:

  ```
  ibmcloud ks kube-versions
  ```
  {: pre}

<br />



## Comandos do cluster: serviços e integrações
{: #cluster_services_commands}


### ibmcloud ks cluster-service-bind CLUSTER KUBERNETES_NAMESPACE SERVICE_INSTANCE_NAME [-s]
{: #cs_cluster_service_bind}

Inclua um serviço do {{site.data.keyword.Bluemix_notm}} em um cluster. Para visualizar os serviços do {{site.data.keyword.Bluemix_notm}} disponíveis por meio do catálogo do {{site.data.keyword.Bluemix_notm}}, execute `ibmcloud service offerings`. **Nota**: é possível incluir somente serviços do {{site.data.keyword.Bluemix_notm}} que suportam chaves de serviço.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code><em>KUBERNETES_NAMESPACE</em></code></dt>
   <dd>O nome do namespace do Kubernetes. Este valor é obrigatório.</dd>

   <dt><code><em>SERVICE_INSTANCE_NAME</em></code></dt>
   <dd>O nome da instância de serviço do {{site.data.keyword.Bluemix_notm}} que você deseja ligar. Para localizar o nome de sua instância de serviço, execute <code>ibmcloud service list</code>. Se mais de uma instância tiver o mesmo nome na conta, use o ID da instância de serviço no lugar do nome. Para localizar o ID, execute <code>ibmcloud service show <service instance name> --guid</code>. Um desses valores é necessário.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-service-bind my_cluster my_namespace my_service_instance
  ```
  {: pre}


### ibmcloud ks cluster-service-unbind CLUSTER KUBERNETES_NAMESPACE SERVICE_INSTANCE_GUID [-s]
{: #cs_cluster_service_unbind}

Remova um serviço do {{site.data.keyword.Bluemix_notm}} de um cluster.

**Nota:** ao remover um serviço do {{site.data.keyword.Bluemix_notm}}, as credenciais de serviço serão removidas do cluster. Se um pod ainda está usando o serviço,
ele falha porque as credenciais de serviço não podem ser localizadas.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code><em>KUBERNETES_NAMESPACE</em></code></dt>
   <dd>O nome do namespace do Kubernetes. Este valor é obrigatório.</dd>

   <dt><code><em>SERVICE_INSTANCE_GUID</em></code></dt>
   <dd>O ID da instância de serviço do {{site.data.keyword.Bluemix_notm}} que você deseja remover. Para localizar o ID da instância de serviço, execute `ibmcloud ks cluster-services <cluster_name_or_ID>`.Esse valor é necessário.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-service-unbind my_cluster my_namespace 8567221
  ```
  {: pre}


### ibmcloud ks cluster-services CLUSTER [--namespace KUBERNETES_NAMESPACE][--all-namespaces] [--json][-s]
{: #cs_cluster_services}

Listar os serviços que estão ligados a um ou todos os namespaces do Kubernetes em um cluster. Se nenhuma
opção é especificada, os serviços para o namespace padrão são exibidos.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>--namespace <em>KUBERNETES_NAMESPACE</em></code>, <code>-n <em>KUBERNETES_NAMESPACE</em></code></dt>
   <dd>Inclua os serviços que forem limitados a um namespace específico em um cluster. Esse valor é opcional.</dd>

   <dt><code>--all-namespaces</code></dt>
   <dd>Inclua os serviços que forem limitados a todos os namespaces em um cluster. Esse valor é opcional.</dd>

   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-services my_cluster -- namespace my_namespace
  ```
  {: pre}

### ibmcloud ks va CONTAINER_ID [--extended][--vulnerabilities] [--configuration-issues][--json]
{: #cs_va}

Após você [instalar o scanner de contêiner](/docs/services/va/va_index.html#va_install_container_scanner), visualize um relatório de avaliação de vulnerabilidade detalhado para um contêiner em seu cluster.

**Opções de comando**:

<dl>
<dt><code> CONTAINER_ID </code></dt>
<dd><p>O ID do contêiner. Este valor é obrigatório.</p>
<p>Para localizar o ID de seu contêiner:<ol><li>[Direcione a CLI do Kubernetes para o seu cluster](cs_cli_install.html#cs_cli_configure).</li><li>Liste os seus pods executando `kubectl get pods`.</li><li>Localize o campo **ID do contêiner** na saída do comando `kubectl describe pod <pod_name>`. Por exemplo, `Container ID: docker://1a11a1aa2b2b22223333c44444ccc555667d7dd777888e8ef99f1011121314g15`.</li><li>Remova o prefixo `docker://` do ID antes de usar o ID do contêiner para o comando `ibmcloud ks va`. Por exemplo, `1a11a1aa2b2b22223333c44444ccc555667d7dd777888e8ef99f1011121314g15`.</li></ol></p></dd>

<dt><code>--extended</code></dt>
<dd><p>Estenda a saída de comando para mostrar mais informações de correção para pacotes vulneráveis. Esse valor é opcional.</p>
<p>Por padrão, os resultados da varredura mostram o ID, o status da política, os pacotes afetados e o modo de resolver. Com a sinalização `--extended`, isso inclui informações como o resumo, o aviso de segurança do fornecedor e o link de aviso oficial.</p></dd>

<dt><code>--vulnerabilities</code></dt>
<dd>Restrinja a saída de comando para mostrar apenas as vulnerabilidades do pacote. Esse valor é opcional. Não será possível usar essa sinalização se você usar a sinalização `--configuration-issues`.</dd>

<dt><code>--configuration-issues</code></dt>
<dd>Restrinja a saída de comando para mostrar apenas os problemas de configuração. Esse valor é opcional. Não será possível usar essa sinalização se você usar a sinalização `--vulnerabilities`.</dd>

<dt><code>--json</code></dt>
<dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>
</dl>

**Exemplo**:

```
ibmcloud ks va 1a11a1aa2b2b22223333c44444ccc555667d7dd777888e8ef99f1011121314g15 --extended --vulnerabilities --json
```
{: pre}


### ibmcloud ks webhook-create --cluster CLUSTER --level LEVEL --type slack --url URL [-s]
{: #cs_webhook_create}

Registre um webhook.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code>--cluster <em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>--level <em>LEVEL</em></code></dt>
   <dd>O nível de notificação, como <code>Normal</code> ou <code>Warning</code>. <code>Warning</code> é o valor padrão. Esse valor é opcional.</dd>

   <dt><code>--type <em>slack</em></code></dt>
   <dd>O tipo de webhook. A folga é atualmente suportada. Este valor é obrigatório.</dd>

   <dt><code>--url <em>URL</em></code></dt>
   <dd>A URL para o webhook. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks webhook-create --cluster my_cluster --level Normal --type slack --url http://github.com/mywebhook
  ```
  {: pre}


<br />


## Comandos do cluster: Subnets
{: #cluster_subnets_commands}

### ibmcloud ks cluster-subnet-add CLUSTER SUBNET [ -s ]
{: #cs_cluster_subnet_add}

É possível incluir sub-redes públicas ou privadas móveis existentes de sua conta de infraestrutura do IBM Cloud (SoftLayer) em seu cluster do Kubernetes ou reutilizar sub-redes por meio de um cluster excluído em vez de usar as sub-redes provisionadas automaticamente.

**Nota:**
* Os endereços IP públicos móveis são cobrados mensalmente. Se você remover os endereços IP públicos móveis depois que o cluster for provisionado, ainda terá que pagar o encargo mensal, mesmo se os tiver usado apenas por um curto período de tempo.
* Quando você torna uma sub-rede disponível para um cluster, os endereços IP
dessa sub-rede são usados para propósitos de rede do cluster. Para evitar conflitos de endereço IP, certifique-se de usar uma sub-rede com somente um cluster. Não use uma sub-rede para múltiplos clusters ou para outros
propósitos fora do {{site.data.keyword.containerlong_notm}} ao mesmo
tempo.
* Para rotear entre sub-redes na mesma VLAN, deve-se [ativar a ampliação de VLAN](/docs/infrastructure/vlans/vlan-spanning.html#vlan-spanning).

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code><em>SUBNET</em></code></dt>
   <dd>O ID da sub-rede. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-subnet-add my_cluster 1643389
  ```
  {: pre}


### ibmcloud ks cluster-subnet-create CLUSTER SIZE VLAN_ID [-s]
{: #cs_cluster_subnet_create}

Crie uma sub-rede em uma conta de infraestrutura do IBM Cloud (SoftLayer) e torne-a disponível para um cluster especificado em {{site.data.keyword.containerlong_notm}}.

**Nota:**
* Quando você torna uma sub-rede disponível para um cluster, os endereços IP
dessa sub-rede são usados para propósitos de rede do cluster. Para evitar conflitos de endereço IP, certifique-se de usar uma sub-rede com somente um cluster. Não use uma sub-rede para múltiplos clusters ou para outros
propósitos fora do {{site.data.keyword.containerlong_notm}} ao mesmo
tempo.
* Para rotear entre sub-redes na mesma VLAN, deve-se [ativar a ampliação de VLAN](/docs/infrastructure/vlans/vlan-spanning.html#vlan-spanning).

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório. Para listar os seus clusters, use o comando `ibmcloud ks clusters` [](#cs_clusters).</dd>

   <dt><code><em>SIZE</em></code></dt>
   <dd>O número de endereços IP de sub-rede. Este valor é obrigatório. Os valores possíveis são 8, 16, 32 ou 64.</dd>

   <dt><code><em>VLAN_ID</em></code></dt>
   <dd>A VLAN na qual criar a sub-rede. Este valor é obrigatório. Para listar as VLANS disponíveis, use o comando `ibmcloud ks vlans <zone>` [](#cs_vlans). A sub-rede é provisionada na mesma zona em que a VLAN está.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-subnet-create my_cluster 8 1764905
  ```
  {: pre}


### ibmcloud ks cluster-user-subnet-add CLUSTER SUBNET_CIDR PRIVATE_VLAN
{: #cs_cluster_user_subnet_add}

Traga a sua própria sub-rede privada para os seus clusters do {{site.data.keyword.containerlong_notm}}.

Essa sub-rede privada não é uma fornecida pela infraestrutura do IBM Cloud (SoftLayer). Como tal, deve-se configurar qualquer roteamento de tráfego de rede de entrada e saída para a sub-rede. Para incluir uma sub-rede de infraestrutura do IBM Cloud (SoftLayer), use o comando `ibmcloud ks cluster-subnet-add` [](#cs_cluster_subnet_add).

**Nota**:
* Quando você inclui uma sub-rede privada de usuário em um cluster, os endereços IP dessa sub-rede são usados para Load Balancers privados no cluster. Para evitar conflitos de endereço IP, certifique-se de usar uma sub-rede com somente um cluster. Não use uma sub-rede para múltiplos clusters ou para outros
propósitos fora do {{site.data.keyword.containerlong_notm}} ao mesmo
tempo.
* Para rotear entre sub-redes na mesma VLAN, deve-se [ativar a ampliação de VLAN](/docs/infrastructure/vlans/vlan-spanning.html#vlan-spanning).

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code><em>SUBNET_CIDR</em></code></dt>
   <dd>O Classless InterDomain Routing (CIDR) de sub-rede. Esse valor é obrigatório e não deverá entrar em conflito com qualquer sub-rede que for usada pela infraestrutura do IBM Cloud (SoftLayer).

   Os prefixos suportados variam de `/30` (1 endereço IP) a `/24` (253 endereços IP). Se você definir o CIDR com um comprimento de prefixo e posteriormente precisar mudá-lo, primeiro inclua o novo CIDR, então, [remova o CIDR antigo](#cs_cluster_user_subnet_rm).</dd>

   <dt><code><em>PRIVATE_VLAN</em></code></dt>
   <dd>O ID da VLAN privada. Este valor é obrigatório. Ele deverá corresponder ao ID de VLAN privada de um ou mais nós do trabalhador no cluster.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-user-subnet-add my_cluster 169.xx.xxx.xxx.xxx/ 29 1502175
  ```
  {: pre}


### ibmcloud ks cluster-user-subnet-rm CLUSTER SUBNET_CIDR PRIVATE_VLAN
{: #cs_cluster_user_subnet_rm}

Remova a sua própria sub-rede privada de um cluster especificado.

**Nota:** qualquer serviço que foi implementado em um endereço IP por meio de sua própria sub-rede privada permanecerá ativo após a sub-rede ser removida.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code><em>SUBNET_CIDR</em></code></dt>
   <dd>O Classless InterDomain Routing (CIDR) de sub-rede. Esse valor é obrigatório e deve corresponder ao CIDR que foi configurado pelo comando `ibmcloud ks cluster-user-subnet-add` [](#cs_cluster_user_subnet_add).</dd>

   <dt><code><em>PRIVATE_VLAN</em></code></dt>
   <dd>O ID da VLAN privada. Esse valor é obrigatório e deve corresponder ao ID de VLAN que foi configurado pelo comando `ibmcloud ks cluster-user-subnet-add` [](#cs_cluster_user_subnet_add).</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks cluster-user-subnet-rm my_cluster 169.xx.xxx.xxx.xxx/ 29 1502175
  ```
  {: pre}

### ibmcloud ks subnets [--json][-s]
{: #cs_subnets}

Visualize uma lista de sub-redes que estão disponíveis em uma conta de infraestrutura do IBM Cloud (SoftLayer).

<strong>Opções de comando</strong>:

  <dl>
  <dt><code>--json</code></dt>
  <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

**Exemplo**:

  ```
  ibmcloud ks subnets
  ```
  {: pre}


<br />


## Comandos do balanceador de carga do aplicativo (ALB) Ingress
{: #alb_commands}

### ibmcloud ks alb-cert-deploy [--update] --cluster CLUSTER --secret-name SECRET_NAME --cert-crn CERTIFICATE_CRN [-s]
{: #cs_alb_cert_deploy}

Implemente ou atualize um certificado de sua instância do {{site.data.keyword.cloudcerts_long_notm}} para o ALB em um cluster.

**Nota:**
* Somente um usuário com a função de acesso do Administrador pode executar esse comando.
* É possível atualizar somente certificados que são importados da mesma instância do {{site.data.keyword.cloudcerts_long_notm}}.

<strong>Opções de comandos</strong>

   <dl>
   <dt><code>--cluster <em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>--update</code></dt>
   <dd>Atualize o certificado para um segredo do ALB em um cluster. Esse valor é opcional.</dd>

   <dt><code>--secret-name <em>SECRET_NAME</em></code></dt>
   <dd>O nome do segredo do ALB. Este valor é obrigatório.</dd>

   <dt><code>--cert-crn <em>CERTIFICATE_CRN</em></code></dt>
   <dd>O CRN do certificado. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplos**:

Exemplo para implementar um segredo do ALB:

   ```
   ibmcloud ks alb-cert-deploy --secret-name my_alb_secret --cluster my_cluster --cert-crn crn:v1:staging:public:cloudcerts:us-south:a/06580c923e40314421d3b6cb40c01c68:0db4351b-0ee1-479d-af37-56a4da9ef30f:certificate:4bc35b7e0badb304e60aef00947ae7ff
   ```
   {: pre}

Exemplo para atualizar um segredo do ALB existente:

 ```
 ibmcloud ks alb-cert-deploy --update --secret-name my_alb_secret --cluster my_cluster --cert-crn crn:v1:staging:public:cloudcerts:us-south:a/06580c923e40314421d3b6cb40c01c68:0db4351b-0ee1-479d-af37-56a4da9ef30f:certificate:7e21fde8ee84a96d29240327daee3eb2
 ```
 {: pre}


### ibmcloud ks alb-cert-get --cluster CLUSTER [--secret-name SECRET_NAME][--cert-crn CERTIFICATE_CRN] [--json][-s]
{: #cs_alb_cert_get}

Visualize informações sobre um segredo do ALB em um cluster.

**Observação:** somente um usuário com a função de acesso do administrador pode executar esse comando.

<strong>Opções de comandos</strong>

  <dl>
  <dt><code>--cluster <em>CLUSTER</em></code></dt>
  <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>--secret-name <em>SECRET_NAME</em></code></dt>
  <dd>O nome do segredo do ALB. Esse valor é necessário para obter informações sobre um segredo do ALB específico no cluster.</dd>

  <dt><code>--cert-crn <em>CERTIFICATE_CRN</em></code></dt>
  <dd>O CRN do certificado. Esse valor é necessário para obter informações sobre todos os segredos do ALB correspondentes a um CRN de certificado específico no cluster.</dd>

  <dt><code>--json</code></dt>
  <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

**Exemplos**:

 Exemplo para buscar informações sobre um segredo do ALB:

 ```
 ibmcloud ks alb-cert-get --cluster my_cluster --secret-name my_alb_secret
 ```
 {: pre}

 Exemplo para buscar informações sobre todos os segredos do ALB que correspondem a um CRN de certificado especificado:

 ```
 ibmcloud ks alb-cert-get --cluster my_cluster --cert-crn crn:v1:staging:public:cloudcerts:us-south:a/06580c923e40314421d3b6cb40c01c68:0db4351b-0ee1-479d-af37-56a4da9ef30f:certificate:4bc35b7e0badb304e60aef00947ae7ff
 ```
 {: pre}


### ibmcloud ks alb-cert-rm --cluster CLUSTER [--secret-name SECRET_NAME][--cert-crn CERTIFICATE_CRN] [-s]
{: #cs_alb_cert_rm}

Remova um segredo do ALB em um cluster.

**Observação:** somente um usuário com a função de acesso do administrador pode executar esse comando.

<strong>Opções de comandos</strong>

  <dl>
  <dt><code>--cluster <em>CLUSTER</em></code></dt>
  <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>--secret-name <em>SECRET_NAME</em></code></dt>
  <dd>O nome do segredo do ALB. Esse valor é necessário para remover um segredo do ALB específico no cluster.</dd>

  <dt><code>--cert-crn <em>CERTIFICATE_CRN</em></code></dt>
  <dd>O CRN do certificado. Esse valor é necessário para remover todos os segredos do ALB correspondentes a um CRN de certificado específico no cluster.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

  </dl>

**Exemplos**:

 Exemplo para remover um segredo do ALB:

 ```
 ibmcloud ks alb-cert-rm --cluster my_cluster --secret-name my_alb_secret
 ```
 {: pre}

 Exemplo para remover todos os segredos do ALB que correspondem a um CRN de certificado especificado:

 ```
 ibmcloud ks alb-cert-rm --cluster my_cluster --cert-crn crn:v1:staging:public:cloudcerts:us-south:a/06580c923e40314421d3b6cb40c01c68:0db4351b-0ee1-479d-af37-56a4da9ef30f:certificate:4bc35b7e0badb304e60aef00947ae7ff
 ```
 {: pre}


### ibmcloud ks alb-certs --cluster CLUSTER [--json][-s]
{: #cs_alb_certs}

Visualize uma lista de segredos do ALB em um cluster.

**Nota:** apenas usuários com a função de acesso do Administrador podem executar esse comando.

<strong>Opções de comandos</strong>

   <dl>
   <dt><code>--cluster <em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>
   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>
   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

 ```
 ibmcloud ks alb-certs --cluster my_cluster
 ```
 {: pre}

### ibmcloud ks alb-configure --albID ALB_ID [--enable][--disable][--user-ip USERIP][-s]
{: #cs_alb_configure}

Ative ou desative um ALB em seu cluster padrão. O ALB público é ativado por padrão.

**Opções de comando**:

   <dl>
   <dt><code><em>--albID </em>ALB_ID</code></dt>
   <dd>O ID para um ALB. Execute <code>ibmcloud ks albs <em>--cluster </em>CLUSTER</code> para visualizar os IDs para os ALBs em um cluster. Este valor é obrigatório.</dd>

   <dt><code>--enable</code></dt>
   <dd>Inclua essa sinalização para ativar um ALB em um cluster.</dd>

   <dt><code>--disable</code></dt>
   <dd>Inclua essa sinalização para desativar um ALB em um cluster.</dd>

   <dt><code>--user-ip <em>USER_IP</em></code></dt>
   <dd>

   <ul>
    <li>Esse parâmetro está disponível para ativar um ALB privado apenas.</li>
    <li>O ALB privado é implementado com um endereço IP de uma sub-rede privada fornecida pelo usuário. Se nenhum endereço IP for fornecido, o ALB será implementado com um endereço IP privado da sub-rede privada móvel que foi provisionada automaticamente quando você criou o cluster.</li>
   </ul>
   </dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplos**:

  Exemplo para ativar um ALB:

  ```
  ibmcloud ks alb-configure --albID private-cr18a61a63a6a94b658596aa93a087aaa9-alb1 --enable
  ```
  {: pre}

  Exemplo para ativar um ALB com um endereço IP fornecido pelo usuário:

  ```
  ibmcloud ks alb-configure --albID private-cr18a61a63a6a94b658596aa93a087aaa9-alb1 --enable --user-ip user_ip
  ```
  {: pre}

  Exemplo para desativar um ALB:

  ```
  ibmcloud ks alb-configure --albID public-cr18a61a63a6a94b658596aa93a087aaa9-alb1 --disable
  ```
  {: pre}

### ibmcloud ks alb-get --albID ALB_ID [--json][-s]
{: #cs_alb_get}

Visualize os detalhes de um ALB.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>--albID </em>ALB_ID</code></dt>
   <dd>O ID para um ALB. Execute <code>ibmcloud ks albs --cluster <em>CLUSTER</em></code> para visualizar os IDs para os ALBs em um cluster. Este valor é obrigatório.</dd>

   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks alb-get --albID public-cr18a61a63a6a94b658596aa93a087aaa9-alb1
  ```
  {: pre}

### ibmcloud ks alb-types [--json][-s]
{: #cs_alb_types}

Visualize os tipos de ALB que são suportados na região.

<strong>Opções de comando</strong>:

  <dl>
  <dt><code>--json</code></dt>
  <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

**Exemplo**:

  ```
  ibmcloud ks alb-types
  ```
  {: pre}


### ibmcloud ks albs --cluster CLUSTER [--json][-s]
{: #cs_albs}

Visualize o status de todos os ALBs em um cluster. Se nenhum ID de ALB for retornado, então, o cluster não terá uma sub-rede portátil. É possível [criar](#cs_cluster_subnet_create) ou [incluir](#cs_cluster_subnet_add) sub-redes em um cluster.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>--cluster </em>CLUSTER</code></dt>
   <dd>O nome ou ID do cluster no qual você lista os ALBs disponíveis. Este valor é obrigatório.</dd>

   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks albs --cluster my_cluster
  ```
  {: pre}


<br />


## Comandos de infraestrutura
{: #infrastructure_commands}

### ibmcloud ks credential-set --infrastructure-api-key API_KEY --infrastructure-username USERNAME [-s]
{: #cs_credentials_set}

Configure as credenciais de conta de infraestrutura do IBM Cloud (SoftLayer) para a sua conta do {{site.data.keyword.containerlong_notm}}.

Se você tiver uma {{site.data.keyword.Bluemix_notm}}conta pré-paga, terá acesso ao portfólio de infraestrutura do IBM Cloud (SoftLayer) por padrão. No entanto, talvez você queira usar uma conta de infraestrutura do IBM Cloud (SoftLayer) diferente da que você já tem para pedir a infraestrutura. É possível vincular essa conta de infraestrutura à sua conta do {{site.data.keyword.Bluemix_notm}} conta usando este comando.

Se as credenciais de infraestrutura do IBM Cloud (SoftLayer) são configuradas manualmente, essas credenciais são usadas para pedir infraestrutura, mesmo se uma [chave API do IAM](#cs_api_key_info) já existe para a conta. Se o usuário cujas credenciais estão armazenadas não tiver as permissões necessárias para pedir a infraestrutura, as ações relacionadas à infraestrutura, como a criação de um cluster ou o recarregamento de um nó do trabalhador, poderão falhar.

Não é possível configurar múltiplas credenciais para uma conta do {{site.data.keyword.containerlong_notm}}. Cada conta do {{site.data.keyword.containerlong_notm}} é vinculada a um portfólio de infraestrutura do IBM Cloud (SoftLayer) apenas.

**Importante:** antes de usar esse comando, certifique-se de que o usuário cujas credenciais são usadas tenha as permissões necessárias do [{{site.data.keyword.containerlong_notm}} e de infraestrutura do IBM Cloud (SoftLayer)](cs_users.html#users).

<strong>Opções de comando</strong>:

   <dl>
   <dt><code>--infrastructure-username <em>USERNAME</em></code></dt>
   <dd>Nome do usuário da API de conta de infraestrutura do IBM Cloud (SoftLayer). Este valor é obrigatório. **Nota**: o nome do usuário da API de infraestrutura não é o mesmo que o IBMid. Para visualizar o nome do usuário da API de infraestrutura:
   <ol><li>Efetue login no portal do [{{site.data.keyword.Bluemix_notm}}![Ícone de link externo](../icons/launch-glyph.svg "Ícone de link externo")](https://console.bluemix.net/).</li>
   <li>No menu de expansão, selecione **Infraestrutura**.</li>
   <li>Na barra de menus, selecione **Conta** > **Usuários** > **Lista de usuários**.</li>
   <li>Para o usuário que você deseja visualizar, clique no **IBMid ou Nome do usuário**.</li>
   <li>Na seção **Informações de acesso à API**, visualize o **Nome do usuário da API**.</li>
   </ol></dd>


   <dt><code>--infrastructure-api-key <em>API_KEY</em></code></dt>
   <dd>Chave API de infraestrutura do IBM Cloud infrastructure (SoftLayer). Este valor é obrigatório.

 <p>
  Para gerar uma chave API:

  <ol>
  <li>Efetue login no portal de infraestrutura do [IBM Cloud (SoftLayer)![Ícone de link externo](../icons/launch-glyph.svg "Ícone de link externo")](https://control.bluemix.net/).</li>
  <li>Selecione <strong>Conta</strong> e, em seguida, <strong>Usuários</strong>.</li>
  <li>Clique em <strong>Gerar</strong> para gerar uma chave API de infraestrutura do IBM Cloud (SoftLayer) para a sua conta.</li>
  <li>Copie a chave API para usar nesse comando.</li>
  </ol>

  Para visualizar sua chave API existente:
  <ol>
  <li>Efetue login no portal de infraestrutura do [IBM Cloud (SoftLayer)![Ícone de link externo](../icons/launch-glyph.svg "Ícone de link externo")](https://control.bluemix.net/).</li>
  <li>Selecione <strong>Conta</strong> e, em seguida, <strong>Usuários</strong>.</li>
  <li>Clique em <strong>Visualizar</strong> para ver sua chave API existente.</li>
  <li>Copie a chave API para usar nesse comando.</li>
  </ol>
  </p></dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

  </dl>

**Exemplo**:

  ```
  ibmcloud ks credential-set --infrastructure-api-key <api_key> --infrastructure-username dbmanager
  ```
  {: pre}


### ibmcloud ks credential-unset
{: #cs_credentials_unset}

Remova as credenciais da conta de infraestrutura do IBM Cloud (SoftLayer) de sua conta do {{site.data.keyword.containerlong_notm}}.

Depois de remover as credenciais, a [chave API do IAM](#cs_api_key_info) é usada para pedir recursos em infraestrutura do IBM Cloud (SoftLayer).

<strong>Opções de comando</strong>:

  <dl>
  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

**Exemplo**:

  ```
  ibmcloud ks credential-unset
  ```
  {: pre}


### ibmcloud ks machine-types ZONE  [ -- json ][-s]
{: #cs_machine_types}

Visualizar uma lista de tipos de máquina disponíveis para seus nós do trabalhador. Tipos de máquina variam por zona. Cada tipo de máquina inclui a
quantia de CPU, memória e espaço em disco virtual para cada nó do trabalhador no cluster. Por padrão, o diretório do disco de armazenamento secundário em que todos os dados do contêiner são armazenados é criptografado com a criptografia LUKS. Se a opção `disable-disk-encrypt` for incluída durante a criação do cluster, os dados do Docker do host não estarão criptografados. [Saiba mais sobre a criptografia](cs_secure.html#encrypted_disk).
{:shortdesc}

É possível provisionar o nó do trabalhador como uma máquina virtual em hardware compartilhado ou dedicado ou como uma máquina física em bare metal. [Saiba mais sobre suas opções de tipo de máquina](cs_clusters_planning.html#shared_dedicated_node).

<strong>Opções de comando</strong>:

   <dl>
   <dt><code> <em> ZONA </em> </code></dt>
   <dd>Insira a zona na qual você deseja listar os tipos de máquina disponíveis. Este valor é obrigatório. Revise [zonas disponíveis](cs_regions.html#zones).</dd>

   <dt><code>--json</code></dt>
  <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

**Comando de exemplo**:

  ```
  ibmcloud ks machine-types dal10
  ```
  {: pre}

### ibmcloud ks vlans ZONE  [ -- all ][--json]  [ -s ]
{: #cs_vlans}

Liste as VLANs públicas e privadas que estiverem disponíveis para uma zona em sua conta de infraestrutura do IBM Cloud (SoftLayer). Para listar as VLANs disponíveis, deve-se
ter uma conta paga.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code> <em> ZONA </em> </code></dt>
   <dd>Insira a zona na qual você deseja listar as suas VLANs privadas e públicas. Este valor é obrigatório. Revise [zonas disponíveis](cs_regions.html#zones).</dd>

   <dt><code>--all</code></dt>
   <dd>Lista todas as VLANs disponíveis. Por padrão, as VLANs são filtradas para mostrar somente aquelas VLANs que são válidas. Para ser válida, uma VLAN deve ser associada à infraestrutura que pode hospedar um trabalhador com armazenamento em disco local.</dd>

   <dt><code>--json</code></dt>
  <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks vlans dal10
  ```
  {: pre}


<br />


## Comandos de criação de log
{: #logging_commands}

### ibmcloud ks logging-config-create CLUSTER --logsource LOG_SOURCE --type LOG_TYPE [--namespace KUBERNETES_NAMESPACE][--hostname LOG_SERVER_HOSTNAME_OR_IP] [--port LOG_SERVER_PORT][--space CLUSTER_SPACE] [--org CLUSTER_ORG][--app-containers CONTAINERS] [--app-paths PATHS_TO_LOGS][--syslog-protocol PROTOCOL]  [--json][--skip-validation] [-s]
{: #cs_logging_create}

Crie uma configuração de criação de log. É possível usar esse comando para encaminhar logs para contêineres, aplicativos, nós do trabalhador, clusters do Kubernetes e balanceadores de carga do aplicativo Ingress para o {{site.data.keyword.loganalysisshort_notm}} ou para um servidor syslog externo.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster.</dd>

  <dt><code>--logsource <em>LOG_SOURCE</em></code></dt>    
    <dd>A origem do log para o qual ativar o encaminhamento de log. Esse argumento suporta uma lista separada por vírgula de origens de log para aplicar a configuração. Os valores aceitos são <code>container</code>, <code>application</code>, <code>worker</code>, <code>kubernetes</code> e <code>ingress</code> e <code>kube-audit</code>. Se você não fornecer uma origem de log, configurações serão criadas para <code>container</code> e <code>ingress</code>.</dd>

  <dt><code>--type <em>LOG_TYPE</em></code></dt>
    <dd>Onde você deseja encaminhar os logs. As opções são <code>ibm</code>, que encaminha os logs para o {{site.data.keyword.loganalysisshort_notm}} e <code>syslog</code>, que encaminha os logs para um servidor externo.</dd>

  <dt><code>--namespace <em>KUBERNETES_NAMESPACE</em></code></dt>
    <dd>O namespace do Kubernetes do qual você deseja encaminhar logs. O encaminhamento de log não é suportado para os namespaces do Kubernetes <code>ibm-system</code> e <code>kube-system</code>. Esse valor é válido somente para a origem de log do contêiner e é opcional. Se você não especificar um namespace, todos os namespaces no cluster usarão essa configuração.</dd>

  <dt><code>--hostname <em>LOG_SERVER_HOSTNAME</em></code></dt>
    <dd>Quando o tipo de criação de log for <code>syslog</code>, o nome do host ou endereço IP do servidor do coletor do log. Esse valor é necessário para <code>syslog</code>. Quando o tipo de criação de log for <code>ibm</code>, a URL de ingestão {{site.data.keyword.loganalysislong_notm}}. É possível localizar a lista de URLs de ingestão disponíveis [aqui](/docs/services/CloudLogAnalysis/log_ingestion.html#log_ingestion_urls). Se você não especificar uma URL de ingestão, o endpoint para a região na qual seu cluster foi criado será usado.</dd>

  <dt><code>--port <em>LOG_SERVER_PORT</em></code></dt>
    <dd>A porta do servidor coletor do log. Esse valor é opcional. Se você não especificar uma porta, a porta padrão <code>514</code> será usada para <code>syslog</code> e a porta padrão <code>9091</code> será usada para <code>ibm</code>.</dd>

  <dt><code>--space <em>CLUSTER_SPACE</em></code></dt>
    <dd>O nome do espaço do Cloud Foundry para o qual você deseja enviar logs. Esse valor é válido somente para o tipo de log <code>ibm</code> e é opcional. Se você não especificar um espaço, os logs serão enviados para o nível de conta.</dd>

  <dt><code>--org <em>CLUSTER_ORG</em></code></dt>
    <dd>O nome da organização do Cloud Foundry em que o espaço está. Esse valor é válido somente para o tipo de log <code>ibm</code> e é necessário se você especificou um espaço.</dd>

  <dt><code>--app-paths</code></dt>
    <dd>O caminho no contêiner no qual os apps estão efetuando login. Para encaminhar logs com tipo de origem <code>application</code>, deve-se fornecer um caminho. Para especificar mais de um caminho, use uma lista separada por vírgula. Esse valor é necessário para origem de log <code>application</code>. Exemplo: <code>/var/log/myApp1/&ast;,/var/log/myApp2/&ast;</code></dd>

  <dt><code>-- syslog-protocol</code></dt>
    <dd>O protocolo de camada de transferência que será usado quando o tipo de criação de log for <code>syslog</code>. Os valores suportados são <code>tcp</code> e o <code>udp</code> padrão. Ao encaminhar para um servidor rsyslog com o protocolo <code>udp</code>, os logs com mais de 1 KB serão truncados.</dd>

  <dt><code>--app-containers</code></dt>
    <dd>Para encaminhar logs de apps, é possível especificar o nome do contêiner que contém o seu app. É possível especificar mais de um contêiner usando uma lista separada por vírgula. Se nenhum contêiner é especificado, os logs são encaminhados de todos os contêineres que contêm os caminhos que você forneceu. Essa opção é válida somente para a origem de log <code>application</code>.</dd>

  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>--skip-validation</code></dt>
    <dd>Ignore a validação dos nomes da organização e do espaço quando são especificados. Ignorar a validação diminui o tempo de processamento, mas uma configuração de criação de log inválida não encaminhará os logs corretamente. Esse valor é opcional.</dd>

    <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Exemplos**:

Exemplo para o tipo de log `ibm` que encaminha de uma origem de log `container` na porta padrão 9091:

  ```
  ibmcloud ks logging-config-create my_cluster --logsource container --namespace my_namespace --hostname ingest.logging.ng.bluemix.net --type ibm
  ```
  {: pre}

Exemplo para o tipo de log `syslog` que encaminha de uma origem de log `container` na porta padrão 514:

  ```
  ibmcloud ks logging-config-create my_cluster --logsource container --namespace my_namespace --hostname 169.xx.xxx.xxx --type syslog
  ```
  {: pre}

Exemplo para o tipo de log `syslog` que encaminha logs de uma origem `ingress` em uma porta diferente do padrão:

  ```
  ibmcloud ks logging-config-create my_cluster --logsource container --hostname 169.xx.xxx.xxx --port 5514 --type syslog
  ```
  {: pre}

### ibmcloud ks logging-config-get CLUSTER [--logsource LOG_SOURCE][--json] [-s]
{: #cs_logging_get}

Visualize todas as configurações de encaminhamento de log para um cluster ou filtre configurações de criação de log com base em origem de log.

<strong>Opções de comando</strong>:

 <dl>
  <dt><code><em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>--logsource <em>LOG_SOURCE</em></code></dt>
    <dd>O tipo de origem de log para a qual você deseja filtrar. Apenas as configurações de criação de log dessa origem de log no cluster são retornadas. Os valores aceitos são <code>container</code>, <code>application</code>, <code>worker</code>, <code>kubernetes</code>, <code>ingress</code> e <code>kube-audit</code>. Esse valor é opcional.</dd>

  <dt><code>--show-cobrindo-filtros</code></dt>
    <dd>Mostra os filtros de criação de log que tornam os filtros prévios obsoletos.</dd>

  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
 </dl>

**Exemplo**:

  ```
  ibmcloud ks logging-config-get my_cluster -- logsource worker
  ```
  {: pre}


### ibmcloud ks logging-config-refresh CLUSTER [-s]
{: #cs_logging_refresh}

Atualize a configuração de criação de log para o cluster. Isso atualiza o token de criação de log para qualquer configuração de criação de log que está encaminhando para o nível de espaço em seu cluster.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
     <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Exemplo**:

  ```
  ibmcloud ks logging-config-refresh my_cluster
  ```
  {: pre}


### ibmcloud ks logging-config-rm CLUSTER [--id LOG_CONFIG_ID][--all] [-s]
{: #cs_logging_rm}

Excluir uma configuração de encaminhamento de log ou todas as configurações de criação de log para um cluster. Isso para o encaminhamento de log para um servidor syslog remoto ou {{site.data.keyword.loganalysisshort_notm}}.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>--id <em>LOG_CONFIG_ID</em></code></dt>
   <dd>Se você deseja remover uma configuração de criação de log única, o ID de configuração de criação de log.</dd>

  <dt><code>--all</code></dt>
   <dd>A sinalização para remover todas as configurações de criação de log em um cluster.</dd>

   <dt><code>-s</code></dt>
     <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Exemplo**:

  ```
  ibmcloud ks logging-config-rm my_cluster -- id f4bc77c0-ee7d-422d-aabf-a4e6b977264e
  ```
  {: pre}


### ibmcloud ks logging-config-update CLUSTER --id LOG_CONFIG_ID --type LOG_TYPE  [--namespace NAMESPACE][--hostname LOG_SERVER_HOSTNAME_OR_IP] [--port LOG_SERVER_PORT][--space CLUSTER_SPACE] [--org CLUSTER_ORG][--app-paths PATH] [--app-containers PATH][--json] [--skipValidation][-s]
{: #cs_logging_update}

Atualize os detalhes de uma configuração de encaminhamento de log.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>--id <em>LOG_CONFIG_ID</em></code></dt>
   <dd>O ID de configuração de criação de log que você deseja atualizar. Este valor é obrigatório.</dd>

  <dt><code>--type <em>LOG_TYPE</em></code></dt>
   <dd>O protocolo de encaminhamento de log que você deseja usar. Atualmente, <code>syslog</code> e <code>ibm</code> são suportados. Este valor é obrigatório.</dd>

  <dt><code>--namespace <em>NAMESPACE</em></code>
    <dd>O namespace do Kubernetes do qual você deseja encaminhar logs. O encaminhamento de log não é suportado para os namespaces do Kubernetes <code>ibm-system</code> e <code>kube-system</code>. Esse valor é válido somente para a origem de log do <code>container</code>. Se você não especificar um namespace, todos os namespaces no cluster usarão essa configuração.</dd>

  <dt><code>--hostname <em>LOG_SERVER_HOSTNAME</em></code></dt>
   <dd>Quando o tipo de criação de log for <code>syslog</code>, o nome do host ou endereço IP do servidor do coletor do log. Esse valor é necessário para <code>syslog</code>. Quando o tipo de criação de log for <code>ibm</code>, a URL de ingestão {{site.data.keyword.loganalysislong_notm}}. É possível localizar a lista de URLs de ingestão disponíveis [aqui](/docs/services/CloudLogAnalysis/log_ingestion.html#log_ingestion_urls). Se você não especificar uma URL de ingestão, o endpoint para a região na qual seu cluster foi criado será usado.</dd>

   <dt><code>--port <em>LOG_SERVER_PORT</em></code></dt>
   <dd>A porta do servidor coletor do log. Esse valor será opcional quando o tipo de criação de log for <code>syslog</code>. Se você não especificar uma porta, a porta padrão <code>514</code> será usada para <code>syslog</code> e <code>9091</code> será usada para <code>ibm</code>.</dd>

   <dt><code>--space <em>CLUSTER_SPACE</em></code></dt>
   <dd>O nome do espaço para o qual deseja enviar logs. Esse valor é válido somente para o tipo de log <code>ibm</code> e é opcional. Se você não especificar um espaço, os logs serão enviados para o nível de conta.</dd>

   <dt><code>--org <em>CLUSTER_ORG</em></code></dt>
   <dd>O nome da organização na qual está o espaço. Esse valor é válido somente para o tipo de log <code>ibm</code> e é necessário se você especificou um espaço.</dd>

   <dt><code>-- app-caminhos <em>PATH</em>,<em>PATH</em></code></dt>
     <dd>Um caminho de arquivo absoluto no contêiner para coletar logs. Curingas, como '/var/log/*.log', podem ser usados, mas trechos recursivos, como '/var/log/**/test.log', não podem ser usados. Para especificar mais de um caminho, use uma lista separada por vírgula. Esse valor é obrigatório quando você especifica 'application' para a origem de log. </dd>

   <dt><code>-- app-containers <em>PATH</em>,<em>PATH</em></code></dt>
     <dd>O caminho nos contêineres nos quais os apps estão registrando. Para encaminhar logs com tipo de origem <code>application</code>, deve-se fornecer um caminho. Para especificar mais de um caminho, use uma lista separada por vírgula. Exemplo: <code>/var/log/myApp1/&ast;,/var/log/myApp2/&ast;</code></dd>

   <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

   <dt><code>--skipValidation</code></dt>
    <dd>Ignore a validação dos nomes da organização e do espaço quando são especificados. Ignorar a validação diminui o tempo de processamento, mas uma configuração de criação de log inválida não encaminhará os logs corretamente. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
     <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

**Exemplo para o tipo de log `ibm`**:

  ```
  ibmcloud ks logging-config-update my_cluster --id f4bc77c0-ee7d-422d-aabf-a4e6b977264e --type ibm
  ```
  {: pre}

**Exemplo para o tipo de log `syslog`**:

  ```
  ibmcloud ks logging-config-update my_cluster --id f4bc77c0-ee7d-422d-aabf-a4e6b977264e --hostname localhost --port 5514 --type syslog
  ```
  {: pre}


### ibmcloud ks logging-filter-create CLUSTER --type LOG_TYPE [--logging-configs CONFIGS][--namespace KUBERNETES_NAMESPACE] [--container CONTAINER_NAME][--level LOGGING_LEVEL] [--regex-message MESSAGE][--json] [-s]
{: #cs_log_filter_create}

Crie um filtro de criação de log. É possível usar esse comando para filtrar logs que são encaminhados por sua configuração de criação de log.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster para o qual você deseja criar um filtro de criação de log. Este valor é obrigatório.</dd>

  <dt><code>--type <em>LOG_TYPE</em></code></dt>
    <dd>O tipo de logs nos quais você deseja aplicar o filtro. Atualmente <code>all</code>, <code>container</code> e <code>host</code> são suportados.</dd>

  <dt><code>--logging-configs <em>CONFIGS</em></code></dt>
    <dd>Uma lista separada por vírgula de seus IDs de configuração de criação de log. Se não fornecido, o filtro será aplicado a todas as configurações de criação de log de cluster que forem passadas para o filtro. É possível visualizar as configurações de log que correspondem ao filtro usando a sinalização <code>--show-matching-configs</code> com o comando. Esse valor é opcional.</dd>

  <dt><code>--namespace <em>KUBERNETES_NAMESPACE</em></code></dt>
    <dd>O namespace do Kubernetes do qual se deseja filtrar logs. Esse valor é opcional.</dd>

  <dt><code>--container <em>CONTAINER_NAME</em></code></dt>
    <dd>O nome do contêiner do qual se deseja filtrar logs. Essa sinalização se aplicará apenas quando você estiver usando o tipo de log <code>container</code>. Esse valor é opcional.</dd>

  <dt><code>--level <em>LOGGING_LEVEL</em></code></dt>
    <dd>Filtra logs que estão no nível especificado e inferior. Os valores aceitáveis na ordem canônica são <code>fatal</code>, <code>error</code>, <code>warn/warning</code>, <code>info</code>, <code>debug</code> e <code>trace</code>. Esse valor é opcional. Como um exemplo, se você filtrou logs no nível <code>info</code>, <code>debug</code> e <code>trace</code> também serão filtrados. **Nota**: é possível usar essa sinalização apenas quando as mensagens de log estiverem em formato JSON e contiverem um campo de nível. Saída de exemplo: <code>{"log": "hello", "level": "info"}</code></dd>

  <dt><code>--regex-message <em>MESSAGE</em></code></dt>
    <dd>Filtra quaisquer logs que contêm uma mensagem especificada que é gravada como uma expressão regular em qualquer lugar no log. Esse valor é opcional.</dd>

  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Exemplos**:

Este exemplo filtra todos os logs que são encaminhados de contêineres com o nome `test-container` no namespace padrão que estão no nível de depuração ou menos e têm uma mensagem de log que contém "solicitação GET".

  ```
  ibmcloud ks logging-filter-create example-cluster --type container --namespace default --container test-container --level debug --message "GET request"
  ```
  {: pre}

Este exemplo filtra todos os logs que são encaminhados, em um nível de informações ou menos, por meio de um cluster específico. A saída é retornada como JSON.

  ```
  ibmcloud ks logging-filter-create example-cluster --type all --level info --json
  ```
  {: pre}



### ibmcloud ks logging-filter-get CLUSTER [--id FILTER_ID][--show-matching-configs] [--show-covering-filters][--json] [-s]
{: #cs_log_filter_view}

Visualize uma configuração de filtro de criação de log. É possível usar esse comando para visualizar os filtros de criação de log que você criou.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster do qual você deseja visualizar filtros. Este valor é obrigatório.</dd>

  <dt><code>--id <em>FILTER_ID</em></code></dt>
    <dd>O ID do filtro de log que você deseja visualizar.</dd>

  <dt><code>--show-matching-configs</code></dt>
    <dd>Mostre as configurações de criação de log que correspondem à configuração que você está visualizando. Esse valor é opcional.</dd>

  <dt><code>--show-cobrindo-filtros</code></dt>
    <dd>Mostre os filtros de criação de log que tornam os filtros prévios obsoletos. Esse valor é opcional.</dd>

  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
     <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>


### ibmcloud ks logging-filter-rm CLUSTER [--id FILTER_ID][--all] [-s]
{: #cs_log_filter_delete}

Exclua um filtro de criação de log É possível usar esse comando para remover um filtro de criação de log que você criou.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster por meio do qual você deseja excluir um filtro.</dd>

  <dt><code>--id <em>FILTER_ID</em></code></dt>
    <dd>O ID do filtro de log a ser excluído.</dd>

  <dt><code>--all</code></dt>
    <dd>Exclua todos os seus filtros de encaminhamento de log. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>


### ibmcloud ks logging-filter-update CLUSTER --id FILTER_ID --type LOG_TYPE [--logging-configs CONFIGS][--namespace KUBERNETES_NAMESPACE] [--container CONTAINER_NAME][--level LOGGING_LEVEL] [--message MESSAGE][--json] [-s]
{: #cs_log_filter_update}

Atualize um filtro de criação de log. É possível usar esse comando para atualizar um filtro de criação de log que você criou.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster para o qual você deseja atualizar um filtro de criação de log. Este valor é obrigatório.</dd>

 <dt><code>--id <em>FILTER_ID</em></code></dt>
    <dd>O ID do filtro de log a ser atualizado.</dd>

  <dt><code>--type <em>LOG_TYPE</em></code></dt>
    <dd>O tipo de logs nos quais você deseja aplicar o filtro. Atualmente <code>all</code>, <code>container</code> e <code>host</code> são suportados.</dd>

  <dt><code>--logging-configs <em>CONFIGS</em></code></dt>
    <dd>Uma lista separada por vírgula de seus IDs de configuração de criação de log. Se não fornecido, o filtro será aplicado a todas as configurações de criação de log de cluster que forem passadas para o filtro. É possível visualizar as configurações de log que correspondem ao filtro usando a sinalização <code>--show-matching-configs</code> com o comando. Esse valor é opcional.</dd>

  <dt><code>--namespace <em>KUBERNETES_NAMESPACE</em></code></dt>
    <dd>O namespace do Kubernetes do qual se deseja filtrar logs. Esse valor é opcional.</dd>

  <dt><code>--container <em>CONTAINER_NAME</em></code></dt>
    <dd>O nome do contêiner do qual se deseja filtrar logs. Essa sinalização se aplicará apenas quando você estiver usando o tipo de log <code>container</code>. Esse valor é opcional.</dd>

  <dt><code>--level <em>LOGGING_LEVEL</em></code></dt>
    <dd>Filtra logs que estão no nível especificado e inferior. Os valores aceitáveis na ordem canônica são <code>fatal</code>, <code>error</code>, <code>warn/warning</code>, <code>info</code>, <code>debug</code> e <code>trace</code>. Esse valor é opcional. Como um exemplo, se você filtrou logs no nível <code>info</code>, <code>debug</code> e <code>trace</code> também serão filtrados. **Nota**: é possível usar essa sinalização apenas quando as mensagens de log estiverem em formato JSON e contiverem um campo de nível. Saída de exemplo: <code>{"log": "hello", "level": "info"}</code></dd>

  <dt><code>--message <em>MESSAGE</em></code></dt>
    <dd>Filtra quaisquer logs que contêm uma mensagem especificada em qualquer lugar no log. A mensagem é correspondida literalmente e não como uma expressão. Exemplo: As mensagens “Hello”, “!” e “Hello, World!” se aplicariam ao log “Hello, World!”. Esse valor é opcional.</dd>

  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>



<br />


## Comandos de região
{: #region_commands}

### ibmcloud ks zones  [ -- json ][-s]
{: #cs_datacenters}

Visualize uma lista de zonas disponíveis nas quais você criará um cluster. As zonas disponíveis variam pela região na qual você está com login efetuado. Para alternar regiões, execute `ibmcloud ks region-set`.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks zones
  ```
  {: pre}


### ibmcloud ks region
{: #cs_region}

Localize a região do {{site.data.keyword.containerlong_notm}} na qual você está atualmente. É possível criar e gerenciar clusters específicos para a região. Use o comando `ibmcloud ks region-set` para mudar regiões.

**Exemplo**:

```
ibmcloud ks region
```
{: pre}

**Saída**:
```
Região: us-south
```
{: screen}

### ibmcloud ks region-set [ REGION ]
{: #cs_region-set}

Configure a região para o  {{site.data.keyword.containerlong_notm}}. É possível criar e gerenciar clusters específicos para a região e você pode querer clusters em múltiplas regiões para alta disponibilidade.

Por exemplo, é possível efetuar login no {{site.data.keyword.Bluemix_notm}} na região sul dos EUA e criar um cluster. Em seguida, é possível usar `ibmcloud ks region-set eu-central` para destinar a região central da UE e criar outro cluster. Finalmente, é possível usar `ibmcloud ks region-set us-south` para retornar para o Sul dos EUA para gerenciar o seu cluster nessa região.

**Opções de comando**:

<dl>
<dt><code><em>REGION</em></code></dt>
<dd>Insira a região que você deseja destinar. Esse valor é opcional. Se você não fornecer a região, será possível selecionar uma na lista na saída.

Para obter uma lista de regiões disponíveis, revise [regiões e zonas](cs_regions.html) ou use o comando `ibmcloud ks regions` [](#cs_regions).</dd></dl>

**Exemplo**:

```
ibmcloud ks region-set eu-central
```
{: pre}

```
ibmcloud ks region-set
```
{: pre}

**Saída**:
```
Choose a region:
1. ap-north
2. ap-south
3. eu-central
4. uk-south
5. us-east
6. us-south
Enter a number> 3
OK
```
{: screen}

### ibmcloud ks regions
{: #cs_regions}

Lista as regiões disponíveis. O `Region Name` é o nome do {{site.data.keyword.containerlong_notm}} e o `Region Alias` é o nome geral do {{site.data.keyword.Bluemix_notm}} para a região.

**Exemplo**:

```
ibmcloud ks regions
```
{: pre}

**Saída**:
```
Region Name   Region Alias
ap-north      jp-tok
ap-south      au-syd
eu-central    eu-de
uk-south      eu-gb
us-east       us-east
us-south      us-south
```
{: screen}


<br />


## Comandos de nó do trabalhador
{: worker_node_commands}


### Descontinuado: ibmcloud ks worker-add --cluster CLUSTER [--file FILE_LOCATION][--hardware HARDWARE] --machine-type MACHINE_TYPE --workers NUMBER --private-vlan PRIVATE_VLAN --public-vlan PUBLIC_VLAN [--disable-disk-encrypt][-s]
{: #cs_worker_add}

Inclua nós do trabalhador independentes em seu cluster padrão que não estejam em um conjunto de trabalhadores.

<strong>Opções de comando</strong>:

<dl>
<dt><code>--cluster <em>CLUSTER</em></code></dt>
<dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

<dt><code>--file <em>FILE_LOCATION</em></code></dt>
<dd>O caminho para o arquivo YAML incluir nós do trabalhador no cluster. Em vez de definir nós do trabalhador adicionais usando as opções fornecidas nesse comando, será possível usar um arquivo do YAML. Esse valor é opcional.

<p><strong>Nota:</strong> se você fornecer a mesma opção no comando que o parâmetro no arquivo do YAML, o valor no comando terá precedência sobre o valor no YAML. Por exemplo, você define um tipo de máquina em seu arquivo YAML e usa a opção --machine-type no comando, o valor inserido na opção de comando substituirá o valor no arquivo YAML.

<pre class="codeblock">
<code>name: <em>&lt;cluster_name_or_ID&gt;</em>
zone: <em>&lt;zone&gt;</em>
machine-type: <em>&lt;machine_type&gt;</em>
private-vlan: <em>&lt;private_VLAN&gt;</em>
public-vlan: <em>&lt;public_VLAN&gt;</em>
hardware: <em>&lt;shared_or_dedicated&gt;</em>
workerNum: <em>&lt;number_workers&gt;</em>
diskEncryption: <em>false</em></code></pre>

<table>
<caption>Entendendo os componentes de arquivo YAML</caption>
<thead>
<th colspan=2><img src="images/idea.png" alt="Ícone de ideia"/> entendendo os componentes de arquivo do YAML</th>
</thead>
<tbody>
<tr>
<td><code><em>name</em></code></td>
<td>Substitua <code><em>&lt;cluster_name_or_ID&gt;</em></code> pelo nome ou ID do cluster no qual você deseja incluir nós do trabalhador.</td>
</tr>
<tr>
<td><code><em>zone</em></code></td>
<td>Substitua <code><em>&lt;zone&gt;</em></code> pela zona para implementar os seus nós do trabalhador. As zonas disponíveis são dependentes da região na qual você efetuou login. Para listar as zonas disponíveis, execute <code>ibmcloud ks zones</code>.</td>
</tr>
<tr>
<td><code><em>machine-type</em></code></td>
<td>Substitua <code><em>&lt;machine_type&gt;</em></code> pelo tipo de máquina na qual você deseja implementar os nós do trabalhador. É possível implementar os nós do trabalhador como máquinas virtuais em hardware compartilhado ou dedicado ou como máquinas físicas no bare metal. Os tipos de máquinas físicas e virtuais disponíveis variam de acordo com a zona na qual você implementa o cluster. Para obter mais informações, consulte o comando `ibmcloud ks machine-types` [](cs_cli_reference.html#cs_machine_types).</td>
</tr>
<tr>
<td><code><em>private-vlan</em></code></td>
<td>Substitua <code><em>&lt;private_VLAN&gt;</em></code> pelo ID da VLAN privada que você deseja usar para os seus nós do trabalhador. Para listar VLANs disponíveis, execute <code>ibmcloud ks vlans <em>&lt;zone&gt;</em></code> e procure roteadores de VLAN que iniciem com <code>bcr</code> (roteador de backend).</td>
</tr>
<tr>
<td><code>public-vlan</code></td>
<td>Substitua <code>&lt;public_VLAN&gt;</code> pelo ID da VLAN pública que você deseja usar para os seus nós do trabalhador. Para listar VLANs disponíveis, execute <code>ibmcloud ks vlans &lt;zone&gt;</code> e procure roteadores de VLAN que iniciem com <code>fcr</code> (roteador de front-end). <br><strong>Nota</strong>: {[private_VLAN_vyatta]}</td>
</tr>
<tr>
<td><code>Hardware</code></td>
<td>Para tipos de máquinas virtuais: o nível de isolamento de hardware para seu nó do trabalhador. Use dedicated se desejar que os recursos físicos disponíveis sejam dedicados somente a você ou shared para permitir que os recursos físicos sejam compartilhados com outros clientes IBM. O padrão é shared.</td>
</tr>
<tr>
<td><code>workerNum</code></td>
<td>Substitua <code><em>&lt;number_workers&gt;</em></code> pelo número de nós do trabalhador que você deseja implementar.</td>
</tr>
<tr>
<td><code>diskEncryption: <em>false</em></code></td>
<td>Nós do trabalhador apresentam criptografia de disco por padrão; [saiba mais](cs_secure.html#encrypted_disk). Para desativar a criptografia, inclua essa opção e configure o valor para <code>false</code>.</td></tr>
</tbody></table></p></dd>

<dt><code>--hardware <em>HARDWARE</em></code></dt>
<dd>O nível de isolamento de hardware para seu nó do trabalhador. Use dedicated se desejar que os recursos físicos disponíveis sejam dedicados somente a você ou shared para permitir que os recursos físicos sejam compartilhados com outros clientes IBM. O padrão é shared. Esse valor é opcional.</dd>

<dt><code>--machine-type <em>MACHINE_TYPE</em></code></dt>
<dd>Escolha um tipo de máquina. É possível implementar os nós do trabalhador como máquinas virtuais em hardware compartilhado ou dedicado ou como máquinas físicas no bare metal. Os tipos de máquinas físicas e virtuais disponíveis variam de acordo com a zona na qual você implementa o cluster. Para obter mais informações, consulte a documentação para o comando `ibmcloud ks machine-types` [](cs_cli_reference.html#cs_machine_types). Esse valor é necessário para clusters padrão e não está disponível para clusters livres.</dd>

<dt><code>--workers <em>NUMBER</em></code></dt>
<dd>Um número inteiro que representa o número de nós do trabalhador a serem criados no cluster. O valor padrão é 1. Esse valor é opcional.</dd>

<dt><code>--private-vlan <em>PRIVATE_VLAN</em></code></dt>
<dd>A VLAN privada que foi especificada quando o cluster foi criado. Este valor é obrigatório.

<p><strong>Nota:</strong> os roteadores de VLAN privada sempre iniciam com <code>bcr</code> (roteador de backend) e os roteadores de VLAN pública sempre iniciam com <code>fcr</code> (roteador de front-end). Ao criar um cluster e especificar as VLANs públicas e privadas, o número e a combinação de letras após esses prefixos devem corresponder.</p></dd>

<dt><code>--public-vlan <em>PUBLIC_VLAN</em></code></dt>
<dd>A VLAN pública que foi especificada quando o cluster foi criado. Esse valor é opcional. Se você deseja que os nós do trabalhador existam somente em uma VLAN privada, não forneça um ID de VLAN pública. <strong>Nota</strong>: {[private_VLAN_vyatta]}

<p><strong>Nota:</strong> os roteadores de VLAN privada sempre iniciam com <code>bcr</code> (roteador de backend) e os roteadores de VLAN pública sempre iniciam com <code>fcr</code> (roteador de front-end). Ao criar um cluster e especificar as VLANs públicas e privadas, o número e a combinação de letras após esses prefixos devem corresponder.</p></dd>

<dt><code>--disable-disk-encrypt</code></dt>
<dd>Nós do trabalhador apresentam criptografia de disco por padrão; [saiba mais](cs_secure.html#encrypted_disk). Para desativar a criptografia, inclua essa opção.</dd>

<dt><code>-s</code></dt>
<dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

</dl>

**Exemplos**:

  ```
  ibmcloud ks worker-add --cluster my_cluster --number 3 --public-vlan my_public_VLAN_ID --private-vlan my_private_VLAN_ID --machine-type b2c.4x16 --hardware shared
  ```
  {: pre}

  Exemplo para o {{site.data.keyword.Bluemix_dedicated_notm}}:

  ```
  ibmcloud ks worker-add --cluster my_cluster --number 3 --machine-type b2c.4x16
  ```
  {: pre}

### ibmcloud ks worker-get [ CLUSTER_NAME_OR_ID ] WORKER_NODE_ID  [ -- json ][-s]
{: #cs_worker_get}

Visualize os detalhes de um nó do trabalhador.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER_NAME_OR_ID</em></code></dt>
   <dd>O nome ou o ID do cluster do nó do trabalhador. Esse valor é opcional.</dd>

   <dt><code><em>WORKER_NODE_ID</em></code></dt>
   <dd>O nome do seu nó do trabalhador. Execute <code>ibmcloud ks workers <em>CLUSTER</em></code> para visualizar os IDs para os nós do trabalhador em um cluster. Este valor é obrigatório.</dd>

   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Comando de exemplo**:

  ```
  ibmcloud ks worker-get my_cluster kube-dal10-cr18a61a63a6a94b658596aa93d087aaa9-w1
  ```
  {: pre}

**Saída de exemplo**:

  ```
  ID: kube-dal10-123456789-w1 State: normal Status: Ready Trust: disabled Private VLAN: 223xxxx Public VLAN: 223xxxx Private IP: 10.xxx.xx.xxx Public IP: 169.xx.xxx.xxx Hardware: shared Zone: dal10 Version: 1.8.11_1509
  ```
  {: screen}

### ibmcloud ks worker-reboot [-f][--hard] CLUSTER WORKER [WORKER][-s]
{: #cs_worker_reboot}

Reinicialize um nó do trabalhador em um cluster. Durante a reinicialização, o estado do nó do trabalhador não muda.

**Atenção:** reinicializando um nó do trabalhador pode causar distorção de dados no nó do trabalhador. Use esse comando com cuidado e quando souber que uma reinicialização pode ajudar a recuperar seu nó do trabalhador. Em todos os outros casos, [recarregue seu nó do trabalhador](#cs_worker_reload).

Antes de reinicializar o nó do trabalhador, certifique-se de que os pods estão reprogramados em outros nós do trabalhador para ajudar a evitar um tempo de inatividade para seu app ou distorção de dados em seu nó do trabalhador.

1. Liste todos os nós do trabalhador em seu cluster e anote o **nome** do nó do trabalhador que você deseja reinicializar.
   ```
   kubectl get nodes
   ```
   O **nome** retornado nesse comando é o endereço IP privado designado ao nó do trabalhador. É possível localizar mais informações sobre o seu nó do trabalhador quando você executa o `ibmcloud ks workers <cluster_name_or_ID>` e procura o nó do trabalhador com o mesmo endereço **IP privado**.
2. Marque o nó do trabalhador como não programável em um processo conhecido como bloqueio. Ao bloquear um nó do trabalhador, ele fica indisponível para planejamento futuro do pod. Use o **nome** do nó do trabalhador recuperado na etapa anterior.
   ```
   kubectl cordon <worker_name>
   ```
   {: pre}

3. Verifique se o planejamento do pod está desativado para seu nó do trabalhador.
   ```
   kubectl get nodes
   ```
   {: pre}
   O nó do trabalhador ficará desativado para planejamento do pod se o status exibir **SchedulingDisabled**.
 4. Force os pods para que sejam removidos do nó do trabalhador e reprogramados nos nós do trabalhador restantes no cluster.
    ```
    kubectl drain <worker_name>
    ```
    {: pre}
    Esse processo pode levar alguns minutos.
 5. Reinicialize o nó do trabalhador. Use o ID do trabalhador que é retornado do comando `ibmcloud ks workers <cluster_name_or_ID>`.
    ```
    ibmcloud ks worker-reboot <cluster_name_or_ID> <worker_name_or_ID>
    ```
    {: pre}
 6. Espere cerca de 5 minutos antes de disponibilizar o seu nó do trabalhador para planejamento de pod para assegurar que a reinicialização esteja concluída. Durante a reinicialização, o estado do nó do trabalhador não muda. A reinicialização de um nó do trabalhador é geralmente concluída em alguns segundos.
 7. Disponibilize o nó do trabalhador para planejamento do pod. Use o **nome** do nó do trabalhador retornado do comando `kubectl get nodes`.
    ```
    kubectl uncordon <worker_name>
    ```
    {: pre}
    </br>

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>-f</code></dt>
   <dd>Use esta opção para forçar a reinicialização do nó do trabalhador sem avisos do usuário. Esse valor é opcional.</dd>

   <dt><code>--hard</code></dt>
   <dd>Use esta opção para forçar uma reinicialização forçada de um nó do trabalhador cortando a energia para o nó do trabalhador. Use essa opção se o nó do trabalhador não responder ou se ele tiver uma interrupção do
Docker. Esse valor é opcional.</dd>

   <dt><code><em>WORKER</em></code></dt>
   <dd>O nome ou ID de um ou mais nós do trabalhador. Use um espaço para listar múltiplos nós do
trabalhador. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks worker-reboot my_cluster kube-dal10-cr18a61a63a6a94b658596aa93d087aaa9-w1 kube-dal10-cr18a61a63a6a94b658596aa996aa93d087aaa9-w2
  ```
  {: pre}


### ibmcloud ks worker-reload [-f] CLUSTER WORKER [WORKER][-s]
{: #cs_worker_reload}

Recarregue todas as configurações necessárias para um nó do trabalhador. Um recarregamento poderá ser útil se seu nó do trabalhador tiver problemas, como desempenho lento ou se o nó do trabalhador estiver preso em um estado inoperante.

O recarregamento de um nó do trabalhador aplica atualizações da versão de correção ao nó do trabalhador, mas não atualizações principais ou secundárias. Para ver as mudanças de uma versão de correção para a próxima, revise a documentação de [Log de mudanças da versão](cs_versions_changelog.html#changelog).
{: tip}

Antes de recarregar seu nó do trabalhador, certifique-se de que os pods estejam reprogramados em outros nós do trabalhador para ajudar a evitar um tempo de inatividade para seu app ou distorção de dados em seu nó do trabalhador.

1. Liste todos os nós do trabalhador em seu cluster e anote o **nome** do nó do trabalhador que você deseja recarregar.
   ```
   kubectl get nodes
   ```
   O **nome** retornado nesse comando é o endereço IP privado designado ao nó do trabalhador. É possível localizar mais informações sobre o seu nó do trabalhador quando você executa o `ibmcloud ks workers <cluster_name_or_ID>` e procura o nó do trabalhador com o mesmo endereço **IP privado**.
2. Marque o nó do trabalhador como não programável em um processo conhecido como bloqueio. Ao bloquear um nó do trabalhador, ele fica indisponível para planejamento futuro do pod. Use o **nome** do nó do trabalhador recuperado na etapa anterior.
   ```
   kubectl cordon <worker_name>
   ```
   {: pre}

3. Verifique se o planejamento do pod está desativado para seu nó do trabalhador.
   ```
   kubectl get nodes
   ```
   {: pre}
   O nó do trabalhador ficará desativado para planejamento do pod se o status exibir **SchedulingDisabled**.
 4. Force os pods para que sejam removidos do nó do trabalhador e reprogramados nos nós do trabalhador restantes no cluster.
    ```
    kubectl drain <worker_name>
    ```
    {: pre}
    Esse processo pode levar alguns minutos.
 5. Recarregue o nó do trabalhador. Use o ID do trabalhador que é retornado do comando `ibmcloud ks workers <cluster_name_or_ID>`.
    ```
    ibmcloud ks worker-reload <cluster_name_or_ID> <worker_name_or_ID>
    ```
    {: pre}
 6. Aguarde o recarregamento ser concluído.
 7. Disponibilize o nó do trabalhador para planejamento do pod. Use o **nome** do nó do trabalhador retornado do comando `kubectl get nodes`.
    ```
    kubectl uncordon <worker_name>
    ```
</br>
<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>-f</code></dt>
   <dd>Use esta opção para forçar a recarga de um nó do trabalhador sem avisos do usuário. Esse valor é opcional.</dd>

   <dt><code><em>WORKER</em></code></dt>
   <dd>O nome ou ID de um ou mais nós do trabalhador. Use um espaço para listar múltiplos nós do
trabalhador. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks worker-reload my_cluster kube-dal10-cr18a61a63a6a94b658596aa93d087aaa9-w1 kube-dal10-cr18a61a63a6a94b658596aa996aa93d087aaa9-w2
  ```
  {: pre}


### ibmcloud ks worker-rm [-f] CLUSTER WORKER [WORKER][-s]
{: #cs_worker_rm}

Remover um ou mais nós do trabalhador de um cluster. Se você remover um nó do trabalhador, o seu cluster se tornará desbalanceado. É possível rebalancear automaticamente o seu conjunto de trabalhadores executando o comando `ibmcloud ks worker-pool-rebalance` [](#cs_rebalance).

Antes de remover o seu nó do trabalhador, certifique-se de que os pods estejam reprogramados em outros nós do trabalhador para ajudar a evitar um tempo de inatividade para o seu app ou a distorção de dados em seu nó do trabalhador.
{: tip}

1. Liste todos os nós do trabalhador em seu cluster e anote o **nome** do nó do trabalhador que você deseja remover.
   ```
   kubectl get nodes
   ```
   O **nome** retornado nesse comando é o endereço IP privado designado ao nó do trabalhador. É possível localizar mais informações sobre o seu nó do trabalhador quando você executa o `ibmcloud ks workers <cluster_name_or_ID>` e procura o nó do trabalhador com o mesmo endereço **IP privado**.
2. Marque o nó do trabalhador como não programável em um processo conhecido como bloqueio. Ao bloquear um nó do trabalhador, ele fica indisponível para planejamento futuro do pod. Use o **nome** do nó do trabalhador recuperado na etapa anterior.
   ```
   kubectl cordon <worker_name>
   ```
   {: pre}

3. Verifique se o planejamento do pod está desativado para seu nó do trabalhador.
   ```
   kubectl get nodes
   ```
   {: pre}
   O nó do trabalhador ficará desativado para planejamento do pod se o status exibir **SchedulingDisabled**.
4. Force os pods para que sejam removidos do nó do trabalhador e reprogramados nos nós do trabalhador restantes no cluster.
   ```
   kubectl drain <worker_name>
   ```
   {: pre}
   Esse processo pode levar alguns minutos.
5. Remova o nó do trabalhador. Use o ID do trabalhador que é retornado do comando `ibmcloud ks workers <cluster_name_or_ID>`.
   ```
   ibmcloud ks worker-rm <cluster_name_or_ID> <worker_name_or_ID>
   ```
   {: pre}

6. Verifique se o nó do trabalhador foi removido.
   ```
   ibmcloud ks workers <cluster_name_or_ID>
   ```
</br>
<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

   <dt><code>-f</code></dt>
   <dd>Use esta opção para forçar a remoção de um nó do trabalhador sem avisos do usuário. Esse valor é opcional.</dd>

   <dt><code><em>WORKER</em></code></dt>
   <dd>O nome ou ID de um ou mais nós do trabalhador. Use um espaço para listar múltiplos nós do
trabalhador. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks worker-rm my_cluster kube-dal10-cr18a61a63a6a94b658596aa93d087aaa9-w1 kube-dal10-cr18a61a63a6a94b658596aa996aa93d087aaa9-w2
  ```
  {: pre}


### ibmcloud ks worker-update [-f] CLUSTER WORKER [WORKER][--kube-version MAJOR.MINOR.PATCH] [--force-update][-s]
{: #cs_worker_update}

Atualize os nós do trabalhador para aplicar as atualizações e correções de segurança mais recentes no sistema operacional e para atualizar a versão do Kubernetes para corresponder à versão do nó principal. É possível atualizar a versão do Kubernetes do nó principal com o comando `ibmcloud ks cluster-update` [](cs_cli_reference.html#cs_cluster_update).

**Importante**: executar `ibmcloud ks worker-update` pode causar tempo de inatividade para os seus apps e serviços. Durante a atualização, todos os pods serão reprogramados sobre outros nós do trabalhador e os dados serão excluídos, se não forem armazenados fora do pod. Para evitar tempo de inatividade, [assegure-se de que você tenha nós do trabalhador suficientes para manipular a carga de trabalho enquanto os nós do trabalhador selecionados estão atualizando](cs_cluster_update.html#worker_node).

Pode ser necessário mudar seus arquivos YAML para implementações antes de atualizar. Revise essa [nota sobre a liberação](cs_versions.html) para obter detalhes.

<strong>Opções de comando</strong>:

   <dl>

   <dt><em>CLUSTER</em></dt>
   <dd>O nome ou ID do cluster no qual você lista nós do trabalhador disponíveis. Este valor é obrigatório.</dd>

   <dt><code>-f</code></dt>
   <dd>Use esta opção para forçar a atualização do mestre sem avisos do usuário. Esse valor é opcional.</dd>

   <dt><code>--force-update</code></dt>
   <dd>Tente a atualização mesmo se a mudança for maior que duas versões secundárias. Esse valor é opcional.</dd>

   <dt><code>--kube-version <em>MAJOR.MINOR.PATCH</em></code></dt>
     <dd>A versão do Kubernetes com a qual você deseja que os nós do trabalhador sejam atualizados. A versão padrão será usada se este valor não for especificado.</dd>

   <dt><code><em>WORKER</em></code></dt>
   <dd>O ID de um ou mais nós do trabalhador. Use um espaço para listar múltiplos nós do
trabalhador. Este valor é obrigatório.</dd>

   <dt><code>-s</code></dt>
   <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

   </dl>

**Exemplo**:

  ```
  ibmcloud ks worker-update my_cluster kube-dal10-cr18a61a63a6a94b658596aa93d087aaa9-w1 kube-dal10-cr18a61a63a6a94b658596aa996aa93d087aaa9-w2
  ```
  {: pre}


### ibmcloud ks workers CLUSTER [--worker-pool] POOL [--show-deleted][--json] [-s]
{: #cs_workers}

Visualizar uma lista de nós do trabalhador e o status de cada um deles em um cluster.

<strong>Opções de comando</strong>:

   <dl>
   <dt><code><em>CLUSTER</em></code></dt>
   <dd>O nome ou o ID do cluster para os nós disponíveis do trabalhador. Este valor é obrigatório.</dd>

   <dt><code>--worker-pool <em>POOL</em></code></dt>
   <dd>Visualize somente os nós do trabalhador que pertencem ao conjunto de trabalhadores. Para listar os conjuntos de trabalhadores disponíveis, execute `ibmcloud ks worker-pools --cluster <cluster_name_or_ID>`. Esse valor é opcional.</dd>

   <dt><code>--show-deleted</code></dt>
   <dd>Visualize nós do trabalhador que foram excluídos do cluster, incluindo o motivo para a exclusão. Esse valor é opcional.</dd>

   <dt><code>--json</code></dt>
   <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
  <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
   </dl>

**Exemplo**:

  ```
  ibmcloud ks workers my_cluster
  ```
  {: pre}

<br />


## Comandos do conjunto do trabalhador
{: #worker-pool}

### ibmcloud ks worker-pool-create --name POOL_NAME --cluster CLUSTER --machine-type MACHINE_TYPE --size-per-zone WORKERS_PER_ZONE [--hardware ISOLATION][--labels LABELS] [--disable-disk-encrypt]
{: #cs_worker_pool_create}

É possível criar um conjunto de trabalhadores em seu cluster. Quando você incluir um conjunto de trabalhadores, ele não terá uma zona designada por padrão. Você especifica o número de trabalhadores que você deseja em cada zona e os tipos de máquina para os trabalhadores. O conjunto de trabalhadores recebe as versões padrão do Kubernetes. Para concluir a criação de trabalhadores, [inclua uma zona ou zonas](#cs_zone_add) em seu conjunto.

<strong>Opções de comando</strong>:
<dl>

  <dt><code>--name <em>POOL_NAME</em></code></dt>
    <dd>O nome que você deseja dar ao seu conjunto de trabalhadores.</dd>

  <dt><code>--cluster <em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>--machine-type <em>MACHINE_TYPE</em></code></dt>
    <dd>Escolha um tipo de máquina. É possível implementar os nós do trabalhador como máquinas virtuais em hardware compartilhado ou dedicado ou como máquinas físicas no bare metal. Os tipos de máquinas físicas e virtuais disponíveis variam de acordo com a zona na qual você implementa o cluster. Para obter mais informações, consulte a documentação para o comando `ibmcloud ks machine-types` [](cs_cli_reference.html#cs_machine_types). Esse valor é necessário para clusters padrão e não está disponível para clusters livres.</dd>

  <dt><code>--size-per-zona <em>WORKERS_PER_ZONE</em></code></dt>
    <dd>O número de trabalhadores a serem criados em cada zona. Este valor é obrigatório.</dd>

  <dt><code>--hardware <em>HARDWARE</em></code></dt>
    <dd>O nível de isolamento de hardware para seu nó do trabalhador. Use dedicated se desejar que os recursos físicos disponíveis sejam dedicados somente a você ou shared para permitir que os recursos físicos sejam compartilhados com outros clientes IBM. O padrão é shared. Esse valor é opcional.</dd>

  <dt><code>--labels <em>LABELS</em></code></dt>
    <dd>Os rótulos que você deseja designar aos trabalhadores em seu conjunto. Exemplo: <key1>=<val1>,<key2>=<val2></dd>

  <dt><code>--disable-disk-encrpyt </code></dt>
    <dd>Especifica que o disco não está criptografado. O valor padrão é <code>false</code>.</dd>

</dl>

**Comando de exemplo**:

  ```
  ibmcloud ks worker-pool-create my_cluster --machine-type b2c.4x16 --size-per-zone 6
  ```
  {: pre}

### ibmcloud ks worker-pool-get --worker-pool WORKER_POOL --cluster CLUSTER
{: #cs_worker_pool_get}

Visualize os detalhes de um conjunto de trabalhadores.

<strong>Opções de comando</strong>:

<dl>
  <dt><code>-- worker-conjunto <em>WORKER_POOL</em></code></dt>
    <dd>O nome do conjunto de nós do trabalhador do qual você deseja visualizar os detalhes. Para listar os conjuntos de trabalhadores disponíveis, execute `ibmcloud ks worker-pools --cluster <cluster_name_or_ID>`. Este valor é obrigatório.</dd>
  <dt><code>--cluster <em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster no qual o conjunto de trabalhadores está localizado. Este valor é obrigatório.</dd>
</dl>

**Comando de exemplo**:

  ```
  ibmcloud ks worker-pool-get --worker-pool pool1 --cluster my_cluster
  ```
  {: pre}

**Saída de exemplo**:

  ```
  Name: pool ID: a1a11b2222222bb3c33c3d4d44d555e5-f6f777g State: active Hardware: shared Zones: dal10,dal12 Workers per zone: 3 Machine type: b2c.4x16.encrypted Labels: - Version: 1.10.11_1512
  ```
  {: screen}

### ibmcloud ks worker-pool-rebalance --cluster CLUSTER --worker-pool WORKER_POOL [-s]
{: #cs_rebalance}

É possível rebalancear o seu conjunto de trabalhadores depois de excluir um nó do trabalhador. Quando você executar esse comando, um novo trabalhador ou trabalhadores serão incluídos em seu conjunto de trabalhadores.

<strong>Opções de comando</strong>:

<dl>
  <dt><code><em>--cluster CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>
  <dt><code><em>--worker-pool WORKER_POOL</em></code></dt>
    <dd>O conjunto de trabalhadores que você deseja rebalancear. Este valor é obrigatório.</dd>
  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Exemplo**:

  ```
  ibmcloud ks worker-pool-rebalance --cluster my_cluster --worker-pool my_pool
  ```
  {: pre}

### ibmcloud ks worker-pool-resize --worker-pool WORKER_POOL --cluster CLUSTER --size-per-zone WORKERS_PER_ZONE [-s]
{: #cs_worker_pool_resize}

Redimensione seu conjunto de trabalhadores para aumentar ou diminuir o número de nós do trabalhador que estão em cada zona de seu cluster. O seu conjunto de trabalhadores deve ter pelo menos 1 nó do trabalhador.

<strong>Opções de comando</strong>:

<dl>
  <dt><code>-- worker-conjunto <em>WORKER_POOL</em></code></dt>
    <dd>O nome do conjunto de nós do trabalhador que se deseja atualizar. Este valor é obrigatório.</dd>

  <dt><code>--cluster <em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster para o qual você deseja redimensionar conjuntos de trabalhadores. Este valor é obrigatório.</dd>

  <dt><code>--size-per-zona <em>WORKERS_PER_ZONE</em></code></dt>
    <dd>O número de trabalhadores que você deseja ter em cada zona. Esse valor é obrigatório e deve ser 1 ou superior.</dd>

  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>

</dl>

**Comando de exemplo**:

  ```
  ibmcloud ks worker-pool-resize --cluster my_cluster --worker-pool my_pool --size-per-zone 3
  ```
  {: pre}

### ibmcloud ks worker-pool-rm --worker-pool WORKER_POOL --cluster CLUSTER [--json][-s]
{: #cs_worker_pool_rm}

Remover um conjunto de trabalhadores do seu cluster. Todos os nós do trabalhador no conjunto são excluídos. Seus pods são reprogramados quando você exclui. Para evitar tempo de inatividade, certifique-se de que você tenha trabalhadores suficientes para executar a carga de trabalho.

<strong>Opções de comando</strong>:

<dl>
  <dt><code>-- worker-conjunto <em>WORKER_POOL</em></code></dt>
    <dd>O nome do conjunto de nós do trabalhador que você deseja remover. Este valor é obrigatório.</dd>
  <dt><code>--cluster <em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster do qual você deseja remover o conjunto de trabalhadores. Este valor é obrigatório.</dd>
  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>
  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Comando de exemplo**:

  ```
  ibmcloud ks worker-pool-rm --cluster my_cluster --worker-pool pool1
  ```
  {: pre}

### ibmcloud ks worker-pools --cluster CLUSTER [--json][-s]
{: #cs_worker_pools}

Visualize os conjuntos de trabalhadores que você tem em um cluster.

<strong>Opções de comando</strong>:

<dl>
  <dt><code>-- cluster <em>CLUSTER_NAME_OR_ID</em></code></dt>
    <dd>O nome ou ID do cluster para o qual você deseja listar os conjuntos de trabalhadores. Este valor é obrigatório.</dd>
  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>
  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Comando de exemplo**:

  ```
  ibmcloud ks worker-pools --cluster my_cluster
  ```
  {: pre}

### ibmcloud ks zone-add --zone ZONE --cluster CLUSTER --worker-pools WORKER_POOL1,[WORKER_POOL2] --private-vlan PRIVATE_VLAN [--public-vlan PUBLIC_VLAN][--private-only] [--json][-s]
{: #cs_zone_add}

**Somente clusters de múltiplas zonas**: após criar um cluster ou conjunto de trabalhadores, será possível incluir uma zona. Quando você incluir uma zona, os nós do trabalhador serão incluídos na nova zona para corresponder ao número de trabalhadores por zona que você especificou para o conjunto de trabalhadores.

<strong>Opções de comando</strong>:

<dl>
  <dt><code>--zone <em>ZONE</em></code></dt>
    <dd>A zona que você deseja incluir. Ele deve ser uma [zona com capacidade para múltiplas zonas](cs_regions.html#zones) dentro da região do cluster. Este valor é obrigatório.</dd>

  <dt><code>--cluster <em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>--worker-pool <em>WORKER_POOLS</em></code></dt>
    <dd>Uma lista separada por vírgulas de conjuntos de trabalhadores aos quais a zona é incluída. Pelo menos 1 conjunto de trabalhadores é necessário.</dd>

  <dt><code>--private-vlan <em>PRIVATE_VLAN</em></code></dt>
    <dd><p>O ID da VLAN privada. Esse valor é condicional.</p>
    <p>Se você tiver uma VLAN privada na zona, esse valor deverá corresponder ao ID de VLAN privada de um ou mais nós do trabalhador no cluster. Para ver as VLANs que você tem disponíveis, execute <code>ibmcloud ks cluster-get --cluster &lt;cluster&gt; --showResources</code>.</p>
    <p>Se você não tiver uma VLAN privada ou pública nessa zona, não especifique essa opção. Uma VLAN privada e uma pública serão criadas automaticamente para você quando você incluir inicialmente uma nova zona em seu conjunto de trabalhadores. Em seguida, <a href="/docs/infrastructure/vlans/vlan-spanning.html#vlan-spanning" >ative a ampliação de VLAN</a> para a sua conta para que os nós do trabalhador em diferentes zonas possam se comunicar entre si.</p>
<p>**Nota**: novos nós do trabalhador são incluídos nas VLANs especificadas, mas as VLANs para quaisquer nós do trabalhador existentes não mudam.</p></dd>

  <dt><code>--public-vlan <em>PUBLIC_VLAN</em></code></dt>
    <dd><p>O ID da VLAN pública. Esse valor será necessário se você desejar expor as cargas de trabalho nos nós para o público depois de criar o cluster. Ele deve corresponder ao ID da VLAN pública de um ou mais nós do trabalhador no cluster para a zona. Para ver as VLANs que você tem disponíveis, execute <code>ibmcloud ks cluster-get --cluster &lt;cluster&gt; --showResources</code>.</p>
    <p>Se você não tiver uma VLAN privada ou pública nessa zona, não especifique essa opção. Uma VLAN privada e uma pública serão criadas automaticamente para você quando você incluir inicialmente uma nova zona em seu conjunto de trabalhadores. Em seguida, <a href="/docs/infrastructure/vlans/vlan-spanning.html#vlan-spanning" >ative a ampliação de VLAN</a> para a sua conta para que os nós do trabalhador em diferentes zonas possam se comunicar entre si.</p>
    <p>**Nota**: novos nós do trabalhador são incluídos nas VLANs especificadas, mas as VLANs para quaisquer nós do trabalhador existentes não mudam.</p></dd>

  <dt><code>-- somente privado </code></dt>
    <dd>Use essa opção para evitar que uma VLAN pública seja criada. Necessário somente quando você especifica a sinalização `--private-vlan` e não inclui a sinalização `--public-vlan`.  **Nota**: se você desejar um cluster somente privado, deverá configurar um dispositivo de gateway para conectividade de rede. Para obter mais informações, consulte [Planejando a rede externa privada apenas para uma configuração de VLAN privada](cs_network_planning.html#private_vlan).</dd>

  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Exemplo**:

  ```
  ibmcloud ks zone-add --zone dal10 --cluster my_cluster --worker-pools pool1,pool2,pool3 --private-vlan 2294021
  ```
  {: pre}

  ### ibmcloud ks zone-network-set --zone ZONE --cluster CLUSTER --worker-pools WORKER_POOL1,[WORKER_POOL2] --private-vlan PRIVATE_VLAN [--public-vlan PUBLIC_VLAN][--json] [-s]
  {: #cs_zone_network_set}

  **Somente clusters de múltiplas zonas**: configure os metadados de rede para um conjunto de trabalhadores para usar uma VLAN pública ou privada diferente para a zona do que foi usada anteriormente. Os nós do trabalhador que já foram criados no conjunto continuam a usar a VLAN pública ou privada anterior, mas os novos nós do trabalhador no conjunto usam os novos dados de rede.

  <strong>Opções de comando</strong>:

  <dl>
    <dt><code>--zone <em>ZONE</em></code></dt>
      <dd>A zona que você deseja incluir. Ele deve ser uma [zona com capacidade para múltiplas zonas](cs_regions.html#zones) dentro da região do cluster. Este valor é obrigatório.</dd>

  <dt><code>--cluster <em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>--worker-pool <em>WORKER_POOLS</em></code></dt>
    <dd>Uma lista separada por vírgulas de conjuntos de trabalhadores aos quais a zona é incluída. Pelo menos 1 conjunto de trabalhadores é necessário.</dd>

  <dt><code>--private-vlan <em>PRIVATE_VLAN</em></code></dt>
    <dd>O ID da VLAN privada. Este valor é obrigatório. Ele deverá corresponder ao ID de VLAN privada de um ou mais nós do trabalhador no cluster. Para ver as VLANs que você tem disponíveis, execute <code>ibmcloud ks cluster-get --cluster &lt;cluster&gt; --showResources</code>. Se você não tiver nenhuma VLAN disponível, será possível <a href="/docs/infrastructure/vlans/vlan-spanning.html#vlan-spanning" >ativar a ampliação de VLAN</a> para a sua conta.<br><br>**Nota**: novos nós do trabalhador são incluídos nas VLANs especificadas, mas as VLANs para quaisquer nós do trabalhador existentes não mudam.</dd>

  <dt><code>--public-vlan <em>PUBLIC_VLAN</em></code></dt>
    <dd>O ID da VLAN pública. Esse valor será necessário se você desejar mudar a VLAN pública para a zona. Se você não desejar mudar a VLAN privada com a VLAN pública, use o mesmo ID de VLAN privada. O ID de VLAN pública deve corresponder ao ID de VLAN pública de um ou mais nós do trabalhador no cluster. Para ver as VLANs que você tem disponíveis, execute <code>ibmcloud ks cluster-get --cluster &lt;cluster&gt; --showResources</code>. Se você não tiver nenhuma VLAN disponível, será possível <a href="/docs/infrastructure/vlans/vlan-spanning.html#vlan-spanning" >ativar a ampliação de VLAN</a> para a sua conta.<br><br>**Nota**: novos nós do trabalhador são incluídos nas VLANs especificadas, mas as VLANs para quaisquer nós do trabalhador existentes não mudam.</dd>

  <dt><code>--json</code></dt>
    <dd>Imprime a saída de comando no formato JSON. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
  </dl>

  **Exemplo**:

  ```
  ibmcloud ks zone-network-set --zone dal10 --cluster my_cluster --worker-pools pool1,pool2,pool3 --private-vlan 2294021
  ```
  {: pre}

### ibmcloud ks zone-rm --zone ZONE --cluster CLUSTER [-f][-s]
{: #cs_zone_rm}

**Somente clusters de múltiplas zonas**: remova uma zona de todos os conjuntos de trabalhadores em seu cluster. Todos os nós do trabalhador no conjunto de trabalhadores para essa zona são excluídos.

Antes de remover uma zona, certifique-se de que tenha nós do trabalhador suficientes em outras zonas no cluster para que os seus pods possam reagendar para ajudar a evitar um tempo de inatividade para o seu app ou uma distorção de dados em seu nó do trabalhador.
{: tip}

<strong>Opções de comando</strong>:

<dl>
  <dt><code>--zone <em>ZONE</em></code></dt>
    <dd>A zona que você deseja incluir. Ele deve ser uma [zona com capacidade para múltiplas zonas](cs_regions.html#zones) dentro da região do cluster. Este valor é obrigatório.</dd>

  <dt><code>--cluster <em>CLUSTER</em></code></dt>
    <dd>O nome ou ID do cluster. Este valor é obrigatório.</dd>

  <dt><code>-f</code></dt>
    <dd>Forçar a atualização sem prompts de usuário. Esse valor é opcional.</dd>

  <dt><code>-s</code></dt>
    <dd>Não mostrar a mensagem do dia ou os lembretes de atualização. Esse valor é opcional.</dd>
</dl>

**Exemplo**:

  ```
  ibmcloud ks zone-rm --zone dal10 --cluster my_cluster
  ```
  {: pre}
