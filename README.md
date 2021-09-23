## Instructions
- Clone the code

    ```git clone https://github.com/Learning-Hub-by-Chetan-Talwar/ApacheRole```
- Move the Role to Default directory 

    ```mv ApacheRole /etc/ansible/roles```
- Create a playbook with below content to execute the role 

    ```
    ---
    - hosts: all
      tasks:
        - name: calling role
          include_role:
            name: ApacheRole
    ```
- To execute it run the below command

    ```ansible-playbook your_playbook_name```