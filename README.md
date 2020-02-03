# Ubuntu

### Add user to group 

```bash
 $ sudo usermod -a -G groupName userName / adduser username groupName 
 ```

### Check which group a certain user belongs to

```bash
 $ groups [username]
 ```

### Users list

```bash
 $ cut -d: -f1 /etc/passwd
 ```
 
  ### Add user

```bash
 $ sudo adduser new_username / sudo useradd new_username
 ```
 
 
  ### Remove user

```bash
 $ sudo userdel username 
 ```
 
 
  ### Change the password for a user

```bash
 $ sudo passwd username 
 ```
