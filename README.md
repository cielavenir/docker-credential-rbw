## docker-credential-rbw

A docker credential helper based on [rbw](https://github.com/doy/rbw) bitwarden client.

There are bitwarden helpers such as https://gitlab.com/eyJhb/docker-credential-bitwarden and https://github.com/jenbroek/bitwarden-helpers .

They use https://bitwarden.com/help/cli/ , which is stateless. As a consequence, getting the secret takes several seconds.

Using rbw agent, the operations are much faster.

All store|get|erase|list|version subcommands are implemented.

## Folder Name

The credentials should go into a folder, which must be pre-created.

The name can be specified by envvar BWHELPER\_DOCKER (from jenbroek/bitwarden-helpers) or DOCKER\_BITWARDEN\_FOLDER (from eyJhb/docker-credential-bitwarden).

If not specified, the default value is `docker-creds`.
