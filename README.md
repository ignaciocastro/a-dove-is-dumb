<!-- GitAds-Verify: D8XCGD6HK69NEG5ETORD7S4H64UFBXZZ -->

# Please switch your domains to a.dove.isdumb.one. Old domain will be retired. Read more [here](https://github.com/ignaciocastro/adobe-is-dumb/issues/13)
<div align="center">
  <a href=https://a.dove.isdumb.one><img src="https://github.com/ignaciocastro/adobe-is-dumb/blob/assets/header.jpg?raw=true"></a>
  
  <sub><sup>click to open</sup></sub>


[/127](https://a.dove.isdumb.one/127 "Alternative using 127.0.0.1 instead of 0.0.0.0") [/cdn](https://a.dove.isdumb.one/cdn "Served from jsDelivr") [/fastly](https://a.dove.isdumb.one/fastly "Served from jsDelivr's Fastly mirror (对中国用户有用)") [/pihole](https://a.dove.isdumb.one/pihole "Optimized for Pi-hole users (No IP before domain)")

_Latest update: Sun, 09 Jun 2024 13:47:03 UTC_

<sub>_NEW: Please switch your domains to a.dove.isdumb.one. Old domain will be retired. Read more [here](https://github.com/ignaciocastro/adobe-is-dumb/issues/13)._</sub>


Quick, easy and painless way of blocking Adobe's licensing servers. Updated continuously, without blocking other network-required features.</div>


## Usage

<details>
<summary>Normal usage (manual updates)</summary>

- Copy the contents from the list to your hosts file, located in C:/Windows/System32/drivers/etc/hosts.
</details>

<details>
    <summary>HostsMan users (Automatic updates)</summary>

- HostsMan users can't use CDN / Pi-hole URLs because of the program's request headers requirements.

1. Open HostsMan as Administrator
2. Click on Hosts > Manage Update Sources -> Add source
3. Fill with the following information
    - Name: Adobe is dumb
    - File name or URL: https://a.dove.isdumb.one or https://a.dove.isdumb.one/127
    - Name of hosts file: Leave blank
    - Import Comments: Enabled
    - Import Possible Hijacks: Use global settings
4. Click on OK > Close > Configure Updater
5. Check "Automatically check and download new hosts file updates", Apply > Ok
6. Click on "Check for Updates"
</details>

<details>
    <summary>SwitchHosts users (Automatic updates)</summary>

1. Open SwitchHosts as administrator
2. Click on + > Select Hosts type as "Remote"
3. Fill with the following information
    - Hosts title: Adobe is dumb
    - File name or URL: Any URL available at the beggining (CDNs included)
    - Auto refresh: 24 hours if using normal URLs, 1 hour if using CDNs
4. Click on OK > Right click on the name > Refresh
5. Click on the toggle to enable it
</details>

<details>
    <summary>hostsmgr users (Automatic updates)</summary>

1. Add your prefered URL to hosts_sources.dat
2. Run hostsmgr to update
</details>

<details>
    <summary>Pi-Hole users (Automatic updates)</summary>

1. Open the Pi-hole dashboard > Adlists
2. Fill with the following information
    - Address: https://a.dove.isdumb.one/pihole
    - Comment: Adobe is dumb
3. Click "Add", then run `pihole -g` or update gravity online.
</details>

## Troubleshooting
### It's been X hours/days/weeks/months since this last updated! Is this list deprecated / abandoned?
Not at all. This list is usually weeks ahead of Adobe's domain switches, so it doesn't need to continuously update. The only times you'll see a recent push would be:
- If they add more domains and I can add them as preventive updates
- If they make a switch between domain formats (Moving from _*.adobe.io_ to _*.prod.cloud.adobe.io_, for example.)

### My prefered program is not letting me use the list!
This can happen with programs that do not support 301 redirects as the source URL. You can use the following direct URLs instead:

<details>
    <summary>List of direct URLs (Click to expand)</summary>

- Default: https://a.dove.isdumb.one/list.txt
- Alternative (127.0.0.1): https://a.dove.isdumb.one/127.txt
- CDN: https://cdn.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt
- Fastly: https://fastly.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt
- Pihole: https://a.dove.isdumb.one/pihole.txt
</details>

### It was working fine and now I'm getting / I'm still getting the "Unlicensed program" window / I have a new subdomain to submit
Adobe tends to update their license subdomain every two weeks. Feel free to open [an issue](https://github.com/ignaciocastro/adobe-is-dumb/issues/new) if you already tried updating the list and nothing happened. It'd be appreciated if you could use Fiddler / Charles Proxy when opening the program, sort by _"/integritychecker/machineevents/v1"_ and include the subdomain it was requested from.

### I'm in a country where Github / Cloudflare is slow or blocked / 我所在的国家Github/Cloudflare速度慢或被屏蔽
jsDelivr URL should redirect you to a suitable mirror according to your latency / country. If you still can't access any option, please [open an issue](https://github.com/ignaciocastro/adobe-is-dumb/issues/new).

对于中国用户：cdn.jsdelivr.net此前曾在大陆遭到屏蔽。你可以试试这些替代品
<details>
    <summary>镜像列表（单击展开)</summary>
    
- Fastly镜像: [违约](https://fastly.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://fastly.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/127.txt) | [Pi-hole](https://fastly.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/pihole.txt)
- Gcore镜像: [违约](https://gcore.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://gcore.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/127.txt) | [Pi-hole](https://gcore.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/pihole.txt)
- Quantil镜像: [违约](https://quantil.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://quantil.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/127.txt) | [Pi-hole](https://quantil.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/pihole.txt)
- Ghproxy: [违约](https://gh-proxy.com/https://raw.githubusercontent.com/ignaciocastro/adobe-is-dumb/main/list.txt) | [备选方案（127.0.0.1)](https://gh-proxy.com/https://raw.githubusercontent.com/ignaciocastro/adobe-is-dumb/main/127.txt) | [Pi-hole](https://gh-proxy.com/https://raw.githubusercontent.com/ignaciocastro/adobe-is-dumb/main/pihole.txt)
</details>

### Donations
They are not necessary, but always appreciated! Your contribution will help me pay for the API services I use to continuously find subdomains, plus the yearly domain price.

<div align="center">

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F2F2PQN55)
[![liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/ignaseeo/)

[![githubsponsor](https://github.com/ignaciocastro/adobe-is-dumb/blob/assets/githubsponsor.svg?raw=true)](https://github.com/sponsors/ignaciocastro)

</center>

##
 <div align="center"><img src="https://github.com/ignaciocastro/adobe-is-dumb/blob/assets/adobe.png?raw=true"></div>
