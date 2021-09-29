# Data for "There’s a Multibillion-Dollar Market for Your Phone’s Location Data "

This contains the data and methodology that we used for our story "[There’s a Multibillion-Dollar Market for Your Phone’s Location Data ](https://themarkup.org/privacy/2021/09/30/theres-a-multibillion-dollar-market-for-your-phones-location-data)."

We set out to shine some light on the murky industry that collects, aggregates, buys, sells and shares your mobile phone location data. The general public has likely never heard of most of the companies in this industry, so we made a list of the different companies that are part of the location data pipeline, from the phone in your hand to the hedge funds and U.S. government agencies that spend big money on this valuable data for a variety of different purposes.  

# Definitions

First, let’s start with some definitions. 

**Data brokers**: Companies that buy and sell data are often referred to as “data brokers,” which is often used as a catch-all term. Here’s a definition of the term from an eponymous [FTC report](https://www.ftc.gov/system/files/documents/reports/data-brokers-call-transparency-accountability-report-federal-trade-commission-may-2014/140527databrokerreport.pdf) on the subject:

> Companies that collect consumers’ personal information and resell or share that information with others.

We quickly learned that while some companies we found did match this description (and in many cases appeared on either [California](https://github.com/the-markup/investigation-data-broker-lobbying/blob/main/data/data_brokers/ca-data-brokers.csv) or [Vermont’s](https://github.com/the-markup/investigation-data-broker-lobbying/blob/main/data/data_brokers/vt-data-brokers.csv) official data broker registries), not every company fits this definition. 

**First party data**: This usually refers to data that has been granted from the person using the app to the app developer, with consent. It is considered the highest quality data, and the term appears frequently in marketing language, even though the definition often gets misused. 

**App developers**: These are the companies that actually write the code for apps downloaded onto phones. The user has a direct relationship with app developers, as they are the entity that users are permitting to access their data. 

**SDKs**: Software Development Kits. A general term for the tools and code provided by a company to enable and encourage developers to write code for a platform. For the purposes of this description, these are libraries of code, often made available for free to app developers to include in mobile phone apps. They may provide drop-in functionality to add new features, such as maps or navigation directions. In many cases SDKs are advertised as a way for developers to monetize their apps: free tools, in exchange for user data.  

**Aggregators**: These are companies that gather up raw location data from a variety of sources, usually from app developers. They sometimes have their own SDKs. Other times, they don’t strictly collect the data themselves, but amass huge collections of location data from hundreds of apps. They buy and sell data, and may refine it, aggregate it, or combine it with other data tailored for different industries, such as retail footfall traffic for malls, or public transportation for transit authorities.  

**Location intelligence firms**: These are usually firms selling specialized geolocation analyses to larger corporate clients, including hedge funds and venture capital and private equity firms. 
While they don’t offer access to raw movement and location data, they do create demand for this commodity from the top of the market. These firms often advertise their advanced AI and machine learning capabilities with slick dashboards and predictive tools based on historical data. 

**Alternative data**:  A term we saw frequently appears in the marketing materials for the higher end firms that are advertising to hedge funds and private equity firms. Location and movement data are often cited as examples of nontraditional alternative data, set apart from traditional financial information, that could give investors an edge with unusual exclusive insights.

# How We Decided What to Include

Here’s how we decided which firms to include in our list of 47 location data companies. Note: This list is not meant to be an authoritative catalog of all the businesses operating in this space, but rather a survey of dozens of some of the noteworthy interconnected firms that play different roles in the location data supply chain. 

If a company we encountered met at least one of the following criteria, we included it on our list: 
 
* A company that collects consumers’ mobile device location data from an app and resells, licenses, or shares this information with others 
* A company that obtains location data originating from consumers’ mobile devices where it doesn’t have a direct relationship with the consumer whose data it’s obtaining
* A company whose marketing language offers app developers the use of an SDK in exchange for monetization or access to location data
* A company that offers its location data for sale on data marketplaces or data directories
* A company that clearly states it is offering potential customers access to consumer location data derived from mobile devices

We did not include companies that were general consumer data companies, of which there many. We specifically looked for marketing language, product descriptions, and privacy disclosures that described access to location data that originated from mobile phones. 

Did we miss any? Write to us: [keegan@themarkup.org](mailto:keegan@themarkup.org) and [alfred@themarkup.org](mailto:alfred@themarkup.org)

# Data
[location-data-companies.csv](https://github.com/the-markup/location-data-industry/blob/master/location-data-companies.csv) - 26.2 KB. 48 rows. First row is the header.

[full_company_responses.docx](https://github.com/the-markup/location-data-industry/blob/master/full_company_responses.docx) - 350 KB. All of the responses from the companies we reached out to (DOCX).

[full_company_responses.pdf](https://github.com/the-markup/location-data-industry/blob/master/full_company_responses.pdf) - 142 KB. All of the responses from the companies we reached out to (PDF).

## Data Dictionary 

<table border="0" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th>Column</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>name</strong></td>
      <td>The name of the company.</td>
    </tr>
     <tr>
      <td><strong>website</strong></td>
      <td>The URL of the company website.</td>
    </tr>
     <tr>
      <td><strong>logo</strong></td>
      <td>The company logo.</td>
    </tr>
     <tr>
      <td><strong>narrative</strong></td>
      <td>Examples of marketing claims, or noteworthy reasons for inclusion on this list.</td>
    </tr>
     <tr>
      <td><strong>company_reponse</strong></td>
      <td>Selections from the company's response to The Markup’s request for comment.</td>
    </tr>
     <tr>
      <td><strong>privacy_email</strong></td>
      <td>The privacy email for removal and data access requests.</td>
    </tr>
    <tr>
      <td><strong>privacy_policy</strong></td>
      <td>TThe privacy policy page, with instructions for data removal or requests.</td>
    </tr>
       <tr>
      <td><strong>CA_broker</strong></td>
      <td>Does the company appear on California's official data broker registry?</td>
    </tr>
       <tr>
      <td><strong>VT_broker</strong></td>
      <td>Does the company appear on Vermont's official data broker registry?</td>
    </tr>
  </tbody>
</table>

## Licensing
Copyright 2021, The Markup News Inc.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.