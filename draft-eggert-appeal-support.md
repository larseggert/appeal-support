---
title: "Requiring Support for Appealing to the IESG and IAB"
abbrev: "Requiring Support for Appeals"
category: bcp
docname: draft-eggert-appeal-support-latest
submissiontype: IETF
v: 3
updates: 2026
area: GEN
# workgroup: PROCON Working Group
venue:
  group: PROCON
  mail: procon@ietf.org
  github: larseggert/appeal-support
  latest: https://larseggert.github.io/appeal-support/draft-eggert-appeal-support.html
author:
-
    name: Lars Eggert
    # role: editor
    org: Mozilla
    street: Stenbergintie 12 B
    city: Kauniainen
    code: "02700"
    country: FI
    email: lars@eggert.org
    uri: https://eggert.org/

normative:

informative:
  MontrealPlenary:
    title: "Minutes of the IETF66 Thursday Technical Plenary"
    target: https://www.ietf.org/proceedings/66/plenaryt.html
    date: 2019-7-13

--- abstract

RFC2026 describes the procedure for appealing decisions or process
failures to the IESG and the IAB. This document updates RFC2026 and
requires that an appellant must first gain support for their appeal
before an appeal may be considered by the body it is submitted to.

--- middle

# Introduction

{{Section 6.5 of !RFC2026}} outlines how conflicts in the IETF should
be resolved and describes how matters can be resolved by appealing
decisions at IESG and IAB level. The appeal mechanism has proven to
be an important mechanism for maintaining an open nature of the IETF
standards process.

It has been argued that appeals put an asymmetric workload on the
bodies that handle the appeal. It has also been argued that the
appeals process has been abused to stall forward progress
{{MontrealPlenary}}.

Therefore, this document updates {{!RFC2026}} in that an appellant
MUST gain support for entering the appeals process from at
least **three** active IETF participants ("supporters") for an appeal
to be considered. This requirement reduces the likelihood that the
appeals process will be abused by individuals while still maintaining
an open and accessible process for conflict resolution.

Below we describe how this requirement is integrated in the process
steps and what makes a supporter qualify.

# Conventions and Definitions

This document uses the term "supporter". This is a person with an
active IETF background (see {{qual}}). The supporter only supports
that the matter at hand should be reviewed by the responsible
board -- IESG or IAB. Their support for entering the appeals process
should in no way be seen as (non-)support for (the view of) the
appellant, but more for the fact that time of the responsible review
boards is to be spent on the issue.

{::boilerplate bcp14-tagged}

# Qualified Supporters {#qual}

Supporters are intended to have a reasonable IETF experience. They are
supposed to be active participants that know the IETF community.

Therefore, qualified supporters MUST be NomCom-eligible under the
criteria in{{Section 3 of !RFC9389}}, where "the day the call for
NomCom volunteers is sent" in this context is the day the appeal is
raised.

To keep the dispute resolution as open as possible, there are no
further requirements on supporters, i.e., {{Section 4.15
of !RFC8713}} does **not** apply to potential supporters. The group
of potential supporters hence may include members of the IESG, the
IAB, etc.

Qualified supporters MUST NOT have supported the same appellant during
a previous appeal within the past year. Qualified supporters MAY have
supported other appellants.

Appellants MAY act as a supporter for their own appeal when they meet
the above criteria. As a result they can only self-support once.

# Mechanics

Introducing the requirement for three supporters also introduces some
additional mechanics in the process. The two normative changes to the
process described in {{!RFC2026}} are that

- three supporters must have filed their support with the
  appeal-handling body at most two weeks after the appeal has been
  received by that body;

- the appeal-handling body MAY choose to not consider the appeal if
  there are insufficient qualified supporters.

Note that the appeal-handling body MAY choose to consider an appeal
even when there are insufficient qualified supporters.

It is the responsibility of the appellant to find qualified
supporters. In order to find qualified supporters, the appellant MAY
send a **single** message to **one** public IETF mailing list.

Supporters SHOULD send their supporting messages personally to the
appeal-handling body in question and SHOULD NOT proxy their message
through the appellant.

If an appellant escalates an appeal from the IESG to the IAB, that
escalated appeal MUST find new qualified supporters.

# Conclusions

The mechanism proposed herein only applies to appeals to the IESG and
the IAB. It does not apply to other forms of dispute resolution.

# Security Considerations

This document specifies neither a protocol nor an operational
practice, and as such, it creates no new security considerations.

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

This is a re-spin of {{?I-D.kolkman-appeal-support}}. Thanks to Olaf
Kolkmann for having the right idea nineteen years ago and writing it
down.
