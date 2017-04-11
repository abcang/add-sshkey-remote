add-sshkey-remote
--
Script to add the SSH key to the service.

## Support
* SSH Server
* Github
* Bitbucket
* GitLab

## Require
* curl

## Usage

```
Usage:
    add-sshkey-remote [command] [args]

Command:
ssh [user@]<hostname> [-p|--path <path>]                                        adding ssh keys to authorized_keys on remote host
github <user> [-l|--label <label>] [-p|--path <path>]                           adding ssh keys to github
bitbucket <user> [-l|--label <label>] [-p|--path <path>]                        adding ssh keys to bitbucket
gitlab <user> [-l|--label <label>] [-p|--path <path>] [-u|--url <gitlab_url>]   adding ssh keys to gitlab
```

Example:

```
$ ./add-sshkey-remote github abcang -l MainPC -p ~/.ssh/id_rsa.pub
```

For GitLab:
```
$ ./add-sshkey-remote gitlab abcang --url https://gitlab.mydomain.com
```

Use with curl:
```
$ curl -fsSL https://raw.githubusercontent.com/abcang/add-sshkey-remote/master/add-sshkey-remote | bash -s github abcang
```

## License
MIT License
