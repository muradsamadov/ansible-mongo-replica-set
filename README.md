## Execution

` ansible-playbook main.yml -i inventory.txt `

## Change mongod.conf file

If you want to change and deploy something in the mongod.conf file:

` ansible-playbook main.yml -i inventory.txt --tags "copy_mongod.conf" `

> Notes: During the execution of the above playbook, the mongo service will be restarted via the tags module.
