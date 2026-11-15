# Mission 2 — Become Comfortable with the Terminal

## Task 2.1 — Basic Terminal operations

| Operation | Command | What it does / what I observed |
|---|---|---|
| Show current folder | `pwd` | Shows the full path. It showed that I was in my project folder; I left my username out of these notes. |
| List files | `ls` | Shows the files and folders. I saw the items in my project. |
| Detailed list | `ls -lh` | Shows more details, including sizes and dates. |
| Go to parent folder | `cd ..` | Moves up one folder. I moved from the project folder to Desktop. |
| Create a practice folder | `mkdir -p mission-02-terminal/terminal-practice` | Created a folder for this practice. |
| Create an empty file | `touch mission-02-terminal/terminal-practice/notes.txt` | Created an empty text file. |
| Copy a file | `cp mission-02-terminal/terminal-practice/notes.txt mission-02-terminal/terminal-practice/backup.txt` | Made a copy of the empty file. |
| Rename the copy | `mv mission-02-terminal/terminal-practice/backup.txt mission-02-terminal/terminal-practice/final_backup.txt` | Renamed the copied file. |
| Display file contents | `cat mission-02-terminal/terminal-practice/notes.txt` | Displayed the original file. It was empty, so nothing appeared. |

## Task 2.2 — Practise file changes safely

I made `terminal-practice/notes.txt`, wrote one line, and added a second line. I displayed the file and saw both lines. I copied it to make a backup and renamed the backup.

- Replacing text with `>` writes new contents over the file. Appending with `>>` adds text at the end.
- Copying makes another file and leaves the original. Moving changes the file's location or name.
- `pwd` tells me which folder I am working in.
- `ls` helps me see which files and folders are there.

## Task 2.3 — Flags and pipes

I compared `ls` with `ls -lah`. The detailed listing showed extra information. `-l` shows a detailed list, `-a` includes hidden entries, and `-h` makes file sizes easier to read.

I used `ls -lah mission-02-terminal | head -n 5` to show only the first five lines of the listing. The pipe `|` sends the listing from `ls -lah` to `head`, and `head` displays the first few lines. I redacted the computer account name before keeping any output.

## Task 2.4 — Package managers

Homebrew is installed. Its version is 6.0.18, and I viewed its list of five formula packages. I did not install or remove anything.

A package manager helps install and update software from one place. It can also manage other software a program needs.

## 1. Task / objective

Practise Terminal commands, manage files safely, understand flags and pipes, and learn what a package manager does.

## 2. Work completed

I checked folders, created and copied practice files, appended text, compared directory listings, used a pipe, and checked Homebrew.

## 3. Commands / tools used

- `pwd`, `ls`, `ls -lh`, `cd ..` — checked my location and listed folders.
- `mkdir`, `touch`, `cp`, `mv`, `cat`, `printf` — created, copied, renamed, and displayed practice files.
- `>`, `>>` — wrote to a file and added text to the end.
- `ls -lah`, `head -n 5`, `sed` — viewed a detailed listing, limited the displayed lines, and redacted account information.
- `brew --version`, `brew list --formula` — checked Homebrew and viewed its formula list.
- `git add`, `git commit`, `git push` — staged the Mission 2 files, saved a commit, and uploaded it.

## 4. My understanding

Terminal commands let me check and manage files by typing. Flags change the information a command shows. A pipe sends one command's output to another command. A package manager helps manage software.

## 5. Difficulties faced

Some detailed command output included my computer account name.

## 6. How I resolved them

I left the full path out of the README and redacted the account name from the listing output.

## 7. Evidence / files

- `terminal-practice/notes.txt`
- `terminal-practice/final_backup.txt`
- `terminal-practice/notes.txt`
- `terminal-practice/final-backup.txt`
- This README has the command reference and answers.

## 8. Commit details

- Commit message: `Complete Terminal and file management mission`
- The completed Mission 2 work was pushed to GitHub.