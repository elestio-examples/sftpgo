# SFTPGo on Elestio with CI/CD

<a href="https://dash.elest.io/deploy?source=cicd&social=dockerCompose&url=https://github.com/elestio-examples/sftpgo"><img src="deploy-on-elestio.png" alt="Deploy on Elest.io" width="180px" /></a>

Example CI/CD pipeline showing how to deploy SFTPGo on Elestio.

# Once deployed ...

You are now able to sign to the Admin UI here:
    
    https://[CI_CD_DOMAIN]/web/admin
    login: root
    password: [ADMIN_PASSWORD] (set in env var)

Warning: the admin accout is restricted to the admin UI and cannot connect by any other protocol.
Once logged in you can create users, then users will be able to login using FTP / SFTP / Webdav / web client ui.

FTP service will be available on:

    Host: [CI_CD_DOMAIN]
    FTP Port: 21
    SFTP Port: 2022
    Web client: https://[CI_CD_DOMAIN]
    Webdav URL: https://[CI_CD_DOMAIN]:4080/

Documentation: https://github.com/drakkan/sftpgo/tree/main/docs

REST API: https://github.com/drakkan/sftpgo/blob/main/docs/rest-api.md
