# workshop
# Digital Forensics Workshop: Using Sleuth Kit & Autopsy
# 1. Introduction
Overview of Sleuth Kit (TSK) and Autopsy.
Use cases: Digital investigations, file recovery, and disk analysis.
# 2. Installation Guide
# A. Installing Autopsy (Includes Sleuth Kit)
Download Autopsy:
Visit Autopsy Download Page.
Download the Windows installer.
Install Autopsy:
Run the installer and follow instructions.
# B. Installing Sleuth Kit (Standalone)
Download Sleuth Kit:

Visit Sleuth Kit Download Page.
Extract files to a directory.
Set Up Environment (Optional for CLI Use):

Add the Sleuth Kit folder to your system PATH to use commands globally.
# 3. Basic Sleuth Kit Commands
# A. Identifying File System Type
sh
Copy
fsstat /path/to/disk/image
Displays details about the file system (FAT, NTFS, EXT).
# B. Listing Partitions
sh
Copy
mmls /path/to/disk/image
Shows partitions inside a disk image.
# C. Extracting Partition Data
sh
Copy
fls -o <sector_offset> /path/to/disk/image
Lists files in a partition (including deleted files).
# D. Recovering Deleted Files
sh
Copy
icat -o <sector_offset> /path/to/disk/image <inode_number> > recovered_file
Extracts a deleted file using its inode number.
# E. Viewing File Metadata
sh
Copy
istat /path/to/disk/image <inode_number>
Displays metadata of a file, including timestamps.
# F. Searching for Specific Files
sh
Copy
find /path/to/disk/image -name "*.txt"
Finds all .txt files in the image.
# G. Extracting Strings from a Disk Image
sh
Copy
strings /path/to/disk/image | grep "keyword"
Searches for text patterns in the disk image.
# H. Viewing Master Boot Record (MBR)
sh
Copy
dd if=/path/to/disk/image bs=512 count=1 | xxd
Displays the MBR of the disk.
# 4. Using Autopsy for GUI-Based Analysis
# A. Launching Autopsy
Open Autopsy in a web browser.
Click "Create New Case" and enter details.
# B. Adding a Data Source
Select "Add Data Source".
Choose:
Disk Image (E01, VMDK, raw).
Local Drive (e.g., C:).
Folder (e.g., C:\Users\Public).
Click "Start Analysis".
# C. Investigating Files
Recover Deleted Files

Navigate to File System.
Look for red-colored (deleted) files.
Right-click → Extract.
Keyword Search

Search for terms like "password", "confidential".
Check User Activity

View Windows Registry, browser history, recent documents.
# 5. Hands-on Demonstrations
# Scenario 1: Recovering a Deleted Document
Use fls and icat in Sleuth Kit.
Confirm recovery with Autopsy.
# Scenario 2: Searching for Suspicious Keywords
Use strings to extract text from raw disk data.
# Scenario 3: Identifying Recently Accessed Files
Use istat to check timestamps.
# 6. Conclusion
Summary of findings.
Discuss real-world forensic applications.
Q&A session.
