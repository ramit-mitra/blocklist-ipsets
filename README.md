![Last updated](https://img.shields.io/badge/Last%20updated%20at-Wed%20Aug%2031%2009:30%20AM%20UTC%202022-orange.svg?style=for-the-badge&logo=git)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ramit-mitra/blocklist-ipsets?color=green&logo=github&style=for-the-badge)

# **blocklist-ipsets**

An IP list of `bad actors` trying to exploit/abuse public infrastructure (like servers, websites, ssh endpoints, etc).   
`Published in public interest`.

### Features

- Generated from active exploits attempted on my servers
- Automated updates
- Opensource

### Objective

- Publish a consolidated list of active abusive IP address
- These IPs are being used to attack public servers using known sshd and other exploits
- This is a list containing IP addresses that should never be allowed to access your server/web applications (IMO)
- IP address blocking has become a common practice for webmasters who want to prevent their sites from being accessed by malicious visitors. This is especially useful for websites that offer services such as ecommerce, dating, or social networking.

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
- No warranty and/or liability

### Contribution

Please share your feedback and/or feature requess by opening an issue. Thankyou.

### Tags

- automation
- security
- blocklist
- exploits
- linux

<p align="center">
<br/>
<hr />
<img src="https://media.giphy.com/media/EOIHxXCGiPPIT2Xl9t/giphy.gif">
<hr />
</p>

