# !!! SM/Root Handoff Guide !!!

## These steps must be followed when on-boarding/off-boarding rootstaff or SMs, or I will be disappointed in you.


### On-boarding/off-boarding rootstaff

The following privileges/accounts must be granted when someone is made root, **and taken away/disabled when they are no longer root**.

* /root and /admin Kerberos principals
* Membership of the ocfroot LDAP group
	- `kinit you/admin`
	- `ldapvi cn=ocfroot`
* Kerberos permissions in the ACL list
	- `add otherstaffer/admin`
	- `add otherstaffer/root`
* 24/7 Keycard Access, and their name on the Emergency after hours list
* Membership of the root@ Google group to receive technical spam
* Membership of the workspace-admins@ Google group to enforce physical security token 2fa
* Super Admin status in Google Workspace
* "Root" role in the OCF Discord
* Owner status in the OCF Github
* A 1password account, membership of the "Owners" group, and access to the root (and really-root?) vaults
* Their hardware token ssh key added to agenix in the ocf/nix repo
* Their ssh key added to nix deploy users
* Membership of the security contact in socreg
* Panorama access (perhaps this should be SM only?)
* //TODO anything I missed? 


### SM Handoff

The following steps must be taken every time there is a new Site Manager, to ensure proper transfer of accounts.

* All of the above steps if one SM is gaining or losing root.
* The following should always be held by one of the current SMs, and such should be transferred to an incoming SM if the person who holds it is leaving:
  * Ownership of the OCF Discord
  * //TODO i probably forgot a lot of things
  * Any account that requires a single user to be the owner
* Additionally, the incoming/outgoing SMs should perform an audit of this list, and ensure that any new/removed manually assigned privileges are reflected here.

meow
meow (with Brazilian characteristics)
