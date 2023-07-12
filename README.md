# EventTriggers_OSImageProvision
Event triggers that could initiate a new image build or update to a post-provisioning script. These triggers could be due to changes in the operating system (OS), security patches, core application updates, and even routine maintenance.

## Event Triggers:

1.	New OS version release:
    - Major version upgrade: For example, moving from Ubuntu 20.04 to Ubuntu 22.04.
    - Minor Build Version: For example, moving from Windows Server 2019 version 1809
2.	Critical Security OS Patches:
    - Patch released for an OS-level vulnerability: This could be an issue with the OS kernel, a critical system service, or an integral part of the OS.
3.	Critical Application Patches:
    - Patch released for a critical application-level vulnerability: An update for software like a web server (Apache), a database server (MySQL), or a programming language interpreter (Python).
4.	Patch Cycles:
    - "Patch Tuesday" On the second Tuesday of each month, Microsoft releases security patches and updates for its software products, including Windows Server. These patches typically address security vulnerabilities, add new features, and improve system performance.
    - Red Hat does not follow a specific monthly patch cycle like Microsoft. Instead, Red Hat releases patches as they become available. However, Red Hat does provide a "Planned Update Release Dates" schedule for minor releases of its products, which includes RHEL. Minor releases typically happen every six months and contain not just bug fixes and security patches, but also new hardware enablement and selected new features.
5.	Updates to core applications:
    - Major upgrade for a core application: For example, moving from MySQL 8.0 to MySQL 9.0.
    - Minor upgrade or patch for a core application: This could be an update to fix bugs or improve performance.
6.	Change in System Configurations:
    - Changes to network settings: This could include a change in DNS servers, changes in IP address management (from static to DHCP, for instance), or changes to network interfaces.
    - Updates to firewall rules: Adding or removing allowed ports or changing security protocols.
    - Changes in user roles and permissions: Adding a new user role, changing the permissions of an existing role, or removing a role.
7.	Security Agent / Standard:
    - New Security Agent Version: If a new version of your security agent software is released, it may include critical security enhancements or bug fixes.
    - Security Configuration Changes: If your security agent requires new configurations – such as new firewall rules, intrusion detection settings, or antivirus definitions – these changes could prompt a new build of your Golden Image.
    - Discovered Vulnerabilities: If your security agent detects a vulnerability in the system – such as an insecure system setting, a necessary patch that hasn't been applied, or an outdated software version – you should resolve these issues and update your Golden Image.
8.	Operational Agent / Standard:
    - Operational Agent Updates: If a new version of your operational agent software (like system monitoring or log collection tools) is released, you may need to update your Golden Image.
    - Operational Configuration Changes: If your monitoring agent requires new configurations – such as registry change and/or Service config change 
9.	Addition or Removal of Applications:
    - Adding Stand stack applications: This could be a new shell like PowerShell, Python, a new productivity app, etc.
    - Removing applications: Discontinuing the use of a tool or software that is no longer needed or has been replaced by a better solution. Like OS junkware and/role specific servers like Cups
10.	Routine Maintenance:
    - Updating system settings for optimization: Tweaking memory usage, improving I/O performance, or adjusting power settings.
11.	Post Incident Analysis:
    - Incident due to misconfigured service: This could be a security breach, a data loss, or a service outage caused by an incorrect configuration.
    - Incident due to outdated application: This could be a security incident or system instability caused by an newly discover software bug.
12.	Infrastructure Changes:
    - Migrating to a new cloud provider: Moving from AWS to Google Cloud, Azure to Oracle Cloud, etc.
    - Upgrading host hardware: This could involve updating drivers for new hardware or making changes to accommodate new hardware requirements.

___
Remember, the goal is not just to react to these triggers, but to develop a well-thought-out, systematic response that will ultimately improve our system's stability, performance, and security.

