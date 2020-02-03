# Ubuntu

### Add user to group 

```bash
 $ sudo usermod -a -G groupName userName
 ```

### Check which group a certain user belongs to

```bash
 $ groups [username]
 ```

### Users list

```bash
 $ cut -d: -f1 /etc/passwd
 ```
