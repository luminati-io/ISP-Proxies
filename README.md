# Bright Data ISP Proxies

[![Promo](https://github.com/luminati-io/ISP-Proxies/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://brightdata.com/proxy-types/isp-proxies?promo=github15)

## Overview
Utilize Bright Data's extensive [ISP proxy network](https://brightdata.com/proxy-types/isp-proxies) for secure, stable, and high-speed data collection with IPs sourced directly from ISPs.

- **700,000+ ISP IPs**
- **Static Residential IPs** with long-term stability
- **99.9% success rate**
- **HTTP(S) & SOCKS5 support**
- **Free Country-Level Targeting**

## Key Features
- **Global Reach**: Access ISP IPs across [multiple countries](https://brightdata.com/locations).
- **High Success Rates**: Up to 99.9% success in accessing websites.
- **Fast and Stable**: Low latency and reliable uptime with 99.99% network availability.
- **Exclusive IP Access**: Dedicated IPs for consistent connections.
- **Ethically Sourced**: All ISP proxies are obtained directly from ISPs and are compliant with GDPR and CCPA.

## Pricing Plans
- **Pay As You Go**: $15/GB for monthly commitment-free usage.
- **Monthly Subscriptions - Shared**:
  - **10 IPs**: $1.80/IP, $18/month + VAT.
  - **100 IPs**: $1.45/IP, $145/month + VAT.
  - **500 IPs**: $1.40/IP, $700/month + VAT.
  - **1,000 IPs**: $1.30/IP, $1300/month + VAT.
  - **Enterprise Plans**: Custom solutions for extensive data collection needs.
 
- **Monthly Subscriptions - Dedicated**:
  - **10 IPs**: $3.50/IP, $35/month + VAT.
  - **100 IPs**: $2.75/IP, $275/month + VAT.
  - **500 IPs**: $2.60/IP, $1300/month + VAT.
  - **1,000 IPs**: $2.50/IP, $2500/month + VAT.
  - **Enterprise Plans**: Custom solutions for extensive data collection needs.
 
- **Monthly Subscriptions - Pay/GB**:
  - $12.75/GB, $499/month + VAT.
  - $11.25/GB, $999/month + VAT.
  - $10.50/GB, $1999/month + VAT.
  - **Enterprise Plans**: Custom solutions for extensive data collection needs.


Sign up and get a dollar-for-dollar match on your first deposit, up to $500!

## Getting Started with ISP Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Manage IPs and configurations via Bright Data's Control Panel or API.
3. **Supported Languages**: Quick start guides provided for Python, Java, C#, Node.js, and Shell.

## Code Examples

### Python

```python
import sys

# Replace '[your customerID]', 'isp', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-isp", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-isp", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-isp:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## Integrations
Our ISP proxies are compatible with widely-used automation tools, including:

- [**Puppeteer**](https://brightdata.com/integration/puppeteer)
- [**Selenium**](https://brightdata.com/integration/selenium)
- [**Playwright**](https://brightdata.com/integration/playwright)
- [**AdsPower**](https://brightdata.com/integration/adspower)
- [**MultiLogin**](https://brightdata.com/integration/multilogin)

## Use Cases
Common applications for ISP proxies:

- [**eCommerce**](https://brightdata.com/use-cases/ecommerce): Track pricing and product availability.
- [**Social Media**](https://brightdata.com/use-cases/social-media-for-marketing): Monitor trends and engagement.
- [**Real Estate**](https://brightdata.com/use-cases/real-estate): Collect data on property listings.
- [**Travel**](https://brightdata.com/use-cases/travel): Compare travel deals across locations.

## FAQ

### What is an ISP Proxy?
ISP proxies are static residential IPs assigned to servers, allowing you to access content as if using a regular residential IP but with higher speeds and stability.

### How do ISP Proxies work?
ISP proxies use IPs directly from ISPs, enabling fast, reliable access to content from a residential perspective with the speed of datacenter connections.

### What are the benefits of using ISP Proxies?
ISP proxies offer the stability and anonymity of [residential IPs](https://brightdata.com/proxy-types/residential-proxies) along with the speed of datacenter IPs, ideal for tasks like web scraping, ad verification, and SEO monitoring.

### How are ISP Proxies used by businesses?
ISP proxies are popular for tasks like accessing restricted content, verifying ads, monitoring competitive sites, and quality assurance testing.

### Are Bright Data's ISP Proxies compliant?
Yes, all ISP proxies are ethically sourced and compliant with data protection laws, including GDPR and CCPA, ensuring responsible data practices.
