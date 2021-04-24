# Jenkins

## Infrastructure as Code with Ansible

## Objective
Building Jenkins server, to deploye application on Kubernetes Cluster via CI/CD pipeline

### Maintainer
<table>
    <thead>
      <tr>
        <th>Name</th>
        <th>NUID</th>
      </tr>
    </thead>
    <tbody>
        <tr>
            <td>Akshay Babaji Phapale</td>
            <td>001316563</td>
        </tr>
        <tr>
            <td>Naresh Agrawal</td>
            <td>001054600</td>
        </tr>
    </tbody>
</table>

### Technology Stack
* AWS
* Ansible

### Prerequisites
* AWS CLI
* Ansible


### Build Instructions
- Run following commands in the root directory
```
 $ ansible-playbook -i hosts create.yml -v --extra-var "elastic_ip=<elastic_ip> instance_type=<nstance_type>"
```

<b>Note</b>: Change variables value according to need 

### Destroy Instruction 
```
 $ ansible-playbook terminate.yml -v --extra-var "elastic_ip=<elastic_ip> instance_type=<nstance_type>"
```