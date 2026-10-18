# Day 4 – Basic Device Security

## Objective
Configure basic security settings on Cisco routers and switches using Cisco IOS CLI.

## Tasks Completed
- Changed the device hostname to R1.
- Configured an enable password (`CCNA`).
- Tested privileged EXEC mode password authentication.
- Enabled password encryption using `service password-encryption`.
- Configured a more secure enable secret (`Cisco`).
- Verified password encryption in the running configuration.
- Saved the configuration to startup-config.

## Commands Used

**Global Configuration Mode**
```
enable
configure terminal
hostname R1
enable password CCNA
service password-encryption
enable secret Cisco
```

**Verification and Saving**
```
end
show running-config
write memory
```

## What I Learned
- `enable password` sets a password for privileged EXEC mode.
- `service password-encryption` encrypts passwords using Cisco Type 7, which is weak and reversible.
- `enable secret` provides stronger password protection and takes priority over `enable password`.
- `show running-config` displays the active device configuration.
- `write memory` saves the running configuration so it persists after a reboot.
- Cisco IOS commands must be entered in the correct configuration mode.

## Lab Evidence
Screenshots showing the password configuration, encryption, running configuration, and successful save.
