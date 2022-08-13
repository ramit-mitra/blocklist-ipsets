# blocklist-ipsets
An IP list of bad actors exploiting public infra like website, ssh endpoints, etc.

### Features
- Generated from active exploits attempted on my servers
- Actively updated
- Opensource

### Objective
- Publish a consolidated list of active abusive IP address
- These IPs are being used to attack public servers using known sshd and other exploits
- This is a list containing IP addresses that should never be allowed to access your server/web applications (IMO)

### Use cases
- Improve your security by blocking all access from these IP adresses to your infrastructure
- Block requests to your web application originating from these IPs (high chance that these IPs will be used to exploit/abuse your web applications)

### File list
- `rottenIPs.json` - Consolidated list of abusive IP addresses (as JSON file)

### Usage
```
curl https://raw.githubusercontent.com/ramit-mitra/blocklist-ipsets/main/rottenIPs.json | jq
```

### Disclaimer
- This data is generated from exploits attemped on my servers
- Provided for personal and commercial use

### Contribution
Please share your feedback and/or feature requess by opening an issue. Thankyou. 
