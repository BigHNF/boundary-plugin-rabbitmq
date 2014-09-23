Boundary RabbitMQ Plugin
=======================

Boundary RabbitMQ plugin extracts key performance metrics from an instance of RabbitMQ instances

The RabbitMQ plugin requires that you have python 2.6.6 or later installed on the target system.

## Metrics
Here are the list of metrics created when the RabbitMQ plugin is installed along with their descriptions.

| Metric                                        | Description |
|-----------------------------------------------|-------------|
|RABBITMQ\_TOTAL\_EXCHANGES                     | |
|RABBITMQ\_TOTAL\_CONSUMERS                     | |
|RABBITMQ\_TOTAL\_CONNECTIONS                   | |
|RABBITMQ\_MESSAGES\_PUSH\_TOTAL                | |
|RABBITMQ\_MESSAGES\_PUSH\_RATE                 | |
|RABBITMQ\_MESSAGES\_PUSHED\_WITH\_NO\_ACK      | |
|RABBITMQ\_MESSAGES\_PUSHED\_WITH\_NO\_ACK\_RATE| |
|RABBITMQ\_MESSAGES\_PULLED                     | |
|RABBITMQ\_MESSAGES\_TOTAL\_PUSH\_PULL\_RATE    | |
|RABBITMQ\_MESSAGES\_REDELIVERED                | |
|RABBITMQ\_MESSAGES\_REDELIVERY\_RATE           | |
|RABBITMQ\_MESSAGES\_PUBLISHED                  | |
|RABBITMQ\_MESSAGES\_PUBLISH\_RATE              | |
|RABBITMQ\_QUEUE\_TOTAL\_MESSAGES               | |
|RABBITMQ\_QUEUE\_MESSAGE\_RATE                 | |
|RABBITMQ\_QUEUE\_MESSAGES\_READY               | |
|RABBITMQ\_QUEUE\_READY\_MESSAGES\_RATE         | |
|RABBITMQ\_QUEUED\_UN\_ACK\_MESSAGES            | |
|RABBITMQ\_QUEUE\_UN\_ACK\_MESSAGES\_RATE       | |
|RABBITMQ\_MEMORY\_USED                         | |
|RABBITMQ\_DISK\_FREE                           | |


## Dashboards
Here are the list of dashboards that are created when the RabbitMQ plugin is installed with their descriptions.

|Dashboard           | Description                                      |
|:-------------------|--------------------------------------------------|
|_RabbitMQ Summary_  |Contains summary metris related to RabbitMQ       |
|_RabbitMQ Messages_ |Contains metrics related to RabbitMQ messages     |
|_RabbitMQ Queues_   |Contains metrics related to RabbitMQ queues       |
|_RabbitMQ Resources_|Contains metrics related to the RabbitMQ resources|


## Adding the RabbitMQ Plugin to Premium Boundary

1. Login into Boundary Premium
2. Display the settings dialog by clicking on the _settings icon_: ![](src/main/resources/settings_icon.png)
3. Click on the _Plugins_ in the settings dialog.
4. Locate the _rabbitmq_ plugin item and click on the _Install_ button.
5. A confirmation dialog is displayed indicating the plugin was installed sucessfully, along with the metrics and the dashboards.
6. Click on the _OK_ button to dismiss the dialog.

## Removing the RabbitMQ Plugin from Premium Boundary

1. Login into Boundary Premium
2. Display the settings dialog by clicking on the _settings icon_: ![](src/main/resources/settings_icon.png)
3. Click on the _Plugins_ in the settings dialog which lists the installed plugins.
4. Locate the _rabbit_ plugin and click on the item, which then displays the uninstall dialog.
5. Click on the _Uninstall_ button which displays a confirmation dialog along with the details on what metrics and dashboards will be removed.
6. Click on the _Uninstall_ button to perfom the actual uninstall and then click on the _Close_ button to dismiss the dialog.

## Configuration

Once the RabbitMQ plugin is install, metric collection requires that a _relay_ is installed on the target system. Instructions on how to install a relay for linux/unix can found [here](http://premium-documentation.boundary.com/relays), and for Windows [here](http://premium-support.boundary.com/customer/portal/articles/1656465-installing-relay-on-windows).

General operations for plugins are describe in this [article](http://premium-support.boundary.com/customer/portal/articles/1635550-plugins---how-to)
