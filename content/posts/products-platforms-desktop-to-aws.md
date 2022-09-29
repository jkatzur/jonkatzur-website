---
title: "Products & Platforms pt 2 - from Desktop Windows to AWS"
date: 2018-08-21T22:45:22-04:00
draft: false
---

**Rise of Windows & Enterprise Licensed Products**
The first wave of enterprise products built for mass adoption by office workers were built largely on top of the desktop computing platform of Windows (which of course Microsoft was able to build because of [IBM’s decision to let them own the OS](https://www.pcmag.com/archive/the-rise-of-dos-how-microsoft-got-the-ibm-pc-os-contract-286148)). Windows allowed developers to build products for the entire enterprise market regardless of the hardware they purchased. Developers could build for one platform and have a major market immediately open up to them. Domain expert products covered areas like computer aided design (AutoCAD), graphic design (Adobe), and financial analysis (Peachtree, etc…).

The competitive market in design provides a great lesson in products vs platforms in [Silicon Graphics](https://www.triplepundit.com/story/2012/fall-silicon-graphics/61346). They were founded as an end-to-end hardware & software solution for graphics processing and were used to build the special effects in movies like Jurassic Park. While they had the best end-to-end solution, they lost to competitors built on Windows.  They lost for two primary reasons: 1) The dramatic cost reduction of PCs; and 2) The rise of general purpose applications on Windows made the Windows PC a more attractive enterprise option.

For enterprise data, though, desktop Windows was not enough. Companies could utilize Windows servers, or, over time, utilize data warehouses like Teradata, Oracle, or DB2. These on-premise deployed appliances scaled to data volumes and concurrent user needs of large enterprises. They enabled businesses to pick a single strategic partner and build know-how and long-term relationships on top of it. CIOs had to make the BIG decision of which platforms to buy and install (torturously), and then would aim to get as much out of that platform, via incremental products as possible. That distribution channel allowed developers of enterprise applications could then tap in to these platforms, like SAP on Oracle hardware and Microstrategy with Teradata.

The key takeaways from the licensed era are:

1. Licensed products & platforms have massive fixed costs in upfront R&D and then near 100% unit margins. These companies must pick the right domains, nail launch and distribution, and execute on sales & marketing to drive revenue
2. Choosing the right platform to develop a product on is a hugely important decision to achieve distribution. Products that pick incorrectly lose
3. Given how challenging it was to install and deploy products in this era a key requirement was conviction that it would actually work
4. Platforms, over time, compete with companies who build on top of them when the value is there - see Excel market share over time below

It’s useful to realize that the shift from licensed products to the next phase was relatively recently, and many major enterprise players grew out of the licensed model.

**Software as a Service**
The original wave of SaaS companies - especially Salesforce, but including many giants like Zendesk, Docusign, Slack, Gsuite, ServiceNow, etc… were predicated on the idea that for many of your challenges you do not care how the company builds their products. The platform that supports this wave of SaaS products is the web browser itself (hat tip to Google for innovating to make it possible to build ever more robust browser-based applications). The advancement of the Web Browser enabled developers to move from building Desktop based solutions for Windows to building Browser based solutions while attaining great distribution.

The extent to which SaaS shifts the paradigm of enterprise computing cannot be overstated. In the prior licensed era, enterprises had to make a big decision about which platforms to adopt. CIOs would think of themselves as Oracle, SAP, Teradata, or Microsoft shops - that was the big decision - which platforms to install in my data center. There was substantial complexity to these operations and CIOs were very focused on reducing their cost basis and risk of new investment. New vendors added risk both from substantial upfront licensing fees, regardless of outcome, and risk the implementation would be successful at all, given all of the integration and custom development work required.

SaaS products dramatically reduced the risk on the CIO by

1. Lowering the upfront investment risk by moving to a recurring subscription model - often with relatively easy opt-out terms, at least for smaller engagement
2. Offloading implementation risk - by handling installation, integration, and maintenance via their systems and onboarding
These sea-changes led directly to the rise of User Experience as the dominant factor in winning / losing in SaaS. Companies and users freed (mostly - obviously there is nuance here) from the need to make massive upfront investments and ROI decisions are able to focus on driving the best user experience.

**Symbiotic Growth of SaaS, Public Clouds and Open Source**

As SaaS is growing, we see the beginning of Public Clouds, first with AWS. With the Browser as the distribution mechanism, SaaS companies could now more flexibly pick their development platform of choice. AWS, based on savvy investment early on, was perfectly positioned to be the development platform of choice. To meet developer needs AWS must be the easier way to build an application, starting with systems engineering that allowed developers to focus on building the initial application before architecting for scale.

To achieve this they built fantastic systems software. They also took on large fixed capital investments, and let developers pay out costs over time, based on usage, which aligns perfectly with the SaaS operating model. Developers could avoid the upfront investments that customers no longer wanted, and pay AWS only as their revenue ramped, an [Amazon Tax](https://stratechery.com/2016/the-amazon-tax/) of sorts. This tax means any service that competes with something a public cloud provider sells begins with a ~25% margin disadvantage (must either charge more or accept worse margins).

This incentive structure means AWS makes money from renting resources, not software. For developers software and resources are complements and financially AWS is incented to reduce the cost of software to grow the customer’s ability to buy resources. Further, AWS is focused on being the widest development platform, and thus want to enable communities of developers to thrive there. Taken together, AWS is inclined to embraced the open-source community (except when, of course, it’s building its own [direct competitors using its platform](https://aws.amazon.com/about-aws/whats-new/2017/04/aws-database-migration-service-adds-support-for-mongodb-and-amazon-dynamodb/) - like Microsoft with Excel). AWS aims to achieve vendor lock with the right combination of AWS-only services (e.g S3, Lamda, etc…).

Meanwhile, Google’s response to AWS’s lead was to make it dramatically easier to switch between the clouds, open-sourcing an internal tool renamed [Kubernetes](https://stratechery.com/2016/how-google-cloud-platform-is-challenging-aws/). This is Google’s attempt to reset the public cloud market around a neutral platform (Kubernetes), similar to how browsers enabled web products to overcome Microsoft’s hegemony. Similarly, Microsoft’s response to AWS is to [love Linux](https://cloudblogs.microsoft.com/windowsserver/2015/05/06/microsoft-loves-linux/), recognize Windows lost in the public cloud, and enable Azure to win with enterprises, especially those seeking hybrid cloud offerings and hands-on support.

The key takeaways on public clouds are:

1. Public clouds grew symbiotically with SaaS companies as the development platform of choice - enabled by browser based distribution
2. The public clouds have a natural tendency to drive cost of software down - and embrace open-source to achieve this
3. Developing on top of public clouds means paying a platform tax (begins with 25% disadvantage). This tax also shifts fixed cost to capital costs, making starting up easier by reducing economies of scale
4. The key platform race is between AWS-first and Kubernetes-first model. Kubernetes gives developers and enterprises more downstream choices, at the expense of some of the capabilities possible in AWS-first world (similar to Browser vs Desktop)