# We are creating a vurenavle AD env.

1. We edited this `C:\Windows\Tasks\secpol.cfg` file in win 11. 

2. We leave the domain from W01 and taked a snaoshot and then we rejoined.

3. This all rejoinig thing was a test.

4. We can use `net Users \domain` form workstation to see all the domain users.

5. To undo the changes we made, users and group deleting 
```
.\gen_ad.ps1 .\out.json -Undo
```