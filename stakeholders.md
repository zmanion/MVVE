# Stakeholders

## Stakeholder Roles and Glossary

Defining stakeholders and a few specific terms. These roles are not exclusive, a stakeholder can hold multiple roles.

### Defender

Primary audience of this work.

direct: end user, system administrator

indirect: vulnerability management product or service, acting on behalf of direct defenders

A note about offense, red team activity is clearly a "know your enemy" type of defense. Actual offense for the purpose of offense is not our focus here, although the fundamentals of our work should still apply, that is, offense needs to manage vulnerabilities also.

### Supplier

Borrowing from thoroughly debated CVE and SBOM definitions: the vendor, developer, maintainer, steward, producer, provider, supplier, manufacturer of the product.

Suppliers are often also defenders, in that they likely care about reducing risk to their users and are often users themselves of upstream products.

Borrowing another term from CVE: A product is a generic unit of software, component, device, project, service, system. Can include hardware, but very rarely does a vulnerability exist in cold, unpowered hardware (CPU timing vulnerabilities being an exception, and those are mitigated by software involving microcode and kernel parameters).

### Consumer and Producer

The producer and consumer of vulnerability information, not of products.

### Researcher

Security researcher, bug hunter, finder, reporter. Some researchers are CNAs. Typically also indirect defenders. Researchers are often producers of vulnerability information.
