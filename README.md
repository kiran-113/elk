Modify the .env file and enter strong password values for both the ELASTIC_PASSWORD and KIBANA_PASSWORD variables.

You must use the ELASTIC_PASSWORD value for further interactions with the cluster. The KIBANA_PASSWORD value is only used internally when configuring Kibana.

Create and start the three-node Elasticsearch cluster and Kibana instance:

docker-compose up -d
When the deployment has started, open a browser and navigate to http://localhost:5601 to access Kibana, where you can load sample data and interact with your cluster.
Stop and remove the deploymentedit
When you’re done experimenting, you can remove the network, containers, and volumes:

docker-compose down -v

