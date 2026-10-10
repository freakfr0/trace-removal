# Trace Removal & Security Audit Tools

> **Repository description:** Read-only Bash utilities for authorized server log auditing, incident response, Linux system administration, and digital-forensics review.

[![Platform](https://img.shields.io/badge/platform-Linux-blue)](https://www.kernel.org/)
[![Shell](https://img.shields.io/badge/shell-Bash-4EAA25)](https://www.gnu.org/software/bash/)
[![Focus](https://img.shields.io/badge/focus-defensive%20security-blueviolet)](#responsible-use)

A collection of shell utilities for **authorized server administration, incident response, and digital-forensics review**. These scripts inventory common log locations and report log-directory usage without changing the host.

> [!IMPORTANT]
> **Safe, read-only operation:** The shell scripts currently provided here are audit-only. They do not erase logs, alter timestamps, conceal processes, disable security controls, or remove system files. Preserve original evidence and follow your organization's incident-response and retention policies.

## Features

- Inspect common Linux log directories when present and readable.
- Report disk usage for `/var/log`, `/var/log/audit`, and `/var/log/journal`.
- List recent log-file metadata (timestamp, size, and path) without printing log contents.
- Support initial triage and non-destructive system review.
- Keep scripts organized by their project-specific folder names.

## Repository layout

The shell scripts are kept in their named project directories under `trace_removal/`.

| Directory | Script |
|---|---|
| `Advanced_Artifact_Cleanup_Script/` | `cleanup_script.sh` |
| `Advanced_Cleanup_Script/` | `cleanup_script.sh` |
| `Advanced_Footprint_Cleaning_Script/` | `cleanup_script.sh` |
| `Advanced_Footprint_Cleanup_Script/` | `cleanup_script.sh` |
| `Advanced_Security_Operations_Script/` | `advanced_security_operations.sh` |
| `Advanced_Trace_Cleaning_Script/` | `clean_traces.sh` |
| `Advanced_Trace_Removal_Script/` | `cleanup.sh` |
| `Advanced_Trace_Removal_Script_v2/` | `remove_traces.sh` |
| `clear_logs_and_hide_activities/` | `clear_logs_and_hide_activities.sh` |
| `trace_removal/` | `trace_removal.sh` |

## Requirements

- Linux
- Bash
- Standard command-line utilities: `date`, `find`, `sort`, `head`, and `du`
- Read permission for the log paths you want to inspect

## Usage

Run a script from the repository root. Example:

```bash
bash trace_removal/Advanced_Security_Operations_Script/advanced_security_operations.sh
```

Scripts inspect standard system log paths. Restricted permissions or missing directories may limit the report. Run scripts only on systems you own or are explicitly authorized to administer.

## Responsible use

- Use only on systems you own or are explicitly authorized to assess.
- Preserve logs and metadata during investigations; work from copies when possible.
- Never use cleanup procedures to conceal unauthorized activity or destroy forensic evidence.
- Review scripts before execution and test changes in a disposable environment first.

## License

No license is specified yet. Add a `LICENSE` file before redistributing this project under a particular license.

## Search keywords & hashtags

`trace-removal` · `linux-log-auditing` · `bash-scripts` · `incident-response` · `digital-forensics` · `security-audit` · `system-administration`

#Cybersecurity #DigitalForensics #IncidentResponse #LinuxSecurity #BashScripts #SecurityTools #LogAuditing #ServerSecurity #SysAdmin #DefensiveSecurity #DFIR #BlueTeam
