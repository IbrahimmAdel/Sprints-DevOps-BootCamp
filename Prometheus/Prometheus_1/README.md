# Prometheus task 1
## 1) What are the different HTTP status codes and explain their meaning?
* 1xx - Informational : Request received / Processing
* 2xx - Success : Successfully received
* 3xx - Redirect : Further action must be taken
* 4xx - Client Error : Request doesn’t have what it needs
* 5xx - Server Error : Server fulfil the request
-----
## 2) What database is used by Prometheus?
- **TSDB** 'Time-Series DataBase'
-----
## 3) What is the difference between different metrics types ( counter, gauge, histogram)?
### **counter** :
- 'How many?'
- Counter is a fundamental way for tracking how often an event occurs within an application or service.
- An example of a counter metric is http_requests_total, which reports the running total of HTTP requests to an endpoint on an application or service.
### **gauge** :
- 'Current state of events'
- gauage is used to periodically take measurements or snapshots of a metric at a single point in time.

### **histogram** :
- 'How long?'
- A histogram samples observations (usually things like request durations or response sizes) and counts them in configurable buckets. It also provides a sum of all observed values.
-----
## 4) Install Prometheus on your local host or on a server in any cloud provider.
- Create EC2 instance
![](https://github.com/IbrahimmAdel/DevOps_sprints/blob/main/Prometheus/Prometheus_1/4.1.png)
- Install Prometheus on it 
![](https://github.com/IbrahimmAdel/DevOps_sprints/blob/main/Prometheus/Prometheus_1/4.2.png)
-----
## 5) Add any new target to prometheus.yaml file and apply any query on it using promql language. 
- Install CAdvisor on the EC2
![](https://github.com/IbrahimmAdel/DevOps_sprints/blob/main/Prometheus/Prometheus_1/5.1.png)
- Add CAdvisor to **scrape_configs** section in `/etc/prometheus/prometheus.yml`
![](https://github.com/IbrahimmAdel/DevOps_sprints/blob/main/Prometheus/Prometheus_1/5.2.png)
- apply query on CAdvisor using promql language
![](https://github.com/IbrahimmAdel/DevOps_sprints/blob/main/Prometheus/Prometheus_1/5.3.png)


