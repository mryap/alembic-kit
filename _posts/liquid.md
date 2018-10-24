

Static Site like Jekyll (also running this site) uses the Liquid templating language to process templates.

[Liquid](https://shopify.github.io/liquid/) is used by Salesforces, Shopify , Drip etc. https://github.com/Shopify/liquid/wiki#who-uses-liquid 

| <p>  |                                                              |
| ---- | ------------------------------------------------------------ |
|      | {% if customer.clearbit-employment_role == "marketing" %}    |
|      | As marketers, it’s our job to manage personalized email at scale through our tools, and to coordinate with every other team (and all their tools) that are possibly sending email. Sales, product, support… |
|      | {% elsif customer.clearbit-employment_role == "sales" %}     |
|      | Sales needs to work alongside marketing, product to avoid overwhelming people just as deals are moving forward — when reps send personal emails, that <em>must</em> sync in with everything else. Sales email > <em>everything else</em>. |
|      | {% endif %}                                                  |
|      | </p>                                                         |

So What?

Liquid templating  enable more flexible logic to determine which variation of content they might see. This means personalisation! 

`{% if customer. employment_role == "marketing" %}` 
`As marketers, it’s our job to manage personalized email at scale through our tools, and to coordinate with every other team (and all their tools) that are possibly sending email. Sales, product, support…`
`{% elsif customer. employment_role == "sales" %}` 
`Sales needs to work alongside marketing, product to avoid overwhelming people just as deals are moving forward — when reps send personal emails, that <em>must</em> sync in with everything else. Sales email > <em>everything else</em>.`