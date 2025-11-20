<div align="center">
  <a href=https://a.dove.isdumb.one><img src="https://cdn.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@assets/header.jpg"></a>
  
  <sub><sup>click to open</sup></sub>


[/127](https://a.dove.isdumb.one/127 "Alternative using 127.0.0.1 instead of 0.0.0.0") [/cdn](https://a.dove.isdumb.one/cdn "Served from jsDelivr") [/fastly](https://a.dove.isdumb.one/fastly "Served from jsDelivr's Fastly mirror (对中国用户有用)") [/pihole](https://a.dove.isdumb.one/pihole "Optimized for Pi-hole users (No IP before domain)") [/winhosts](https://a.dove.isdumb.one/winhosts "Follows Microsoft Windows' default hosts file format") [/ipv6](https://a.dove.isdumb.one/ipv6 "List for IPv6 blocking") [/clash](https://a.dove.isdumb.one/clash "Formatted for Clash-based programs")

_Latest update: Thu, 20 Nov 2025 07:23:09 UTC_

<sub>_NEW: Join the Telegram channel for updates [here](https://a.dove.isdumb.one/telegram)._</sub>


Quick, easy and painless way of blocking Adobe's telemetry checking servers. Updated continuously, without blocking other network-required features.</div>

## Usage

<details>
<summary>Normal usage (manual updates)</summary>

- Copy the contents from the list to your hosts file, located in C:/Windows/System32/drivers/etc/hosts.
- If your hosts file is the default one, you can use the Windows formatted list and copy and paste everything instead
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
    - Auto refresh: 1 hour
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
- CDN: https://cdn.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/list.txt
- Fastly: https://fastly.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/list.txt
- Pihole: https://a.dove.isdumb.one/pihole.txt
- Microsoft Windows hosts: https://a.dove.isdumb.one/winhosts.txt
- IPV6-format blocking: https://a.dove.isdumb.one/ipv6.txt
</details>

### It was working fine and now I'm getting / I'm still getting the red banner pop-up / I have a new subdomain to submit
Adobe tends to update their telemetry checking subdomain every two weeks. Feel free to open [an issue](https://github.com/ignaciocastro/a-dove-is-dumb/issues) if you already tried updating the list and nothing happened. Use Fiddler / Charles Proxy when opening the program, sort by _"/integritychecker/machineevents/v1"_ and include the subdomain it was requested from. **Please include the URL as text instead of just pasting a screenshot**, your submission will be rejected if you don't paste the URL.

### I'm in a country where Github / Cloudflare is slow or blocked / 我所在的国家Github/Cloudflare速度慢或被屏蔽
jsDelivr URL should redirect you to a suitable mirror according to your latency / country. If you still can't access any option, please [open an issue](https://github.com/ignaciocastro/a-dove-is-dumb/issues).

对于中国用户：cdn.jsdelivr.net此前曾在大陆遭到屏蔽。你可以试试这些替代品
<details>
    <summary>镜像列表（单击展开)</summary>
    
- Fastly镜像: [违约](https://fastly.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://fastly.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/127.txt) | [Pi-hole](https://fastly.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/pihole.txt) | [Microsoft Windows hosts](https://fastly.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/winhosts.txt) | [IPv6格式阻止](https://fastly.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/ipv6.txt)
- Gcore镜像: [违约](https://gcore.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://gcore.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/127.txt) | [Pi-hole](https://gcore.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/pihole.txt) | [Microsoft Windows hosts](https://gcore.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/winhosts.txt) | [IPv6格式阻止](https://gcore.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/ipv6.txt)
- Quantil镜像: [违约](https://quantil.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/list.txt) | [备选方案（127.0.0.1)](https://quantil.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/127.txt) | [Pi-hole](https://quantil.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/pihole.txt) | [Microsoft Windows hosts](https://quantil.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/winhosts.txt) | [IPv6格式阻止](https://quantil.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@latest/ipv6.txt)
- Ghproxy: [违约](https://gh-proxy.com/https://raw.githubusercontent.com/ignaciocastro/a-dove-is-dumb/main/list.txt) | [备选方案（127.0.0.1)](https://gh-proxy.com/https://raw.githubusercontent.com/ignaciocastro/a-dove-is-dumb/main/127.txt) | [Pi-hole](https://gh-proxy.com/https://raw.githubusercontent.com/ignaciocastro/a-dove-is-dumb/main/pihole.txt) | [Microsoft Windows hosts](https://gh-proxy.com/https://raw.githubusercontent.com/ignaciocastro/a-dove-is-dumb/main/winhosts.txt) | [IPv6格式阻止](https://gh-proxy.com/https://raw.githubusercontent.com/ignaciocastro/a-dove-is-dumb/main/ipv6.txt)
</details>


### Donations
They are not necessary, but always appreciated! Your contribution will help me pay for the API services I use to continuously find subdomains, plus the yearly domain price.

<div align="center">

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F2F2PQN55)
[![buymeacoffee](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://buymeacoffee.com/ignaciocastro)

[Github Sponsors (+crypto wallets)](https://github.com/sponsors/ignaciocastro)

</center>

##
 <div align="center"><img src="https://cdn.jsdelivr.net/gh/ignaciocastro/a-dove-is-dumb@assets/a-dove.png"></div>
