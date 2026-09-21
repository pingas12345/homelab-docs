# Lessons Learned

Practical takeaways from building and maintaining this environment.

## What Worked Well

- Using Portainer as a central management plane significantly reduced operational friction.
- Keeping the majority of application workloads in Docker improved consistency and rollback capability.
- WireGuard + Dynamic DNS provided reliable and secure remote access without exposing services directly.
- Storing media on a NAS in JBOD configuration made capacity expansion straightforward.
- Logical grouping of services (Media, Automation, Management) made documentation and maintenance easier.

## Areas for Improvement

- More rigorous backup testing and documented recovery procedures.
- Upgrade NAS, upgrade drives and implement RAID
- Stronger infrastructure-as-code practices (more complete Compose files under version control).
- Improved monitoring and proactive alerting.
- Better documentation of native (non-container) services on the host.
- Implement wiki for internal knowledge management and for family reference.

## General Observations

- Clear documentation is as valuable as the services themselves.
- Starting simple and iterating is more effective than trying to build a perfect stack on day one.
