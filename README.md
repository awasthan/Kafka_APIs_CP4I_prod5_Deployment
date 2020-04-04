# Kafka_APIs_CP4I_prod5_Deployment
This job is parameterized. The jenkinsfile reads below parameter values from the job
1) imagename: Name of the image that you would build by baking in the BAR files on base image
2) tag: Tag of the image that you would build and push to OCP registry
3) OCP_Registry_External_URL: Externally accesible url of the OCP registry. For example "default-route-openshift-image-registry.apps.prod5.os.fyre.ibm.com". Enter without http/https.
4) OCP_Registry_Internal_URL: Internal URL of the OCP registry. For example "image-registry.openshift-image-registry.svc:5000"
5) DeploymentType: This is a 'choice' parameter. Possible values are 'install' and 'upgrade' here.
6) ReleaseName: Name of the helm release
7) ACE_APP1: Name of first ACE application for which BAR file is pulled from Nexus repository
8) ACE_APP1_VERSION: Version number of the BAR file of ACE_APP1 to pull
9) ACE_APP2: Name of second ACE application for which BAR file is pulled from Nexus repository
10) ACE_APP2_VERSION: Version number of the BAR file of ACE_APP2 to pull
11) ICP_CONSOLE_URL: Cloud Pak Foundation url
12) HELM_CERT_FILE_NAME: Name of helm certificate file
13) IMAGE_PULL_SECRET: Image pull secret to pull images from specified namespace
14) IntegrationServerName: Name of Integration Server
15) Namespace: Namespace
16) CP4I_User: CP4I User having permission for deployment
17) CP4I_Password: Password of CP4I user
