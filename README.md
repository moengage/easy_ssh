# arione
Role based easy ssh access


Prerequisites:
1. Create a CA authority server and generate new SSH key.
```
ssh-keygen -t rsa -b 4096 -C ‘Certificate authority’ -f cert-authority
```

Here `-t` for encryption type,  `-b` for number of bits, `-C` for comment and `-f` for filename of the key file.

__Note__: Make sure to secure key with a passphrase.

2. Create a bastion host:

To manage all users and their activities we can use bastion host. Configure using this:
https://aws.amazon.com/blogs/security/how-to-record-ssh-sessions-established-through-a-bastion-host/

