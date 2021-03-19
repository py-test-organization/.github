# Workflow Templates


## Apps Deploy
To deploy an app, workflows `appDeployDev` and `appDeployProd` deploy their corresponding build to AWS.

Depending on the framework and needs, you will need to rename some variables. For example, for React applications, you will rename `APPS_DEVELOPER_ID` to `REACT_APP_APPS_DEVELOPER_ID`.

For each app, you will need to set in the repository's secrets
-  `APP_ID`

The published app will be available at `https://<BUCKET>/<APPS_DEVELOPER_ID>/<APP_ID>/<VERSION>/index.html`.
