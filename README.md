## docker-credential-rbw

A docker credential helper based on rbw bitwarden client.

There are bitwarden helpers such as https://gitlab.com/eyJhb/docker-credential-bitwarden and https://github.com/jenbroek/bitwarden-helpers .

They use https://bitwarden.com/help/cli/ , which is stateless. As a consequence, getting the secret takes several seconds.

Using rbw agent, the operations are much faster.
