# Day 27 Commands — Remote Access & File Transfer

1. **ssh** — Connects to a remote machine over an encrypted connection,
   giving you a shell session on that host as if you were sitting in
   front of it.

2. **ssh -p** — Connects to a remote host using a non-default port,
   overriding the standard port 22 that SSH normally listens on.

3. **ssh -i** — Connects using a specific private key file, instead of
   relying on the default key SSH would otherwise look for.

4. **ssh-keygen** — Generates a new public/private SSH key pair, used
   for passwordless, key-based authentication instead of typing a
   password every time.

5. **ssh-copy-id** — Copies your public key to a remote server's
   authorized_keys file automatically, setting up passwordless login in
   one command instead of doing it manually.

6. **scp** — Securely copies files between a local machine and a remote
   one (or between two remotes), using the same encrypted connection as
   SSH.

7. **sftp** — Opens an interactive, secure file transfer session with a
   remote host, similar to old-school FTP but encrypted, letting you
   browse and transfer files interactively.

8. **rsync** — Synchronizes files and directories between locations,
   only transferring the differences on subsequent runs — much more
   efficient than scp for repeated transfers of large directories.

9. **~/.ssh/config** — A configuration file that lets you define
   shortcuts and default settings (hostname, user, port, key) for
   specific SSH connections, so you don't have to type long ssh
   commands repeatedly.

10. **sshd_config hardening** — Refers to editing the SSH server's
    configuration file (/etc/ssh/sshd_config) to improve security —
    common changes include disabling root login and disabling password
    authentication in favor of keys only.
