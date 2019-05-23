# SSH

## Transfer protocols

### Commmon transfer protocols

- Hypertext Transfer Protocol (HTTP)
- File Transfer (FTP)
- Hypertext Transfer Protocol Secure (HTTPS)
- Secure Shell (SSH)

### SSH

- A way for computers to securely communicate with each sother
- high level encryted
- can remote into another computer
- can connect to remote servers
- tranfer files from computer to a remote server

```
ssh {user}@{host}
```

### Encryption definitions

- Symmetrical Encryption
  - One secret key for encyption and decryption
  - uses a key exchange algorithm
- Asymmetrical Encryption
  - Uses two separate keys, one for encryption and one for decryption (public, private)
- Hashing
  - another form of cryptography
  - Bcypt to provide hashing

### Path to decryption

1.  Diffie-Hillman Key Exchange
2.  Arrive at Symetric Key
3.  Make sure of no funny business (Hashing)
4.  Authenticate User (Password)
    - root / password (not the best solutions)

### Authenticate with local ssh key

It is better to use a local encryption key =>

<i>Change to .ssh directory</i>

```
cd ~/.ssh
```

<i>Create a new .ssh encryption key</i>

```
~/.ssh# ssh-keygen -C "myemail@gmail.com"
```

<i>Add a key to remote ssh</i>

```
~/.ssh# ssh-ad ~/.ssh/id_rsa_preferred_key
```

<i>Get authorized keys list</i>

```
~/.ssh# vim authorized_keys
```

<hr />

#### Resources:

https://www.makeuseof.com/tag/beginners-guide-setting-ssh-linux-testing-setup/

<b>Assymetric connection</b>

https://www.youtube.com/watch?v=NmM9HA2MQGI

https://www.youtube.com/watch?v=Yjrfm_oRO0w

https://www.youtube.com/watch?v=vsXMMT2CqqE&t=

https://www.youtube.com/watch?v=NF1pwjL9-DE
