## Task 1: Prepare Your Ubuntu Server
Before installing Grafana and configuring Azure Monitor agent, we ensure that Ubuntu server is up-to-date

![Task 1 Image](images/task1b.png)
![Task 1 Image](images/task1c.png)

## Task 2: Install Grafana

I ran the scripts provided in the lab manual and verified that Grafna server is running
![Task 2 Image](images/task2.png)

## Task 3: Install the Azure Monitor Agent

Using the instructions in lab manual , I installed azure CLI and was successfully connected to my account 

![Task 3 Image](images/task3a.png)
![Task 3 Image](images/task3b.png)

## Task 4: Collect Performance Metrics

Created log analytics workspace in Azure portal
![Task 4 Image](images/task4a.png)

Created data collection rule and added the ubuntu VM as data source
![Task 4 Image](images/task4b.png)

Collected performace metrics
![Task 4 Image](images/task4c.png)

Monitor agent with Data collection rule is created
![Task 4 Image](images/task4d.png)

## Task 5: Connect Grafana to Azure Monitor
Create App regiter in azure portal
we can see the Tenant ID and APP ID there 
![Task 5 Image](images/task5a.png)

Then I created client certificate 
![Task 5 Image](images/task5b.png)

Added network inbound rule
![Task 5 Image](images/task5d.png)

Open Grafana in your web browser (http://20.151.92.61:3000/login) and log in with the default credentials (admin/admin)

![Task 5 Image](images/task5e.png)

- Navigated to Configuration > Data Sources and click on “Add data source.”

- Selected “Azure Monitor” from the list.

![Task 5 Image](images/task5x.png)

- Entered the details for Azure subscription, tenant ID, client ID, and client secret.
![Task 5 Image](images/task5f.png)

- Save and test the connection to ensure it is configured correctly.
Used the Client ID, App ID and Client secret
![Task 5 Image](images/task5g.png)

## Task 6: Create a Dashboard in Grafana


![Task 6 Image](images/task6b.png)

Imported  Resources Overview
![Task 6 Image](images/task6c.png)
![Task 6 Image](images/task6r.png)
Imported Key vaults
![Task 6 Image](images/task6d.png)
