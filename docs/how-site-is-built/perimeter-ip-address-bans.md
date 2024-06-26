# IP Address banning
Three modules are used for IP Banning, with custom Perimeter settings.

This is done to prevent spammers from crawling the site for known Wordpress vulnerabilities.

## Perimeter
Allows for custom rule sets, comes with a default that has been modified by monitoring the system logs for abuse during the March 2024, and June 2024 Wordpress hacks.

**Config:** https://tndeaflibrary.nashville.gov/admin/config/system/perimeter
**Module:** https://www.drupal.org/project/perimeter

## Automatic Ban
Allows for log analysis of possible bot activity. Further review of these logs could assist in banning bot traffic.
**Config:** https://tndeaflibrary.nashville.gov/admin/config/people/autoban/analyze
**Module: ** 

## Advanced IP Address Bans
Allows for full IP block banning, custom banning time frames, and customizing the message displayed when banned.
**Config:** https://tndeaflibrary.nashville.gov/admin/config/people/advban

## IP Address Bans
Built in Core manual IP address banning tool. This was used prior to the Advanced IP ban module which allowed for full blocks of IP addresses instead of individuals.
**Config:** https://tndeaflibrary.nashville.gov/admin/config/people/ban
