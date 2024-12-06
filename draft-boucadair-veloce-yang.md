---
title: "YANG deVELpment PrOCEss & maintenance (VELOCE)"
abbrev: "VELOCE"
category: info

docname: draft-boucadair-veloce-yang-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
# area: OPS
# workgroup: VELOCE
keyword:
 - quick but well YANG modules

author:
 -
    fullname: Mohamed Boucadair
    organization: Orange
    email: mohamed.boucadair@orange.com

normative:

informative:


--- abstract

This document describes a YANG deVELpment PrOCEss & maintenance (VELOCE) that is more suitable for the development of YANG modules within the IETF.

--- middle

# Introduction

RFCs are not be suited for documenting YANG modules. However, implementers/vendors are looking for reference models and sufficiently stable models to refer to. To that aim, this document proposes a new approach for documenting IETF-endorsed YANG modules.

Guidance for writing YANG modules are discussed in {{!I-D.ietf-netmod-rfc8407bis}}. Guidelines related to code components ({{Section 3.2 of !I-D.ietf-netmod-rfc8407bis}}) or citations to references listed in the YANG module do not apply for VELOCE.

This document mainly focuses on IETF modules. Note that {{I-D.ietf-netmod-rfc8407bis}} includes provisons for IANA-maintained modules to not be included in RFCs:

{: quote}
>    Designers of IANA-maintained modules MAY supply the full initial
   version of the module in a specification document that registers the
   module or only a script to be used (including by IANA) for generating
   the module (e.g., an XSLT stylesheet as in Appendix A of [RFC9108]).

# Conventions and Definitions

{::boilerplate bcp14-tagged}

# VELOCE Procedure

The following procedure is followed when a WG adopts a YANG module:

* A new repository MUST be created by the WG Chairs following the procedure in {{Section 3.2 of !RFC8874}} to maintain the YANG Module, with the apprpriate CI/CD YANG validation in place. Other administrative polices are defined in {{!RFC8875}}. The same procedure for managing WG documents (e.g., assign editors) applies for managing YANG modules ({{Section 6.1 of !RFC2418}}). Refer also to {{Section 3.3 of !RFC8874}} for considerations related to granting WG participants write and administrators right.
* Contributing methods to YANG module (including issues handling andd merge procedure) are similar to those defined in {{Section 4 of !RFC8874}}.
* The WG Chairs MUST seek in a timely manner after the adoption of the document for the publication of an RFC that describes the initial module objectives and, more importantly, registers the URI in the "ns" subregistry within the "IETF XML Registry" {{?RFC3688}} and the YANG module in the "YANG Module Names" subregistry {{?RFC6020}} within the "YANG Parameters" registry.
* The YANG module MUST NOT be inserted in the document; instead a link to the Github repository MUST be included.
* Bis versions of the initial RFC MAY be considered to document major changes or their rationale. Such a decision is left to the WG Chairs.

# Security Considerations

The same considerations discussed in {{Section 10 of !RFC8874}} apply here.

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

This draft is triggered by the discussion in NEMOPS IAB workshop.
