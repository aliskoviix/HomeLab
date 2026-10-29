# Homelab: Windows Server Active Directory Lab

A virtualised small-company network built in Hyper-V on Windows 11 Pro, used to practise IT support and Windows administration.

**Status:** In progress

## Lab design

| Machine  | Role                                                              | IP                      |
|----------|-------------------------------------------------------------------|-------------------------|
| DC01     | Windows Server 2022 domain controller: AD DS, DNS, DHCP, file shares | 10.10.10.10 (static)    |
| CLIENT01 | Windows 11 Enterprise workstation joined to the domain            | DHCP (10.10.10.100–200) |

The lab runs on an isolated Hyper-V internal switch with NAT (10.10.10.0/24). It has internet access but cannot reach my home network.

## Progress

- [x] Hyper-V host and isolated NAT network
- [ ] Domain controller with AD DS and DNS
- [ ] DHCP server
- [ ] Windows 11 client joined to the domain
- [ ] OU structure and security groups
- [ ] PowerShell: bulk user creation from CSV
- [ ] Department file shares with NTFS permissions
- [ ] Group Policy: drive maps, password and lockout policy, user restrictions
- [ ] Helpdesk account with delegated permissions (least privilege)
- [ ] Troubleshooting tickets documented

## Tech used

Hyper-V · Windows Server 2022 · Active Directory · DNS · DHCP · Group Policy · PowerShell

## Repository layout

- `scripts/` – PowerShell scripts
- `tickets/` – troubleshooting write-ups
- `screenshots/` – evidence of each step
