# Steps to create PS session 

Create PS Sessions

1. Start winRM services

```shell
Start-Service WinRM
```

2. Enable PS Remoting

```shell
Enable-PSRemoting
```

3. Make IP of Win 2022 static

4. Add that IP to TrustedHosts in Win 11

```shell
Set-Item wsman:\localhost\Client\TrustedHosts -value "IP address"
```

5. Add that IP PS Session 

```shell
new-PSSession -ComputerName "IP" -Credential (Get-Credentials)
```

6. Enter that PS Session

```shell
Enter-PSSession 1
```

