# Study Overview
By Joseph Castle, PhD, Code.gov <sup>[1](#fn1)</sup>

*This write-up summarizes portions of the [Federal Source Code Study (FSCS)](https://github.com/GSA/code-gov/blob/master/docs/FederalSourceCodeStudy/FederalSourceCodeStudy.pdf), a three-year study conducted from 2017 to 2020 by the Code.gov team to better understand agency implementation of the Federal Source Code Policy (FSCP). The study considered open source software (OSS) publication as one indicator of FSCP implementation and examined why some agencies publish OSS and others do not.*

Series ToC:
- Study Overview
- [History of OSS](history_of_OSS.md)
- [Federal Government's Intersection with OSS](govt_intersection_OSS.md)
- [Cultural Beliefs](cultural_beliefs.md)
- [Public Engagement](public_engagement.md)

--forthcoming--
- [Structural Dimensions](#)
- [Organizational Location](#)
- [Analysis of Organizational Factors & OSS Publishing](#)
- [Implications & Recommendations for Public Administrators](#)

---

## Towards a Federal Source Code Policy

> Computer software (SW) is essential for the daily operations of industry and government. “More and more major businesses and industries are being run on software – from movies to agriculture to national defense”. <sup>[2](#fn2)</sup>

The federal government spends approximately six billion dollars on SW each year <sup>[3](#fn3)</sup>, representing 7% of the [information technology (IT) budget](https://itdashboard.gov/) of the [Chief Financial Officers (CFO) Act agencies](https://en.wikipedia.org/wiki/Chief_Financial_Officers_Act). <sup>[4](#fn4)</sup>

Agencies purchase SW and customize as needed, often leading to SW purchasing and support that is costly, allows for little to no reuse, results in duplication of effort and spending across agencies, and overall yields poor quality. <sup>[5](#fn5) </sup><sup>[6](#fn6)</sup>

In 2016, in response to software purchasing and reuse inefficiencies, the White House issued the [Federal Source Code Policy: Achieving Efficiency, Transparency, and Innovation through Reusable and Open Source Software](https://sourcecode.cio.gov/) or the FSCP. 

The FSCP directed CFO Act agencies to do three things: 
1. Create an agency source code policy; 
2. Update acquisition language to capture new custom code; and, 
3. Create a source code inventory and publish at least 20% as open source software (OSS). 

The FSCP also established the Code.gov program and technical platform including a [website](https://code.gov/) and [application programming interface (API)](https://open.gsa.gov/api/codedotgov/).

## Organizational Factors Affecting OSS Publication

As an initial step to understanding FSCP implementation and OSS publication, we used the [GitHub API](https://developer.github.com/v3/) to gather metadata pertaining to agency public coding activities. This metadata showed agencies were publishing OSS with mixed results before and after publication of the FSCP. We wondered why some agencies could publish OSS and other agencies could not when every agency has the following characteristics to support OSS publication.

- An inherent mandate to serve the public by being transparent and release public funded products (as appropriate with consideration to security, privacy, etc.).
- Requirements dictated by the FSCP enforcing compliance to publish OSS.
- An IT budget with a portion devoted to SW development.
- IT specialists and contractors with technical skills who regularly work with SW.

With similar agency capabilities for publishing OSS, arguably all agencies should have been publishing OSS, but they were not. This led us to believe there were  systemic organizational factors with code publication. Therefore, the premise of the study centered on broader organizational factors related to organizational cultural beliefs, public engagement, structural dimension, and organization location either hindering or aiding agency OSS publication.

## Study Description

The qualitative study included a metadata analysis, interviews, and artifact collection (e.g., SOPs, organization charts). The sample contained the following attributes.

- 25 participants were from SW development units in 20 of 24 CFO Act agencies. 
- Some agencies had multiple participants, but no participant was from the same SW development unit.
- Most units conducted SW development and data science activities.
- Units often consumed more OSS than they published.
- More units were located outside the agency Chief Information Officer (CIO) office.

## Significance of the Study

This study is significant for developers, in and out of government, because it provides a concise history of OSS. It includes the federal government's early role with computing and more recent role with OSS publication. Further, it is significant for public administrators because it provides a glimpse of organizational factors they need to consider when implementing policy and technology. It also informs the Code.gov team of factors to consider for assisting agencies with implementing the FSCP.

## Coming Up

The next part of this series dives into the history of OSS including how the U.S. government played a significant role in the early days of computing. It discusses how OSS began as a normal part of computing, to be shunned by for-profit companies, and then to make a more recent comeback in all sectors.

## References

<a name='fn1'>1</a>: https://digital.gov/authors/joseph-castle/  
<a name='fn2'>2</a>: https://www.wsj.com/articles/SB10001424053111903480904576512250915629460  
<a name='fn3'>3</a>: https://go.govloop.com/open-source-myths  
<a name='fn4'>4</a>: https://www.itdashboard.gov/drupal/summary/000  
<a name='fn5'>5</a>: https://www.technologyreview.com/2002/07/01/40875/why-software-is-so-bad/  
<a name='fn5'>6</a>: https://www.technologyreview.com/2007/01/01/227178/anything-you-can-do-i-can-do-meta/