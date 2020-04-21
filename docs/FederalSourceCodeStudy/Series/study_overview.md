# Study Overview
By Joseph Castle, PhD, Code.gov <sup>[1](#fn1)</sup>

*This write-up elaborates on portions of the [Federal Source Code Study (FSCS)](https://github.com/GSA/code-gov/blob/master/docs/FederalSourceCodeStudy/FederalSourceCodeStudy.pdf), a three-year study conducted from 2017 to 2020 by the Code.gov team to better understand agency implementation of the Federal Source Code Policy (FSCP). The study considered open source software (OSS) publication as one indicator of FSCP implementation and examined why some agencies publish OSS and others do not.*

Series ToC<sup>*</sup>:
- [History of OSS](#history_of_OSS.md)
- [Federal Government's Intersection with OSS](#)
- [Cultural Beliefs](#)
- [Public Engagement](#)
- [Structural Dimensions](#)
- [Organizational Location](#)
- [Analysis of Organizational Factors & OSS Publishing](#)
- [Implications & Recommendations for Public Administrators](#)

<sup>*</sup>Sections will be added as soon as they are created.

---

## Towards a Federal Source Code Policy (FSCP)

> Computer software (SW) is essential for the daily operations of industry and government. “More and more major businesses and industries are being run on software – from movies to agriculture to national defense”. <sup>[2](#fn2)</sup>

The federal government spends approximately six billion dollars on SW each year <sup>[3](#fn3)</sup>, representing 7% of the [information technology (IT) budget](https://itdashboard.gov/) of the [Chief Financial Officers (CFO) Act agencies](https://en.wikipedia.org/wiki/Chief_Financial_Officers_Act). <sup>[4](#fn4)</sup>

This purchasing of SW frequently results in duplicative and wasteful spending annually because the SW is not publicly shared. Agencies purchase SW and customize as needed, often leading to SW purchasing and support that is costly, allows for little to no reuse, results in duplication of effort and spending across agencies, and overall yields poor quality. <sup>[5](#fn5), </sup><sup>[6](#fn6)</sup>

In 2016, as a response to inefficiencies with software purchasing and reuse, the White House issued the [Federal Source Code Policy: Achieving Efficiency, Transparency, and Innovation through Reusable and Open Source Software](https://sourcecode.cio.gov/) or the FSCP. 

The FSCP directed CFO Act agencies to do three things: 
1. Create an agency source code policy; 
2. Update acquisition language to capture new custom code; and, 
3. Create a source code inventory and publish at least 20% as open source software (OSS). 

The FSCP also established the Code.gov program and technical platform of a [website](https://code.gov/) and [application programming interface (API)](https://open.gsa.gov/api/codedotgov/).

## Organizational Factors Affecting OSS Publication

As an initial first step to understanding FSCP implementation and OSS publication, we used the [GitHub API](https://developer.github.com/v3/) to gather metadata pertaining to agency public coding activities. This metadata showed agencies were publishing OSS with mixed results before and after publication of the FSCP. The Code.gov team wondered why some agencies could publish OSS and other agencies could not. Conceivably, every agency has the following characteristics to support OSS publication.

- An inherent mandate to serve the public by being transparent and release public funded products (as appropriate with consideration to security, privacy, etc.).
- Requirements dictated by the FSCP enforcing compliance to publish OSS.
- An IT budget with a portion devoted to SW development.
- IT specialists and contractors with technical skills who regularly work with SW.

Arguably with similar agency capabilities for publishing OSS, not all were doing so. This led us to the premise of the study focusing on potential organizational factors related to organizational cultural beliefs, public engagement, structural dimension, and organization location influencing agency OSS publication.

## Study Description

The qualitative study included a metadata analysis, interviews, and artifact collection (e.g., SOPs, organization charts). The sample contained the following attributes.

- 20 of 24 CFO Act agencies were represented.
- 25 participants were from unique SW development units. There were multiple participants from some agencies, but no participant from the same SW development unit.
- Unit functions mostly included SW development and data science.
- Units often consumed more OSS than they published.
- More units were located outside the agency Chief Information Officer (CIO) office. (Note: The CIO is the the primary audience of the FSCP but more SW development was happening outside the CIO office.)

## Significance of the Study

This study is significant for developers, in and out of government, because it provides a concise history of OSS and the federal government's early role with computing and more recent role with OSS publication. Further, it is significant for public administrators because it provides a glimpse of organizational factors they need to consider when implementing policy and technology.

## Coming Up

The next part of this series dives into the history of OSS including how the U.S. government played a significant role in the early days of computing. It discusses how OSS began as a normal part of computing, to be shunned by for-profit companies, and then to make a more recent comeback in all sectors.

## References

<a name='fn1'>1</a>: https://digital.gov/authors/joseph-castle/  
<a name='fn2'>2</a>: https://www.wsj.com/articles/SB10001424053111903480904576512250915629460  
<a name='fn3'>3</a>: https://go.govloop.com/open-source-myths  
<a name='fn4'>4</a>: https://www.itdashboard.gov/drupal/summary/000  
<a name='fn5'>5</a>: https://www.technologyreview.com/2002/07/01/40875/why-software-is-so-bad/  
<a name='fn5'>6</a>: https://www.technologyreview.com/2007/01/01/227178/anything-you-can-do-i-can-do-meta/