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
    ssh [user@]hostname       adding ssh keys to authorized_keys on remote host
    github user [label]       adding ssh keys to github
    bitbucket user [label]    adding ssh keys to bitbucket
    help                      print this
```

Example:

```
$ ./add-sshkey-remote github ABCanG MainPC
```

## Known Issue
* Raw response is displayed after command execution.

## License
MIT License
