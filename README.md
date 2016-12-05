# bluemix-todo-apps - node overview

TodoMVC using Cloudant and Compose for MongoDB services running on Bluemix.

## How it Works

1. Add items to the todo list by typing into the box and pressing `Enter`

2. Mark items as complete by clicking the checkmark to the left of the corresponding item.

3. Delete items by clicking the 'X' to the right of the corresponding item that appears on hover.

4. Edit existing todo items by double-clicking on the corresponding item.

## Running the app on Bluemix

1. Create a Bluemix Account

    [Sign up][bluemix_signup_url] for Bluemix, or use an existing account.

2. Download and install the [Cloud-foundry CLI][cloud_foundry_url] tool

3. Go on the Bluemix catalog and select nodeJS Runtime, remember the name of the application you just created, we will use it later

4. Click on the newly created app and go to the Connection section and hit Connect New. Create a new Compose for mongoDB service and remember the name of the service you just created, we will use it later

4. Clone the app to your local environment from your terminal using the following command

```
git clone https://github.com/hkgian/bluemix-node-todo.git
```

5. Change the directory to the node directory
```
cd node
```

6. Edit the manifest.yml file with the name of the application and the name of the Service

7. Push the application to Bluemix with the following commands, you need to be in the folder where the manifest file is located.
```
cf login -a https://api.eu-gb.bluemix.net
cf push
```









[bluemix_signup_url]: https://console.eu-gb.bluemix.net/registation
[cloud_foundry_url]: https://github.com/cloudfoundry/cli
[download_node_url]: https://nodejs.org/download/
[deploy_track_url]: https://github.com/cloudant-labs/deployment-tracker
