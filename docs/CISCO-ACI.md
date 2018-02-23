This module will allow you to provision the ACI objects that are most commonly used or deployed in immutable application architectures.
- [Tenant](https://www.cisco.com/c/en/us/td/docs/switches/datacenter/aci/apic/sw/1-x/Operating_ACI/guide/b_Cisco_Operating_ACI/b_Cisco_Operating_ACI_chapter_0111.html) A high level object that separates one set of resources from another between two separate business groups or clients.
- [Application Profile Group](https://www.cisco.com/c/en/us/td/docs/switches/datacenter/aci/apic/sw/1-x/Operating_ACI/guide/b_Cisco_Operating_ACI/b_Cisco_Operating_ACI_chapter_0111.html#concept_F4947E22AD2143749DAC34E69F80706F) An object with the purpose of containing one or more EPGs in a logical grouping.
- [EPG](https://www.cisco.com/c/en/us/td/docs/switches/datacenter/aci/apic/sw/1-x/Operating_ACI/guide/b_Cisco_Operating_ACI/b_Cisco_Operating_ACI_chapter_0111.html#concept_81AC0F90789B454F80E796A7029EFD1E) An object that provides a contract to be consumed by another EPG. Conceptually similar to Kuberenetes service.
- [Contacts, Subjects, and Filters](https://www.cisco.com/c/en/us/td/docs/switches/datacenter/aci/apic/sw/1-x/Operating_ACI/guide/b_Cisco_Operating_ACI/b_Cisco_Operating_ACI_chapter_01000.html) Contracts are provided by one EPG and consumed by another, and contain multiple subjects, which themselves may contain multiple filters. Filters how ever are not a child object of the contract as they may belong to other contracts, and as such remain their own top level object and are consumed by contracts via a many-to-many relationship with subjects.

![ACI Models](aci-models.png)

[More info on Cisco ACI](https://www.cisco.com/c/en/us/solutions/data-center-virtualization/application-centric-infrastructure/index.html)