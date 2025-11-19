# Description

EA-13258: Fix CentOS 7 build by adding libssh2 compatibility patch

## Changes Made

- Added patch to guard ECDSA and ED25519 SSH key types not available in CentOS 7's libssh2-1.4.3
- Guarded SHA256 fingerprint verification block
- Guarded ECDSA/ED25519 variable declarations and case statements
- Bumped release to 8.17.0-2
- Fixed changelog date

## Testing

- ✅ CentOS 7 build succeeded in OBS (home:cory:EA4)

## Jira

https://jira.cpanel.net/browse/EA-13258
