# ML Application Deployment Exercise

## Deployment using xOpera CLI

To deploy with xOpera CLI, firstly complete `tosca.inputs.yaml` file, specifying keypair name, public key, VM name and OpenStack (OS) credentials, and then execute:

```
$ opera deploy -i tosca.inputs.yaml ml-application.tosca.yaml
```

To view the outputs, e.g. public IP address of the VM, execute:

```
$ opera outputs
```

## Deployment using SODALITE IDE

To deploy with SODALITE IDE, firstly configure the IDE backends as specified in the exercise material. In the `ml-application.aadm` set the module value as your username or namespace. Then, fetch xOpera REST API's public key:

```
$ curl -X 'GET' \
  'https://xopera-rest-api.public-testbed.sodalite.eu/ssh/keys/public' \
  -H 'accept: application/json'
```

Set this public key in the inputs: `aadm.inputs.yaml` along with the keypair name, VM name and OpenStack (OS) credentials, and deploy AADM.