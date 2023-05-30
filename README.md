![Last updated](https://img.shields.io/badge/Last%20updated%20at-Tue%20May%2030%2007:50%20PM%20UTC%202023-orange.svg?style=for-the-badge&logo=git)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ramit-mitra/blocklist-ipsets?color=green&logo=github&style=for-the-badge)

---

# **blocklist-ipsets**

An IP list of `bad actors` trying to exploit/abuse public infrastructure (like servers, websites, ssh endpoints, etc). `Published in public interest`.

### Features

- Generated from active exploits attempted on my servers (`19730` detected IPs)
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

### Usage example

- Ban IPs from this list using UFW  
    - Gist - https://gist.github.com/ramit-mitra/f72b16b34099f85b3423bd32f63930c3
    - Use as: `curl -s  https://gist.githubusercontent.com/ramit-mitra/f72b16b34099f85b3423bd32f63930c3/raw/ufw_block_banned_ips.sh | bash`

- Ban IPs from this list using Fail2ban
    - Gist - https://gist.github.com/ramit-mitra/f5e9c4f9adc4a155ebcce2608bc50f39
    - Use as: `curl -s  https://gist.githubusercontent.com/ramit-mitra/f5e9c4f9adc4a155ebcce2608bc50f39/raw/block_banned_ips.sh | bash`

- Similar approach can be followed for other firewall/IDS/IPS solutions.  

- View the list of IPs
    ```
    curl https://raw.githubusercontent.com/ramit-mitra/blocklist-ipsets/main/rottenIPs.json | jq
    ```

### Disclaimer

- This data is generated from exploits attemped on my servers
- Provided for personal and commercial use
- No warranty and/or liability

### Contribution

Please share your feedback and/or feature request by opening an issue. Thankyou.

### Tags

- automation
- security
- blocklist
- exploits
- linux
- ufw
- iptables
- fail2ban

<p align="center">
    <br />
    <hr />
    <img alt="funny illustrative gif" src="https://media.giphy.com/media/fe4dDMD2cAU5RfEaCU/giphy.gif">
    <hr />
</p>


