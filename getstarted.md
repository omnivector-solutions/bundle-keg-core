# Welcome to Omnivector Solutions' KEG Core Bundle!
Congratulations! You are deploying Omnivector Solutions' KEG Core bundle! {details_link}


# Begin Logging Now!
Following a successful deployment of this bundle, you will be able to start using the components of the keg stack to collect and interpret your logs immediately.

### Graylog
Visit the ip address of the Apache2 charm in your browser to access the Graylog UI.

The Graylog admin password can be retrieved by running the following command using your Juju client connected to this model:

```bash
juju run-action --wait graylog/0 show-admin-password
```

### Kibana
Visit the ip address of the Kibana charm in your browser to access the Kibana UI.

The Kibana admin password can be acquired by running the following command using your Juju client connected to the model in which this bundle is deployed:
```
juju config kibana kibana-password
```

### Elasticsearch
Connect to Elasticsearch from your own application by opening up a connection to `http://<ip-address>:9200>` using the client of your choosing.

# Connecting Other Services
In the case you are connecting other charmed services, the Elasticsearch charm used by this bundle exposes a `client` interface that other charms can relate to.
More information on the elasticsearch-client interface can be found [here](https://github.com/omnivector-solutions/interface-elasticsearch).

Similarly, all of the charms used in this bundle expose endpoints that allow you to programmatically integrate a suite of custom services/applications.


## Contact
* [Omnivector Solutions](https://www.omnivector.solutions) <info@omnivector.solutions>

