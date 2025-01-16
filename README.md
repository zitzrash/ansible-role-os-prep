# Ansible OS Preparation Role

This role prepares the OS for operation by performing the following tasks:
1. Encrypts the second disk in the system.
2. Encrypts the partition next to the root partition.
3. Disables C-state for all CPUs.
4. Switches CPU operation to performance mode.
5. Renames the active network interface to `net0`.
6. Displays CPU and Hyper-Threading information.

## Requirements
- Ansible 2.9 or higher.

## Usage
1. Update the `inventory` file with your server details and disk names.
2. Run the playbook:
   ```bash
   ansible-playbook -i inventory playbook.yml --diff
3. To run the playbook on specific server, instead of group, you can use `var_host` variable
   ```bash
   ansible-playbook -i inventory playbook.yml --diff --check --extra-vars "var_host=your_server"