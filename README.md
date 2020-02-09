# ansible_guide_examples
Ansible with Isilon

Purpose:

Detail the configuration required to enable Dell EMC Isilon interoperability with Ansible core and AWX.  AWX is the upstream project from which the Red Hat Ansible Tower offering is derived. Isilon is the industry benchmark for scale-out file and is widely recognized as a leader by Gartner and IDC. 
The document will explore using the native Ansible modules to access and drive Isilon functionality. I will demonstrate how to access and use the Isilon RESTful Application Programable Interface (API) with curl, the Ansible “URI” module and the traditional Ansible Command Line Interface (CLI) module.
I will highlight the typical challenges that I encountered using the Isilon API and other variable substitution issues in YAML files used with ansible play books.
I describe the core configuration and troubleshooting of the environment as it relates to the overall purpose of this document. Please note, this document is not intended to be an Ansible best practice or detailed how-to guide.
Ultimately the information provided is focused on enabling system engineers and developers alike to include Isilon in their devOps and infrastructure as code journey.

Context:

Ansible is one of several devOps tools gaining widespread popularity within the I.T. industry.
I am a Senior Systems Engineer at Dell EMC and many of my clients (past and present) use Ansible for configuration management, application, cloud, and storage deployments. This guide has been specifically written to empower Dell EMC Isilon clients that have already invested in Ansible.
The examples within this document will be kept simple as the key focus is on interoperability, and enablement; 

Intended audience:

The document has been written for System administrators, DevOps engineers, developers that wish to incorporate Isilon into their Ansible environment. Concepts and terminology used within this document will be of a technical nature. I will provide links to the relevant how-to documentation to ensure you have all the required knowledge to get started with Isilon and/or duplicate this lab for your own learning.

