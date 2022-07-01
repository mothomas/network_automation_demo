## network_automation_demo with Cisco CSR on EVE-NG
Setup a demo ospf topology using ansible playbooks. once the topology created in Eve-NG. 
 
  ### create interface and ospf config
     
    'ansible-playbook -i hosts.yml csr_ospf_demo_main.yml --tags create'
 
  ### backup interface and ospf config
  
    'ansible-playbook -i hosts.yml csr_ospf_demo_main.yml --tags backup'
  
  ### delete interface and ospf config
  
    'ansible-playbook -i hosts.yml csr_ospf_demo_main.yml --tags delete'
  

## Topology
![](https://github.com/mothomas/network_automation_demo/blob/master/images/csr_ospf.png)

## Ansible plugins reference
[ios_modules](https://docs.ansible.com/ansible/latest/collections/cisco/ios/index.html#plugin-index)
