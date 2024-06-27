# Data Spaces in Huawei Cloud

## Need for Data Spaces
The unprecedented growth of digital economy in the past decade has to lead to many new data technologies such as
big data, data lakes, data mining, data analysis, business intelligence and many more. These aimed at ingesting vast amounts of complex data
and generate tangible information out of it. Data is also the foundational building block of AI and ML.

All such data processing and consumption techniques were applied mostly on datasets which were centrally hosted
and consumed mostly by the sole owners of the data. But with data becoming the new currency and asset,
the organizations who own data can increase its value only by sharing them across organizations, sectors, domains, borders, etc.

This has lead to the emergence of **data spaces** ecosystem which aims at building frameworks for
decentralized data sharing with the highest level of security, trust, governance and control.

## Complexities of Data Spaces

Even though the business value a data space brings is great, implementing such a data exchange platform is extremely challenging 
due to complexities at multiple levels.

Some major complexities worth mentioning are legal (such as data sovereignty, data protection, etc.), 
system interoperability, access controls, data quality, agreements between parties and highly available and scalable 
data exchange infrastructure. 

## Components in a Data Space

At a very high level, the technical implementation of data space consists of the following components.

1. **_Management Plane_** - It is component which operates and owns the data space infrastructure. 
2. **_Providers_** - The source data owners who wish to share their data.
3. **_Consumers_** - The participants in the ecosystem who wish to consume data from  providers.
4. **_Connector_** - The interfacing component of provider and consumer which takes care of integrating with the management 
plane and as well as exchange of data with the provider/consumer. 

Management plane is the central system in a data space which not only brings data providers and consumers together but 
also provides a way for these heterogeneous systems to integrate seamlessly and enforces a layer of governance of top. 

Providers register their data offers in the data catalog hosted in the management plane using the management plane APIs.

Consumers can then view the offers in the catalog and start a negotiation with the data provider and agree upon the contractual details 
and the channel through which the data can be transferred. 

The figure below depicts a high-level architecture of a data space.

![file](dataspace-highlevel-export.png)

## Standards for Data spaces

Due to multi-faceted complexities in implementing a data space, there are initiatives globally which aims at building 
standards in data spaces. 

[GAIA-X](https://www.bmwk.de/Redaktion/DE/Dossier/gaia-x.html) is a European initiative aimed at creating a federated, 
secure, and trustworthy data infrastructure for Europe. HUAWEI CLOUD is an active member of GAIA-X initiative and is 
working on implementing a GAIA-X/IDSA compatible data space to facilitate cross-border data exchange. 

[International Data Spaces Association (IDSA)](https://internationaldataspaces.org/) is an open, nonprofit organization, 
with members over 140 organizations from over 20 countries. 
They aim to develop standards and a reference architecture for international data spaces (IDS), 
including a governance model and adoption strategy. IDSA is also a day-1 member of, and contributes its knowledge to, Gaia-X.

### IDS Reference Architecture

Figure below shows the reference architecture of a data space provided by IDS.

![IDS Data Space Reference Architecture](idsa-ref-architecture.png)

The most important components of this reference architecture are

1. **_Connector_**: Connects the participant to a data space and its management layer.
2. **_Registration service_**: A management layer service to register and validate new participants.
3. **_Identity provider_**:  A management layer service to provide authentication and authorization services.
4. **_Catalog_**: A management layer service to register new data offers and view available offers.
5. **_Policy engine_**: Manages contracts between parties before exchanging data and enforces the agreed policies during data exchange.

> HUAWEI CLOUD has developed an in-house IDSA compatible connector called the [boot-x](https://www.boot-x.eu/) which is also listed in the official IDSA 
[data connector report](https://internationaldataspaces.org/data-connector-report/).

### Reference Implementation of IDS Standards

[Eclipse Dataspace Components](https://projects.eclipse.org/projects/technology.edc) is an open-source project hosted 
by the [Eclipse Foundation](https://www.eclipse.org/) which is actively developed by many organizations. 

The EDC will implement the International Data Spaces (IDS) standard as well as relevant protocols and requirements associated with Gaia-X, 
and thereby provide implementation and feedback to these initiatives. 
However, the EDC will be extensible in a way that it may support alternative protocols.

 

## Huawei Cloud as a Data Space Provider 
