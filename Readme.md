### Ansible Playbook Documentation

#### Prequisites:

1. **Install Ansible:**
   - Ansible must be installed on your server. Follow the official documentation for installation instructions: [Ansible Installation Guide](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

2. **Modify Inventory File:**
   - Update the `inventory.ini` file with the details of the servers where you want to run the Ansible playbook.

3. **Establish Connection:**
   - Ensure that there is a stable and secure connection between your Ansible machine and all the target servers.
   - Test the connection to each server using tools like SSH to confirm accessibility.

4. **Update Variable in Playbook:**
   - Open the `playbook.yml` file and locate the variable `$dsnName`.
   - Modify its value according to your specific requirements. For example: 
     ```yaml
       $dsnName = "YourDataSource"
     ```

#### Running the Playbook:

After verifying that all prerequisites are met, follow these steps to execute the Ansible playbook:

1. **Navigate to the Playbook Directory:**
   ```bash
   cd /path/to/playbook
   ```

2. **Run the Playbook:**
   ```bash
   ansible-playbook -i inventory.ini playbook.yml
   ```

