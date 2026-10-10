# Trace Removal & Security Audit Tools

Read-only shell utilities for **authorized server administration, incident response, and digital-forensics review**. The scripts help inventory common log locations and inspect log-directory usage without changing the host.

> **Safety first:** The shell scripts currently provided in this repository are audit-only. They do not erase logs, alter timestamps, conceal processes, disable security controls, or remove system files. Preserve original evidence and follow your organization's incident-response and retention policies.

## Features

- Inspect common log directories when present and readable.
- Report disk usage for `/var/log`, `/var/log/audit`, and `/var/log/journal`.
- List recent log-file metadata (timestamp, size, and path) without printing log contents.
- Run in a non-destructive mode suitable for an initial review.

## Repository layout

The shell scripts are kept in their named project directories under `trace_removal/`:

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

- Linux with Bash
- Standard utilities such as `date`, `find`, `sort`, `head`, and `du`
- Read permission for the log paths you want to inspect

## Usage

From the repository root, run a script by its path, for example:

```bash
bash trace_removal/Advanced_Security_Operations_Script/advanced_security_operations.sh
```

The scripts inspect standard system log paths. If permissions restrict access, the report may omit those details; run only on systems you administer and follow local authorization requirements.

## Responsible use

- Use only on systems you own or are explicitly authorized to assess.
- During an investigation, preserve logs and metadata; work from copies when possible.
- Do not use cleanup procedures to hide unauthorized activity or destroy evidence.
- Review any script before running it, and test changes in a disposable environment first.

## License

No license is specified yet. Add a `LICENSE` file before redistributing this project under a particular license.

## Topics

#cybersecurity #digital-forensics #security-tools #server-security #incident-response #linux #bash #log-auditing #sysadmin
