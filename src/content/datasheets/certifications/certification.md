---
title: Certifications
layout: datasheet.hbs
columns: two
order: 60
---


## Overview

Connected devices nearly always require certifications that ensure they operate within the wireless transmission specifications determined by international regulatory bodies like the FCC and CE. This part of the guide will provide you with more information on how to leverage Particle's existing certifications to reduce the cost, complexity, and time associated with demonstrating regulatory compliance with your end product.

### Table of Contents
 - [FCC](#fcc) - United States
 - [IC](#ic) - Canada
 - [CE](#ce) - Europe
 - [TELEC](#telec) - Japan
 - [RoHS](#rohs) - Europe
 - [PTCRB](#ptcrb) - North America
 - [GCF](#gcf) - Europe
 - [UL](#ul) - World
 - [Battery Certifications](#battery-certifications) - World






## FCC<img class="inline-header-image" src="/assets/images/logo-fcc.png"/>
### Description
 - **Website**: [http://www.fcc.gov](http://www.fcc.gov)
 - **Wikipedia**: [https://en.wikipedia.org/wiki/FCC_Declaration_of_Conformity](https://en.wikipedia.org/wiki/FCC_Declaration_of_Conformity)
 - **Domain**: United States

The FCC (Federal Communications Commission) is an independent agency of the U.S. government that is in charge of regulating interstate and international communications. The FCC marking is required on electronic products manufactured or sold in the United States that certifies that the electromagnetic interference from the device is under limits approved by the FCC.

### Integration

The Photon as well as the PØ/P1 Modules are covered under certifications from the FCC. Certified radio modules comply with the "Intentional Radiator" portion (Part 15c) of FCC certification.

 - The **Photon** is certified as a single-modular transmitter that carries a modular grant. Modular certified radio modules are allowed for integration into multiple host end products by the FCC.

 - The **PØ Module**, which is on the Photon, does not itself have an antenna and thus does not have a discrete certification from the FCC. However, it is certified for integration into a host product under the RF reference of the Photon as a design guideline.

 - The **P1 Module** is also certified as a single-modular transmitter that carries a modular grant, and is certified for integration into multiple host end products by the FCC.

Any host product incorporating the Photon/PØ or P1 modules does not require additional testing or authorization for the Wi-Fi transmitter as long as:
- An antenna of the same type **and** equal or lesser gain to the antenna used for certification is used on the product.  
- Any restrictions found in the grants are followed in the OEM's end product integration of Particle hardware.

The Photon/PØ and P1 modules were certified with antennas of the following gain:
- **Photon/PØ Module**: Chip antenna (1.3dBi), external antenna (2.15dBi)
- **P1 Module**: On-board antenna (printed trace). Deployment with external antenna leveraging the onboard U.FL requires verification of certification.

### Customer Responsibilities
Even though we've certified the Photon and PØ/P1 Modules, as a product creator you're still responsible for meeting test requirements determined by the class of your product as described by the FCC. In general, there are two types of products--**Class A** and **Class B**:
- **Class A**: Digital device for use in commercial, industrial, or business environments.
- **Class B**: Digital device for use in residential environment not withstanding use in commercial, business, and industrial environments. Examples of such devices include, but are not limited to, personal computers, calculators, and similar electronic devices that are marketed for use by the general public.

Particle's certifications will help you decrease the time and cost associated with certification by allowing you to reuse our FCC ID as the FCC ID for your end product for Part 15c of your product's wireless certification. The remaining sections, for which all integrators and product creators are still responsible, are described below:


#### FCC Part 15 Certification
- **PART A: General Provisions and Definitions**  
  In this section, you will classify your device according to the definitions set out by the FCC. Included in this section are definitions for things like "intentional radiators", "kits", "test equipment", and "digital devices".

- **PART B: Unintentional Radiators**  
  This section covers devices whose purpose is not to produce radio waves, but which do anyway, including computers, voltage regulators, and oscillators/crystals.  It's likely that your end product contains unintentional radiators.  Part B allows for self-classication, which means that you don't have to get expensive test reports to demonstrate unintentional radiators in your product.

- **PART C: Intentional Radiators**  
  This section covers devices whose purpose is to produce coherent radio waves. The Photon/PØ/P1 modules are intentional radiators.  This is the most difficult part of FCC certification, and is where you can reuse Particle's hardware certifications to significantly simplify the application process. For instance, a from-scratch certification might cost $10-30K and take 4-8 weeks, while a verification of conformity might only cost $1-5K and take 2 weeks.

- **ADDITIONAL TESTING: Determined by device classification**  
  You'll also be responsible for any additional testing requirements defined by the FCC for your product. You can learn more about additional required testing for your product by visiting the FCC website, linked below.

**MORE INFO** -
[Electronic Code of Federal Regulation for Telecommunications, Part 15: Radio Frequencies Devices](http://www.ecfr.gov/cgi-bin/text-idx?c=ecfr&SID=a9f9d244cc20be8b56099003689d6cc3&rgn=div5&view=text&node=47:1.0.1.1.16&idno=47)

### Documentation

#### Photon/PØ - (updated 3/20/17)
- FCC ID: [2AEMI-PHOTON](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=o2hW1PEmrUZn19QwwX8hCA%3D%3D&fcc_id=2AEMI-PHOTON)
- [Certificate of Conformity](/assets/pdfs/new-certs/fcc/photon-fcc-certificate2017.pdf)
- [Test Reports](/assets/pdfs/new-certs/fcc/photon-test-reports.zip)
- [Test Firmware and Instructions](/assets/files/P0_P1_FCC_Firmware.zip)

#### P1 Module
- FCC ID: [COFWMNBM11](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=VG3YVqF5xjUgj%2BOio7CoOw%3D%3D&fcc_id=COFWMNBM11)  
- [Test Reports](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=VG3YVqF5xjUgj%2BOio7CoOw%3D%3D&fcc_id=COFWMNBM11)
- [Test Firmware and Instructions](/assets/files/P0_P1_FCC_Firmware.zip)

#### Electron U260 - (Updated 4/19/17)
- FCC ID: [XPYSARAU260](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=o2hW1PEmrUZn19QwwX8hCA%3D%3D&fcc_id=XPYSARAU260)
- [Certificate of Conformity - U260 v1.0](/assets/pdfs/electron/fcc-u260-certificate.pdf)
- [Test Reports - U260 v1.0](/assets/pdfs/electron/fcc-u260-test-report.pdf)
- [Certificate of Conformity - U260 v1.1](/assets/pdfs/new-certs/electron/FINAL_U260_FCC_DOC.pdf)
- [Test Reports - U260 v1.1](/assets/pdfs/new-certs/electron/FINAL_U260_FCC_REPORT.pdf)

#### Electron G350
- FCC ID: [XPYSARAG350](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=o2hW1PEmrUZn19QwwX8hCA%3D%3D&fcc_id=XPYSARAG350)
- [Certificate of Conformity - G350](/assets/pdfs/electron/fcc-g350-certificate.pdf)
- [Test Reports - G350](/assets/pdfs/electron/fcc-g350-test-report.pdf)

#### Electron E402 LTE (R410M)

FCC Part 15 Subpart B, Class B (sDoC):

- [Certificate of Conformity](/assets/pdfs/electron402-fcc-part15b.pdf)
- [Test report](/assets/pdfs/electron402-fcc-part15b-test-report.pdf)

#### E Series E310 (U201)
- FCC ID: [XPY1CGM5NNN](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=3vkdOEQAe%2Fc2YGK%2FBZsiJQ%3D%3D&fcc_id=XPY1CGM5NNN)
- [Certificate of Conformity](/assets/pdfs/electron/fcc-u201-certificate.pdf)
- [Test Reports - E310](/assets/pdfs/electron/fcc-u201-test-report.pdf)

#### E Series E402 LTE (R410M)

- FCC ID: [XPY2AGQN4NNN](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=ikrR3FBKrpgwIGJS1sm7Bw%3D%3D&fcc_id=XPY2AGQN4NNN)
- [Certificate of Conformity](/assets/pdfs/e402-fcc.pdf)

#### Argon

802.15.4 (mesh) certification:

- FCC ID: [2AEMI-ARGN](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=j56OXdnX7qhTRT%2BFJDABXg%3D%3D&fcc_id=2AEMI-ARGN)
- [Certificate of Conformity](/assets/pdfs/argon-mesh-wifi-fcc.pdf)
- [Test reports](/assets/pdfs/argon-mesh-fcc-test-report.pdf)

802.11b/g/n (Wi-Fi) certification:

- FCC ID: [2AEMI-ARGN](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=j56OXdnX7qhTRT%2BFJDABXg%3D%3D&fcc_id=2AEMI-ARGN)
- [Certificate of Conformity](/assets/pdfs/argon-mesh-wifi-fcc.pdf)
- [Test reports](/assets/pdfs/argon-wifi-fcc-test-report.pdf)

NFC certification:

- FCC ID: [2AEMI-ARGN](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=BIpTX7WKiovuCzJziwUi8Q%3D%3D&fcc_id=2AEMI-ARGN)
- [Certificate of Conformity](/assets/pdfs/argon-nfc-fcc.pdf)
- [Test reports](/assets/pdfs/argon-nfc-fcc-test-report.pdf)

FCC Part 15 Subpart B, Class B (sDoC):

- [Certificate of Conformity](/assets/pdfs/argon-fcc-part15b.pdf)
- [Test report](/assets/pdfs/argon-fcc-part15b-test-report.pdf)

#### Boron 2G/3G

802.15.4 (mesh) certification:

- FCC ID: [2AEMI-BRN310](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=ga4Ga888rpYrKWc2fmsMbQ%3D%3D&fcc_id=2AEMI-BRN310)
- [Certificate of Conformity](/assets/pdfs/boron310-mesh-fcc.pdf)

Cellular certification:

- FCC ID: [2AEMI-BRN310](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=jUA%2B92M3x8s6Anv9YourlA%3D%3D&fcc_id=2AEMI-BRN310)
- [Certificate of Conformity](/assets/pdfs/boron310-cellular-fcc.pdf)

NFC certification:

- FCC ID: [2AEMI-BRN310](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=QK7%2B3lEbzOBEQeHzO7QnYg%3D%3D&fcc_id=2AEMI-BRN310)
- [Certificate of Conformity](/assets/pdfs/boron310-nfc-fcc.pdf)

FCC Part 15 Subpart B, Class B (sDoC):

- [Certificate of Conformity](/assets/pdfs/boron310-fcc-part15b.pdf)
- [Test report](/assets/pdfs/boron310-fcc-part15b-test-report.pdf)

Additional FCC Test Reports:

- [FCC Part 22](/assets/pdfs/boron310-fcc-part22-test-report.pdf)
- [FCC Part 24](/assets/pdfs/boron310-fcc-part24-test-report.pdf)


#### Boron LTE 

802.15.4 (mesh) certification:

- FCC ID: [2AEMI-BRN402](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=86FVMi%2FyRce7yQ4d9ekA2g%3D%3D&fcc_id=2AEMI-BRN402)
- [Certificate of Conformity](/assets/pdfs/boron402-mesh-fcc.pdf)
- [Test reports](/assets/pdfs/boron402-mesh-fcc-test-report.pdf)

Cellular certification:

- FCC ID: [2AEMI-BRN402](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=86FVMi%2FyRce7yQ4d9ekA2g%3D%3D&fcc_id=2AEMI-BRN402)
- [Certificate of Conformity](/assets/pdfs/boron402-cellular-fcc.pdf)
- [Test report FCC part 22](/assets/pdfs/boron402-fcc-part22.pdf)
- [Test report FCC part 24](/assets/pdfs/boron402-fcc-part24.pdf)
- [Test report FCC part 27](/assets/pdfs/boron402-fcc-part27.pdf)

NFC certification:

- FCC ID: [2AEMI-BR402](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=p5QojqJWtSkeBRjIcM9gyA%3D%3D&fcc_id=2AEMI-BRN402)
- [Certificate of Conformity](/assets/pdfs/boron402-nfc-fcc.pdf)
- [Test reports](/assets/pdfs/boron402-nfc-fcc-test-report.pdf)

FCC Part 15 Subpart B, Class B (sDoC):

- [Certificate of Conformity](/assets/pdfs/boron402-fcc-part15b.pdf)
- [Test report](/assets/pdfs/boron402-fcc-part15b-test-report.pdf)


#### Xenon

802.15.4 (mesh) certification:

- FCC ID: [2AEMI-XENN](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=ugNeG69Gjl0KuJ%2Fo9IiqNg%3D%3D&fcc_id=2AEMI-XENN)
- [Certificate of Conformity](/assets/pdfs/xenon-mesh-fcc.pdf)
- [Test reports](/assets/pdfs/xenon-mesh-fcc-test-report.pdf)

NFC certification:

- FCC ID: [2AEMI-XENN](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=BsbBaeGLV6xp1u%2BNfGYUDw%3D%3D&fcc_id=2AEMI-XENN)
- [Certificate of Conformity](/assets/pdfs/xenon-nfc-fcc.pdf)
- [Test reports](/assets/pdfs/xenon-nfc-fcc-test-report.pdf)


## IC<img class="inline-header-image" src="/assets/images/logo-ic.png"/>

### Description
 - **Website**: [http://www.ic.gc.ca/Intro.html](http://www.ic.gc.ca/Intro.html)
 - **Wikipedia**: [http://en.wikipedia.org/wiki/Industry_Canada](http://en.wikipedia.org/wiki/Industry_Canada)
 - **Domain**: Canada

 IC (Industry Canada) is a department of the Government of Canada that, among many other things, issues Technical Acceptance Certificates (TACs) for Category I radio and broadcasting equipment.

### Integration

The Photon/PØ and P1 Modules are IC certified as single-modular transmitters. Just like with FCC Certification, any host product incorporating the Photon/PØ or P1 modules does not require additional testing or authorization for the Wi-Fi transmitter by IC as long as:
- An antenna of the same type **and** equal or lesser gain to the antenna used for certification is used on the product.  
- Any restrictions found in the grants are followed in the OEM's end product integration of Particle hardware.

### Customer Responsibilities

Industry Canada follows the same testing and rules as the FCC in regards to certified modules in authorized equipment.

### Documentation
For certificates of conformity, search [here](https://sms-sgs.ic.gc.ca/equipmentSearch/searchRadioEquipments?execution=e2s1&lang=en) using the IC ID for each Particle device, respectively.

#### Photon/PØ - (updated 3/20/17)
- IC ID: **20127-PHOTON**.
- [Certificate of Conformity](/assets/pdfs/new-certs/ic/photon-ic-certificate2017.pdf)
- [Test Report](/assets/pdfs/new-certs/ic/photon-test-reports.zip)

#### P1 Module
- IC ID: **10293A-WMNB11**.
- [Certificate of Conformity](/assets/pdfs/p1-ic-certificate.pdf)
- [Test Report](/assets/pdfs/p1-ic-test-report.pdf)

#### Electron U260 - (Updated 4/19/17)
- IC ID: **8595A-SARAU260**.
- [Test Report - U260 v1.0](/assets/pdfs/electron/ic-u260-test-report.pdf)
- [Test Report - U260 v1.1](/assets/pdfs/new-certs/electron/FINAL_U260_ICES_REPORT.pdf)

#### Electron G350
- IC ID: **8595A-SARAG350**.
- [Test Report](/assets/pdfs/electron/ic-g350-test-report.pdf)

#### Electron E402 LTE (R410M)

- [ICES-003 Issue 6:2016, Class B](/assets/pdfs/electron402-fcc-part15b.pdf)
- [ICES-003 Test report](/assets/pdfs/electron402-fcc-part15b-test-report.pdf)

#### E Series E310 (U201)
- IC ID: **8595A-1CGM5NNN**.
- [Certificate of Conformity](/assets/pdfs/electron/ic-u201-certificate.pdf)
- [Test Report](/assets/pdfs/electron/ic-u201-test-report.pdf)

#### E Series E402 LTE (R410M)
- IC ID: **8595A-2AGQN4NNN**.
- [Certificate of Conformity](/assets/pdfs/e402-ic.pdf)

#### Argon

- IC ID: **20127-ARGN**.
- [Certificate of Conformity](/assets/pdfs/argon-ic.pdf)
- [Test Report Mesh](/assets/pdfs/argon-mesh-ic-test-report.pdf)
- [Test Report Wi-Fi](/assets/pdfs/argon-wifi-ic-test-report.pdf)
- [Test Report NFC](/assets/pdfs/argon-nfc-ic-test-report.pdf)
- [ICES-003 Issue 6:2016, Class B](/assets/pdfs/argon-fcc-part15b.pdf)
- [ICES-003 Test report](/assets/pdfs/argon-fcc-part15b-test-report.pdf)

#### Xenon
- IC ID: **20127-XENN**.
- [Certificate of Conformity](/assets/pdfs/xenon-ic.pdf)
- [Test Report Mesh](/assets/pdfs/xenon-mesh-ic-test-report.pdf)
- [Test Report NFC](/assets/pdfs/xenon-nfc-ic-test-report.pdf)

#### Boron 2G/3G

- IC ID: **20127-BRN310**.
- [Certificate of Conformity](/assets/pdfs/boron310-ic.pdf)
- [Test Report Mesh](/assets/pdfs/boron310-mesh-ic-test-report.pdf)
- [Test Report NFC](/assets/pdfs/boron310-nfc-ic-test-report.pdf)
- [ICES-003 Issue 6:2016, Class B](/assets/pdfs/boron310-fcc-part15b.pdf)
- [ICES-003 Test report](/assets/pdfs/boron310-fcc-part15b-test-report.pdf)


#### Boron LTE

- [ICES-003 Issue 6:2016, Class B](/assets/pdfs/boron402-fcc-part15b.pdf)
- [ICES-003 Test report](/assets/pdfs/boron402-fcc-part15b-test-report.pdf)



## CE<img class="inline-header-image" src="/assets/images/logo-ce.png"/>

### Description
 - **Website**: [https://ec.europa.eu/growth/single-market/ce-marking/](https://ec.europa.eu/growth/single-market/ce-marking/)
 - **Wikipedia**: [http://en.wikipedia.org/wiki/CE_marking](http://en.wikipedia.org/wiki/CE_marking)
 - **Domain**: Europe

The CE mark is a mandatory conformity marking for certain products sold within the European Economic Area (EEA). It is analogous in that sense to the FCC marking used on devices sold within in the United States.

### Integration
Both the Photon/PØ and P1 are certified and carry the CE marking. Section 1.3.1 of the [Guide to the R&TTE Directive 1999/5/EC](http://ec.europa.eu/growth/sectors/electrical-engineering/rtte-directive/) states the following regarding the attachment of antennas to a module that already has documentation of conformance:

_"Manufacturers who place on the market products without an antenna or with an antenna that is intended to allow replacement have a responsibility to provide information on the general types and/or characteristics of antennas that may be used with their equipment in order that the overall radio equipment remains compliant. The guidance of the transmitter manufacturer has to be followed when they are installed."_

For the Photon/PØ and P1 Modules, these integration instructions are the same as for the FCC/IC--so long as you're integrating the modules without modifying the RF design or implementing an antenna with gain greater than that used in certification, your equipment will likely remain compliant.

The Photon/PØ and P1 Modules are certified with ETSI radio tests which can be accepted by a number of countries for radio compliance.

### Customer Responsibilities
If a product has adhered to the integration guidelines and has minimal risk, it can be self-certified where manufacturers complete a Declaration of Conformity and affix the CE marking to their own product.

#### Please note that Particle is not responsible in any way for issues arising from inappropriately self-certified products and devices using Particle hardware. EMC testing obligations may still be required as determined by the specific end product requirements.


- The end product will still need to be filed in each country for certification using the FCC/ETSI radio reports.
- 40+ countries recognize and accept radio test reports compliant to ETSI standards as part of the filing process, but note that some countries do not recognize modular approval.
- In most cases, it is possible to leverage Particle's ETSI reports, and thus testing does not need to be repeated.

### Documentation

#### Photon/PØ - (updated 8/6/17)
- [Certificate of Conformity](/assets/pdfs/new-certs/ce/photon-ce-certification-201708.pdf)
- [Test Reports](/assets/pdfs/new-certs/ce/photon-ce-test-reports-201708.zip)
- [RoHS 3.0 Test Report](/assets/pdfs/photon-rohs.pdf)

#### P1 Module - (updated 6/19/2018)
- [Declaration of Conformity](/assets/pdfs/new-certs/ce/p1-declaration.pdf)
- [Certificate of Conformity](/assets/pdfs/new-certs/ce/p1-ce-certification2017.pdf)

#### Electron U270
- [Certificate of Conformity](/assets/pdfs/electron/ce-u270-certificate.pdf)
- [Test Reports](/assets/pdfs/electron/ce-u270-test-reports.zip)

#### Electron G350
- [Certificate of Conformity](/assets/pdfs/electron/ce-g350-certificate.pdf)
- [Test Reports](/assets/pdfs/electron/ce-g350-test-reports.zip)

#### E Series E310 (U201)
- [Certificate of Conformity](/assets/pdfs/electron/ce-u201-certificate.pdf)
- [Test Reports](/assets/pdfs/electron/ce-u201-test-report.pdf)

#### Argon

- [Summary](/assets/pdfs/argon-ce-summary.pdf)
- [EMC Test Report](/assets/pdfs/argon-ce-emc-test-report.pdf)
- [RED Mesh Test Report](/assets/pdfs/argon-mesh-ce-test-report.pdf)
- [RED Wi-Fi Test Report](/assets/pdfs/argon-wifi-ce-test-report.pdf)
- [RED NFC Test Report](/assets/pdfs/argon-nfc-ce-test-report.pdf)
- [EN-60950 Test Report](/assets/pdfs/argon-EN60950-test-report.pdf)
- [EN-62311 Test Report](/assets/pdfs/argon-EN62311-test-report.pdf)
- [EN-62479 Test Report](/assets/pdfs/argon-EN62479-test-report.pdf)
- [RoHS 3.0 Test Report](/assets/pdfs/argon-rohs.pdf)

#### Boron 2G/3G

- [Summary](/assets/pdfs/boron310-ce-summary.pdf)
- [EMC Test Report](/assets/pdfs/boron310-ce-emc-test-report.pdf)
- [RED Mesh Test Report](/assets/pdfs/boron310-mesh-ce-test-report.pdf)
- [RED NFC Test Report](/assets/pdfs/boron310-nfc-ce-test-report.pdf)
- [RED Cellular Test Report](/assets/pdfs/boron310-cellular-ce-test-report.pdf)
- [EN-60950 Test Report](/assets/pdfs/boron310-EN60950-test-report.pdf)
- [EN-62311 Test Report](/assets/pdfs/boron310-EN62311-test-report.pdf)
- [EN-62479 Test Report](/assets/pdfs/boron310-EN62479-test-report.pdf)
- [RoHS 3.0 Test Report](/assets/pdfs/boron310-rohs.pdf)


#### Xenon

- [Summary](/assets/pdfs/xenon-ce-summary.pdf)
- [EMC Test Report](/assets/pdfs/xenon-ce-emc-test-report.pdf)
- [RED Mesh Test Report](/assets/pdfs/xenon-mesh-ce-test-report.pdf)
- [RED NFC Test Report](/assets/pdfs/xenon-nfc-ce-test-report.pdf)
- [EN-60950 Test Report](/assets/pdfs/xenon-EN60950-test-report.pdf)
- [EN-62311 Test Report](/assets/pdfs/xenon-EN62311-test-report.pdf)
- [EN-62479 Test Report](/assets/pdfs/xenon-EN62479-test-report.pdf)
- [RoHS 3.0 Test Report](/assets/pdfs/xenon-rohs.pdf)


## TELEC<img class="inline-header-image" src="/assets/images/logo-telec.png"/>

### Description
 - **Website**: [http://www.telec.co.jp/](http://www.telec.co.jp/)
 - **Documentation**: [http://www.tele.soumu.go.jp/e/index.htm](http://www.tele.soumu.go.jp/e/index.htm)
 - **Domain**: Japan

Particle has completed TELEC certification to achieve compliance with Japanese Radio Law. If you are seeking to distribute your product in Japan, please [contact Particle](mailto:will@particle.io) for more information about compiling TELEC-compliant firmware.

### Documentation

#### Photon/PØ
- [Certificate of Conformity](/assets/pdfs/p0-telec-certificate.pdf)
- [Test Report](/assets/pdfs/p0-telec-test-report.pdf)

#### Argon

- [JRL 38.24.1 Certificate of Conformity](/assets/pdfs/argon-jrl.pdf)
- [Test Report BLE](/assets/pdfs/argon-jrl-ble-test-report.pdf)
- [Test Report Wi-Fi](/assets/pdfs/argon-jrl-wifi-test-report.pdf)

#### Boron 2G/3G

- [JRL 38.24.1 Certificate of Conformity](/assets/pdfs/boron310-jrl.pdf)
- [Test Report](/assets/pdfs/boron310-jrl-ble-test-report.pdf)

#### Xenon

- [JRL 38.24.1 Certificate of Conformity](/assets/pdfs/xenon-jrl.pdf)
- [Test Report](/assets/pdfs/xenon-jrl-ble-test-report.pdf)


## RoHS<img class="inline-header-image" src="/assets/images/logo-rohs.png"/>

### Description
- **Website**: [http://ec.europa.eu/environment/waste/rohs_eee/index_en.htm](http://ec.europa.eu/environment/waste/rohs_eee/index_en.htm)
- **Wikipedia**: [https://en.wikipedia.org/wiki/Restriction_of_Hazardous_Substances_Directive](https://en.wikipedia.org/wiki/Restriction_of_Hazardous_Substances_Directive)
- **Domain**: Europe

RoHS stands for the "Restriction of Hazardous Substances Directive" adopted by the European Union in 2003 and effective as of 2006. It restricts the import and distribution of electronic and electrical equipment with six hazardous materials within the EU. Those hazardous materials are listed below:

| Substance Name  | Allowable Limit |
| ------------- | ------------- |
| Lead (Pb)  | less than 1000ppm  |
| Mercury (Hg)  | less than 100ppm |
| Cadmium (Cd) | less than 100ppm |
| Hexavalent chromium (Cr6+) | less than 1000ppm |
| Polybrominated biphenyls (PBB) | less than 1000ppm |
| Polybrominated diphenyl ether (PBDE) | less than 1000ppm |

There are also a short list of [exemptions](https://en.wikipedia.org/wiki/Restriction_of_Hazardous_Substances_Directive#Restriction_exemptions) to RoHS regulation that are worthy of note.

RoHS compliance is self-declared and there is no certification body that governs compliance, unlike the FCC. Particle has submitted its hardware to RoHS compliance testing and the test reports are available below.

### Documentation

#### Photon/PØ

- [RoHS 3.0 Test Reports](/assets/pdfs/photon-rohs.pdf)
- [Test Reports](/assets/pdfs/p0-rohs-test-reports.zip)

#### Electron U260/U270/G350

- [Test Reports](/assets/pdfs/new-certs/rohs/electron-rohs-test-reports.pdf)

#### Electron E402D (LTE)

- [Test Reports](/assets/pdfs/electron402-rohs.pdf)

#### E Series E310 (U201)

- [Test Reports](/assets/pdfs/electron/rohs-u201.pdf)

#### E Series E402 (SARA-R410M-02B)

- [RoHS 3.0 Test Reports](/assets/pdfs/e402-rohs.pdf)

#### Argon

- [RoHS 3.0 Test Reports](/assets/pdfs/argon-rohs.pdf)

#### Boron 2G/3G

- [RoHS 3.0 Test Reports](/assets/pdfs/boron310-rohs.pdf)

#### Boron LTE

- [RoHS 3.0 Test Reports](/assets/pdfs/boron402-rohs.pdf)

#### Xenon

- [RoHS 3.0 Test Reports](/assets/pdfs/xenon-rohs.pdf)


## UL<img class="inline-header-image" src="/assets/images/logo-ul.png"/>

### Description
<!-- remove for now because their website is broken, preventing pushing docs updates -->
<!-- - **Website**: [http://ul.com/](http://ul.com/) -->
 - **Wikipedia**: <a target="_blank" href="https://en.wikipedia.org/wiki/UL_(safety_organization)#UL_Standards">https://en.wikipedia.org/wiki/UL_(safety_organization)#UL_Standards</a>
 - **Domain**: Worldwide

UL (Underwriters Laboratories) is an American worldwide safety consulting and certification company. UL provides safety-related certification, validation, testing, inspection, auditing, advising, and training services to manufactures, retailers, policymakers, regulators, service companies, and consumers.

### Integration
The large majority of UL certifications, which can be found <a target="_blank" href="https://en.wikipedia.org/wiki/UL_(safety_organization)#UL_Standards">here</a>, are standards for electrical and electronic products that utilize high voltage AC electricity for power. UL certification is typically not required for low voltage or battery powered products.

### Customer Responsibilities
UL certification and safety standards are not applicable to Particle hardware, but may be applicable to the host end product in which they are integrated. It is the product creator's responsibility to ensure compliance with all UL safety standards and to obtain end product certification if required.

## PTCRB<img class="inline-header-image" src="/assets/images/logo-ptcrb.png"/>
### Description
- **Website**: [https://www.ptcrb.com/](https://www.ptcrb.com/)
- **Wikipedia**: [https://en.wikipedia.org/wiki/PTCRB](https://en.wikipedia.org/wiki/PTCRB)
- **Domain**: North America

The PTCRB is a certification body selected by North American cellular operators to create and manage a common cellular certification framework. PTCRB certification is a certification prerequisite for nearly all devices connecting to North American cellular networks.

### Certification variants

There are two common types of PTCRB certification – one that requires subsequent certifications after integration and one that does not. The Electron is certified with **"End Product"** certification, which does not require subsequent certification after integration, which decreases the certification burden on product creators building with the Particle platform.

**Module certification**
This is the PTCRB certification level for cellular modules. The PTCRB defines a module in the following way:

<p class = "boxed">
Modules are finished WWAN radio devices that do not directly connect to a host via a standardized external interface such as USB, PCMCIA, Compact Flash, MMC, RS-232, or IEEE-1394. A module may or may not include an integral antenna system or SIM/USIM interface.
<br>

Most cellular module vendors will seek PTCRB approval for their module in order to make subsequent End Product certifications simpler. Particle leverages the u-blox SARA-G350, SARA-U260, and SARA-U270 modules, all of which have module certifications from the PTCRB.

**End Product certification**
This is the PTCRB certification level for finished cellular products. End Products are defined as devices that meet all of the following attributes:

 - *Physical Interface* - If a physical control interface is required for the End Product, it shall utilize one of the following: USB, PCMCIA, Compact Flash, MMC, RS-232 (DE9), or IEEE-1394. No other physical control interfaces are acceptable.

 - *Power* - Obtains power from the standardized physical control interface or have a provisioned power source (i.e. dedicated battery, or a dedicated power source).
 - *UICC Interface* - Includes a fully self-contained USIM/SIM socket or embedded USIM/SIM
 - *Antenna* - Utilizes a self-contained antenna or provide an external antenna connector.
 - *Radio Access Technologies* - Covers at least one (1) comprehensive radio technology as specified by 3GPP for GERAN, UTRA, or E-UTRA devices

The Electron meets all of these specifications, and is thus certified by the PTCRB as an End Product.

### Customer Responsibilities

When an End Product like the Electron is connected to a host device (PC, PDA, etc.), no certification of the host device is required.  By its design and intended user application, an End Product must:

1. Be consistent with the terms of its FCC / Industry Canada type acceptance (e.g. type of antenna, distance from user, etc.).  In all cases, the End Product shall not alter its antenna system in any way from that allowed by the associated Type Acceptance or other regulatory approval.

2. Serve its final intended use without any further hardware and software modifications. If a control interface connection to a host is required for operation of the device, that connection can only be made through one of the above defined standardized physical interfaces.

### Documentation
#### Electron 3G (U260)
- [Certified Device Detail](https://www.ptcrb.com/certified-devices/device-details/?model=33577)

#### Electron 2G (G350)
- Product has completed and passed all PTCRB test requirements. Please [contact Particle](https://www.particle.io/sales) if you are building an end product with our 2G cellular solutions.

#### E Series E310 (U201)
- [Certified Device Detail](https://www.ptcrb.com/certified-devices/device-details/?model=39636)
- [Certificate of Conformity](/assets/pdfs/electron/ptcrb-u201-certificate.pdf)
- [Test Reports](/assets/pdfs/electron/ptcrb-u201-test-report.pdf)

#### E Series E402 LTE (R410M)
- [Certified Device Detail](https://www.ptcrb.com/certified-devices/device-details/?model=41338)
- [Certificate of Conformity](/assets/pdfs/e402-ptcrb.pdf)
- [AT&T LTE Certification](/assets/pdfs/e402-ota-att.pdf)

#### Boron LTE (R410M)

- [Certified Device Detail](https://www.ptcrb.com/certified-devices/device-details/?model=40983)

## GCF<img class="inline-header-image" src="/assets/images/logo-gcf.png"/>
### Description
- **Website**: [http://www.globalcertificationforum.org/](http://www.globalcertificationforum.org/)
- **Wikipedia**: [https://en.wikipedia.org/wiki/Global_Certification_Forum](https://en.wikipedia.org/wiki/Global_Certification_Forum)
- **Domain**: Europe

The GCF is a certification partnership between European network operators, mobile devices manufacturers, and certification/test labs. It serves a very similar function to the PTCRB for European operators.

### Documentation

#### Electron 3G (U270)
- Product has completed and passed all GCF test requirements. Please [contact Particle](https://www.particle.io/sales) if you are building an end product with our 3G-U270 cellular solutions.

## Carrier Certifications

#### AT&T (LTE Cat M1)

The Boron LTE (BRN402) and E Series LTE (E402) are certified for use on the AT&T LTE Cat M1 network. From the [AT&T Certified Devices page](https://iotdevices.att.com/certified-devices.aspx) search for "Particle".



## Battery Certifications

The 1,800mAh lithium-polymer (Li-Po) battery included with the Electron and other Particle accessories is compliant with all international safety and transportation standards.

**Model Number**: ZN-103450  
**Ratings**: 3.7V DC, 1,800mAh, 7.4Wh  
**Manufacturer**: ZHAONENG BATTERY INDUSTRIAL CO., LTD. (Shenzhen, China)  
**Test Reports**: 
- [IEC62133](/assets/pdfs/new-certs/battery/zn-103450-iec621331.pdf)
- [Material Safety Data Sheet, MSDS](/assets/pdfs/ZN-103450-MSDS.pdf)
