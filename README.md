Openshift Enterprise BPMS Execution Server Cartridge
====================================================

OVERVIEW
--------
  - Provides the BPMS process engine on OpenShift exposed via REST API.


PURPOSE
-------
  - a BPMS6 Execution Server cartridge is important because it allows for easy provisioning in a public and/or on-premise OpenShift cloud environment
    of the most important component of a BPM solution:  the process engine
  - in a production environment, this cartridge enables horizontal elasticity of a BPM execution server 'tier'
  - in a development environment, this cartridge enables easy provisioning of the same BPM execution server in a small, 'free-tier', cloud environment


FEATURES
--------
  - BPMS6 process engine exposed via the REST API provided by the droolsjbpm kie-services-remote project
  - process instance and human task persistence via a pre-configured 'jbpm' mysql database
  - droolsjbpm libraries deployed as EAP6 modules allowing for reduced runtime footprint
  - configurable knowledge session strategies:  PER_PROCESS_INSTANCE or SINGLETON
  - asynchronous (via embedded hornetq) BAM process event listener
  - audit log persistence provided by a pre-configured 'jbpm_bam' postgresql-8.4 database
  - jbpm runtime has been slimmed down to fit comfortably in an Openshift small gear
  - will inter-operate with other cartridges from the Openshift bpmPaaS  suite:
    - business-central cartridge
    - dashboard cartridge
    - bam cartridge

