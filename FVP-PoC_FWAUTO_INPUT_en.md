# FWAuto Input Document: OpenBMC FVP-PoC

## Objective

Automate the build and verification of the Arm OpenBMC FVP-PoC project on a remote Linux host.

## Remote Host

| Item | Value |
|------|-------|
| Host | - |
| User | - |
| Password | - |
| OS | Ubuntu 22.04 (x86_64) |

## Reference Materials

**Please read the README.md from the following GitLab Repo to understand the build and execution process:**

- **GitLab Repo**: https://gitlab.arm.com/server_management/PoCs/fvp-poc
  - Read README.md to understand:
    - build.sh usage (setup, build bmcfvp)
    - run.sh usage
    - Required FVP simulators
    - Verification methods (SSH, Redfish, PLDM)

- **FVP Download** (requires Arm account, manual download):
  - Host FVP: https://developer.arm.com/Tools%20and%20Software/Fixed%20Virtual%20Platforms/Infrastructure%20FVPs#v3-r1
  - BMC FVP: https://developer.arm.com/Tools%20and%20Software/Fixed%20Virtual%20Platforms/Arm%20Architecture%20FVPs

## Verification Criteria

- SSH to BMC (port 4222, password 0penBmc) successful
- Redfish API responds normally
- PLDM commands execute successfully
