### Automate SSH login with password:
**Windows** 

[source](https://www.chrisjhart.com/Windows-10-ssh-copy-id/)

```
# Generate an SSH Key
ssh-keygen -t rsa -b 2048

# Copy SSH Key to Remote Linux Device
type $env:USERPROFILE\.ssh\id_rsa.pub | ssh {id@server} "cat >> .ssh/authorized_keys"

# Test 
ssh {id@server}
```

**Linux** 

[source](https://serverfault.com/questions/241588/how-to-automate-ssh-login-with-password)

```
# Generate an SSH Key
ssh-keygen -t rsa -b 2048

# Copy your keys to the target server
ssh-copy-id {id@server}

# Test
ssh {id@server}
```
