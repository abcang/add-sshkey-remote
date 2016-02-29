add-sshkey-remote
--
Script to add the SSH key to the service.

## Support
* SSH Server
* Github
* Bitbucket

## Usage

```
Usage:
    add-sshkey-remote [command] [args]

Command:
    ssh [user@]<hostname> [-p|--path <path>]                   adding ssh keys to authorized_keys on remote host
    github <user> [-l|--label <label>] [-p|--path <path>]      adding ssh keys to github
    bitbucket <user> [-l|--label <label>] [-p|--path <path>]   adding ssh keys to bitbucket
```

Example:

```
$ ./add-sshkey-remote github ABCanG -l MainPC -p ~/.ssh/id_rsa.pub
```

## Known Issue
* Raw response is displayed after command execution.

## License
MIT License
