# ML Application Deployment Exercise

This repository contains playground material to get acquainted with SODALITE. We propose you to run a simple exercise consisting in automating the deployment of a distributed Machine Learning application. If you are a TOSCA expert and you are not interested in trying out the SODALITE IDE, you can follow the instruction available in Section "Deployment using xOpera CLI". Otherwise, follow the instructions in the next section.  

## Deployment using SODALITE IDE

To deploy with SODALITE IDE, firstly configure the IDE backends as specified in the exercise material. Then, set VM name and OpenStack (OS) credentials in the `aadm.inputs.yaml` inputs file, and deploy AADM. Details on how to do it are available in the `SODALITE Experiments User Manual.pdf`. 

## Deployment using xOpera CLI

To deploy with xOpera CLI, firstly complete `tosca.inputs.yaml` file, specifying keypair name, public key, VM name and OpenStack (OS) credentials, and then execute:

```
$ opera deploy -i tosca.inputs.yaml ml-application.tosca.yaml
```

To view the outputs, e.g. public IP address of the VM, execute:

```
$ opera outputs
```

