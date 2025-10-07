# Information Elements

## Summary


## Elements

Information elements, not necessarily data elements (fields, colummns).  information elements can be conveyed explicitly, implicitly, by inference, by default assumeption.

non-explicitness of any element must be defined

If presence of information is an assertion, non-presence of that information must be defined/clarified.  Non-presence means nothing unless defined.

For a CVE example, the presence of the [unsupported-when-assigned](https://www.cve.org/ResourcesSupport/Glossary#glossaryTags) tag means that

> At the time of CVE ID assignment, all known Products affected by the CVE ID no longer receive security Fixes. Typically, the Products are no longer supported and are considered to be End of Life (EOL).

The lack of the tag means essentially nothing, which may be confusing, the consumer cannot safely interpret this to mean that affected products are EOL or not.

A consumer could interpret lack of this tag to mean either that the affected products are supported or that the EOL status of the affected products is unknown.  In this case, the EOL status information is not being successfully conveyed.




### Vulnerability Identifier

Required by MVVE.

A unique identifier that unambiguously identifies and refers to the vulnerability.

In a philosophical or epistemological sense, a vulnerability exists, and is referred to by identifiers (including names). The vulnerability is the referent.
Identifiers should be unique, succinct, consistent, and preferably easy to match with a regular expression.
The referent must be a unique and atomic vulnerability, “Atomic” meaning it is identified at its lowest common source – If a product includes an open source library that has a vulnerability, the atomic referent is the flaw in the open source library - within that library it would exist in one component/function. the component in the product is then associated and connected to that referent.

To date, we’re getting by mostly with identifiers that are short enough to be memorable by humans and long enough to address at least the lower bound of enumerated and publicly disclosed vulnerabilities. A catchy name (Log4Shell, Heartbleed) is an identifier that usually includes descriptive aspects and is better recognized and remembered by humans, at least on a relatively small scale and for important or widely publicized vulnerabilities. Humans may prefer less descriptive, more arbitrary names (Arbitrary Albatross) over numeric identifiers (CVE-1900-1234, GHSA-f3mf-hm6v-jfhh), or not. The CVE Program identified more than 40,000 vulnerabilities in 2024, so we’re going to need systemic identifiers and cannot rely on catchy names. At the far end of the human-computer identifier spectrum, UUIDs are well beyond practical, wide-scale recall of short-term human memory.

In the authors’ opinion, it is convenient if the unique identifier is easily discovered in logs or documents with a regular expression, and is not difficult to type or transfer from one medium to another and it shouldn’t be impossible to commit to memory (looking at you UUIDs).

### Product Identifier

Required by MVVE.

“The naming problem”

The thing that has status, can be hardware if it’s really hardware and not firmware or microcode, but it’s really nearly all software
We are neutral on which ID scheme in that we don’t have a favorite or preference, but perhaps more importantly, product ID schemes are lacking today, maybe cite MITRE paper. This is its own huge problem, bigger than MVVE.

"Product" is defined broadly and generically to include commercial, proprietary, free, open source, and any other types of software ad hardware (that runs software).

### Status

Required by MVVE.

status must be resolvable for every listed product

To exist at all, a vulnerability must affect at least one product, this is status.  May be inferred?  A dangerous assumption, be explicit?

vulnerability status product



###
