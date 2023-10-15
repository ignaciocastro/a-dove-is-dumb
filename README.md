<div align="center">
  <a href=https://adobe.is.dumb.bar><img src="https://github.com/ignaciocastro/adobe-is-dumb/blob/assets/header.jpg?raw=true"></a>
  <sub><sup>click to open</sup></sub>


[/127](https://adobe.is.dumb.bar/127 "Alternative using 127.0.0.1 instead of 0.0.0.0") [/cdn](https://adobe.is.dumb.bar/cdn "Served from jsDelivr") [/fastly](https://adobe.is.dumb.bar/fastly "Served from jsDelivr's Fastly mirror (对中国用户有用)") [/pihole](https://adobe.is.dumb.bar/pihole "Optimized for Pi-hole users (No IP before domain)")

_Latest update: Sat, 14 Oct 2023 20:45:36 UTC_

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
    - File name or URL: https://adobe.is.dumb.bar or https://adobe.is.dumb.bar/127
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
    - Address: https://adobe.is.dumb.bar/pihole
    - Comment: Adobe is dumb
3. Click "Add", then run `pihole -g` or update gravity online.
</details>

## Troubleshooting
### My prefered program is not letting me use the list!
This can happen with programs that do not support 301 redirects as the source URL. You can use the following direct URLs instead:

<details>
    <summary>List of direct URLs (Click to expand)</summary>

- Default: https://adobe.is.dumb.bar/list.txt
- Alternative (127.0.0.1): https://adobe.is.dumb.bar/127.txt
- CDN: https://cdn.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt
- Fastly: https://fastly.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt
- Pihole: https://adobe.is.dumb.bar/pihole.txt
</details>

### It was working fine and now I'm getting an "Unlicensed program" window! / I'm still getting the "Unlicensed program" window / I have a new subdomain to submit
Adobe tends to update their license subdomain every two weeks. Feel free to open [an issue](https://github.com/ignaciocastro/adobe-is-dumb/issues/new) if you already tried updating the list and nothing happened. It'd be appreciated if you could use Fiddler / Charles Proxy when opening the program, sort by _"/integritychecker/machineevents/v1"_ and include the subdomain it was requested from.

### I'm in a country where Github / Cloudflare is slow or blocked / 我所在的国家Github/Cloudflare速度慢或被屏蔽
jsDelivr URL should redirect you to a suitable mirror according to your latency / country. If you still can't access any option, please [open an issue](https://github.com/ignaciocastro/adobe-is-dumb/issues/new).

对于中国用户：cdn.jsdelivr.net此前曾在大陆遭到屏蔽。你可以试试这些替代品
<details>
    <summary>镜像列表（单击展开)</summary>
    
- Fastly镜像: [违约](https://fastly.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://fastly.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/127.txt) | [Pi-hole](https://fastly.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/pihole.txt)
- Gcore镜像: [违约](https://gcore.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://gcore.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/127.txt) | [Pi-hole](https://gcore.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/pihole.txt)
- Quantil镜像: [违约](https://quantil.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://quantil.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/127.txt) | [Pi-hole](https://quantil.jsdelivr.net/gh/ignaciocastro/adobe-is-dumb@latest/pihole.txt)
- Ghproxy: [违约](https://ghproxy.com/https://raw.githubusercontent.com/ignaciocastro/adobe-is-dumb/main/list.txt) | [备选方案（127.0.0.1)](https://ghproxy.com/https://raw.githubusercontent.com/ignaciocastro/adobe-is-dumb/main/127.txt) | [Pi-hole](https://ghproxy.com/https://raw.githubusercontent.com/ignaciocastro/adobe-is-dumb/main/pihole.txt)
</details>

## Acknowledgements
 - [eaaasun's CCStopper](https://github.com/eaaasun/CCStopper/)
##
 <div align="center"><img src="https://github.com/ignaciocastro/adobe-is-dumb/blob/assets/adobe.gif?raw=true"></div>