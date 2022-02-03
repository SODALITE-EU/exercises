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

To deploy with SODALITE IDE, firstly configure the IDE backends as specified in the exercise material. Then, set VM name and OpenStack (OS) credentials in the `aadm.inputs.yaml` inputs file, and deploy AADM.