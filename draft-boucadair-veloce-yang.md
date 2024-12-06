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
 - next generation
 - unicorn
 - sparkling distributed ledger

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

Guidance for writing  YANG modules are discussed in {{!I-D.ietf-netmod-rfc8407bis}}. All these guidelines apply expect those related to narrative text.

# Conventions and Definitions

{::boilerplate bcp14-tagged}

# VELOCE Procedure

The following procedure is followed when a WG adopts (a document with) a YANG module:

* A new repository MUST be created by the WG Chairs following the procedure in {{Section 3.2 of !RFC8874}}.
* Contributing methods are those defined in {{Section 4 of !RFC8874}}.
* The WG Chairs MUST seek in a timely manner after the adoption of the document for the publication of an RFC that describes the initial module objectives and, more importantly, registers the URI in the "ns" subregistry within the "IETF XML Registry" {{?RFC3688}} and the YANG module in the "YANG Module Names" subregistry {{?RFC6020}} within the "YANG Parameters" registry.
* The YANG module MUST NOT be inserted in the document; instead a link to the Github repository MUST be included.

# Security Considerations

The same considerations discussed in {{Section 10 of !RFC8874}} apply here.

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

This draft is triggered by the discussion in NEMOPS IAB workshop.
