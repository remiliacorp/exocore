---
layout: article
category: article
subtitle: 
topic:
date: 2022-04-16
tags: meta exocore computers learning test
---

# Set up a Custom Domain

Custom domains can be added for a better look and more memorable url, but you will need to purchase one. If you already have a domain, follow the steps in [Configuring a Domain Purchased Elsewhere](#configuring-a-domain-purchased-elsewhere) 

## Purchase Domain on Netlify

If you do not already have a domain, you can purchase it directly within Netlify by adding in a new Custom domain. Prices aren't the best on the market (e.g. `.com` is $15/yr, market rate is $12/yr), but it will automate all setup.

1. Navigate to Settings > Domain Management > Add custom domain.
2. Enter the domain you would like
3. If it is unavailable, you will see `[domain] already has an owner. Is it you?`. Select `No, try another`.
4. If you find one that is available, you will be provided prices and option to register. You can use a [Domain search tool](https://domains.google.com/registrar/search) to help find available domains.

Once you have a domain purchased, Netlify will automate handling DNS configuration and SSL encryption, so your site will be fully ready to go on your domain.

## Purchasing a Custom Domain
 
Domains can be purchased from a variety of suppliers for affordable rates - a `.com` domain goes for about $12/year, though uncommon domains like `.xyz` can be found for as low as $2/year.

I can recommend [Google Domains](https://google.com/domains), I use it because it includes privacy protection and custom email aliases for free, and has an easy to navigate dashboard, as well as Google's very fast DNS. 

For uncommon domains and more competitive prices, [Namecheap](https://namecheap.com) is reliable - it also has a solid "Beast mode" search for finding rare domains.

### Configuring a Domain Purchased Elsewhere

If you purchase your domain elsewhere, you will need to configure your domain provider to point the domain to your Netlify site. Follow this guide: [Configure external DNS for a custom domain](https://docs.netlify.com/domains-https/custom-domains/configure-external-dns/). 

The steps on your domain provider's end will be different depending on your provider, look for something along the lines of "Create A or CNAME Record", "Point DNS to Domain" or "Manage DNS Records".

Then add the custom domain in Netlify:
1. Navigate to Settings > Domain Management > Add custom domain.
2. Enter the domain you would like `[domain] already has an owner. Is it you?`. Select `No, try another`.
3. If you find one that is available, you will see 
3. Select Yes, add domain

SSL (https) will be configured automatically.
