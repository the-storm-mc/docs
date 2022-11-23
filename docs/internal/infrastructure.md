# Infrastructure

The Minecraft servers and LiveMap are hosted on OVH. We use a `KS-GAME-1` server.

Specs:

-   CPU: Intel Core i7-4790K - 4c/8t - 4 GHz/4.4 GHz
-   Memory: 16 GB 1600 MHz
-   Storage: 1×240 GB SSD SATA
-   Network: 100 MiB/s symmetrical
-   OS: Debian 11 (Bullseye)
-   Location: Canada

<figure markdown>
  ![Screenshot of the OVH UI](/assets/images/ovh.png){ width="550" }
  <figcaption>This machine is where everything happens!</figcaption>
</figure>

Our websites are hosted with [Netlify](https://www.netlify.com/).

<figure markdown>
  ![Screenshot of the Netlify UI](/assets/images/netlify.png){ width="550" }
  <figcaption>Netlify hosts our docs and homepage</figcaption>
</figure>

Our domain is registerd with [Google Domains](https://domains.google/) with DNS nameservers at [AWS Route53](https://aws.amazon.com/route53/).

<figure markdown>
  ![Screenshot of the Google Domains UI](/assets/images/google-domains.png){ width="550" }
  <figcaption>Our domain at Google Domains</figcaption>
</figure>

<figure markdown>
  ![Screenshot of the Route53 UI](/assets/images/route53.png){ width="550" }
  <figcaption>Our DNS configuration at Route53</figcaption>
</figure>
