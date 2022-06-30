- ## Instalación y administración en Ubuntu
  ```bash
  #install
  sudo snap install emqx
  # Start emqx
  sudo emqx start
  # Check Status
  sudo emqx.ctl status
  # Stop emqx
  sudo emqx stop
  ```
- ## Dashboard
  http://localhost:18083
  User: admin
  Password: public
-
- ## Commands
  |Command|Description|
  |admins add <Username> <Password> <Tags>|Create admin account|
  |admins passwd <Username> <Password>|Reset admin password|
  |admins del <Username>|Delete admin account|
  ```bash
  #Create admin account
  emqx.ctl admins add root public test
  #Reset admin password
  emqx.ctl admins passwd root private
  #Delete admin account
  emqx.ctl admins del root
  ```