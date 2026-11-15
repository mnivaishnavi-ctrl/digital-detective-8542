# Mission 3 — Understand the Operating System

## Task/objective

Learn what an operating system does by checking this computer, viewing running processes, navigating folders, and inspecting a practice file's permissions.

## Work completed

- Checked the operating system, signed-in local account, disk space, and a brief activity snapshot. The account name and other personal identifiers are intentionally redacted.
- Viewed the running process list while Safari and Visual Studio Code were open.
- Navigated from the repository root into this mission folder and back.
- Created [permission-practice.txt](./permission-practice.txt) and inspected its detailed permissions. I did not change its permissions.
- Summarized six operating system responsibilities in the table below.

### Operating system responsibilities

| Responsibility | What it means | Simple example |
|---|---|---|
| Process management | Starts, schedules, and stops running programs. | The OS lets a browser and text editor take turns using the processor. |
| Memory management | Gives programs working memory and keeps their use organized. | The OS provides memory to a browser tab while another app is open. |
| Device management | Coordinates the computer and connected devices. | The OS sends a document to a printer or accepts keyboard input. |
| File management | Organizes files and folders and controls how they are stored and found. | The OS saves this practice file in the mission folder. |
| User interface/shell | Lets a person use the computer through windows, menus, or typed commands. | Finder provides a graphical interface; Terminal accepts shell commands. |
| Security and permissions | Controls access to accounts, files, and system resources. | File permissions can allow an owner to read and edit a file while preventing execution. |

## Commands/tools used

- `sw_vers` — checked the macOS version.
- `id -u` — checked the current local account identifier; it is omitted here to protect personal details.
- `df -h /` — checked total, used, and available storage.
- `uptime` and `vm_stat` — checked system uptime, load averages, and a brief memory-activity snapshot.
- `ps -Ao pid=,comm=` — viewed process IDs and process names while Safari and Visual Studio Code were open.
- `pwd` and `cd` — checked the current location and moved into and back out of the mission folder.
- `ls -l` — viewed the practice file's detailed permissions.
- `stat -f '%Sp'` — confirmed the practice file's symbolic permission mode.

## My understanding

An operating system manages the hardware and provides the services that apps and people use. A process is a running program or task. Its PID, or process ID, is a number the OS uses to identify it while it is running. Two examples seen in the process list were Safari (PID 1247) and Visual Studio Code (PID 1246); these PIDs describe only this snapshot and can change.

An absolute path starts at the filesystem root and names the full location. For example, `/Users/<redacted>/Desktop/digital-detective-8542/mission-03-operating-system/permission-practice.txt` is an absolute-path example; the personal account name is replaced with `<redacted>`. A relative path starts from the current folder. From the repository root, `mission-03-operating-system/permission-practice.txt` names the same file. From inside the mission folder, the relative path is just `permission-practice.txt`.

The permission listing for the practice file was `-rw-r--r--`. The owner's three permission positions are `rw-`: read is allowed, write is allowed, and execute is not allowed. The file is text, and I left its permissions unchanged.

The system snapshot reported macOS 27.2.1, a 926 GiB filesystem with 13 GiB used and 819 GiB available (2% capacity), and an uptime of about 2 days 14 hours with load averages around 2.06, 1.87, and 1.79. `vm_stat` reported 40,250 free, 229,347 active, 227,618 inactive, and 1,229 speculative memory pages (16 KiB per page). The account name and device identifiers are not included in this report.

## Difficulties faced

The process list included helper processes in addition to the main apps, so its output was longer than the examples needed. System commands can also display account and device identifiers.

## How I resolved them

I filtered the process snapshot to the relevant browser and editor, used the `ls -l` permission columns to identify the owner's permissions, and recorded only the required system facts. I redacted account and device details rather than saving them.

## Evidence/files

- [permission-practice.txt](./permission-practice.txt) — practice file used for path and permission inspection.
- This report records a concise summary of the command output; raw account identifiers and device names were not saved.

## Commit details

- Commit message: `Document operating system and file management`
- Branch: `main`
- The mission report and practice file, together with the Mission 3 status update in the root README, are committed together.