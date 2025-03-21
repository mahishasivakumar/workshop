
# Workshop on Digital Forensics
Installation and Usage of Sleuth Kit & Autopsy
```
Register Number: 212222040095
Name: Mahisha S
```
## Introduction
Digital forensics involves extracting and analyzing data from digital devices to investigate cybercrimes. Sleuth Kit and Autopsy are widely used open-source tools for forensic analysis.

## Installation Steps
### A. Installing Sleuth Kit & Autopsy on Windows
1.Download Autopsy
- Visit Autopsy Official Website and download the latest version.
- Double-click the downloaded file and follow the on-screen instructions.
  ![image](https://github.com/user-attachments/assets/d1e21009-871f-4bc3-9799-60ece667cae0)



2.Installation Process
- Launch Autopsy to check if it works correctly.
- ![Screenshot 2025-03-20 113724](https://github.com/user-attachments/assets/cb96e1fc-9f2d-4b6c-9d8e-6e603deabb32)
   

- Choose Directory
- ![Screenshot 2025-03-20 113742](https://github.com/user-attachments/assets/b0afd4a0-d933-4b22-a83d-da397b18320c)
  

- Give install
  ![Screenshot 2025-03-20 113755](https://github.com/user-attachments/assets/80078b24-50c2-4d69-88fe-79802f361ac0)

  ![Screenshot 2025-03-20 113817](https://github.com/user-attachments/assets/1a04187c-2010-4425-a8b6-9bd2f1745ea3)


- Successfully installed
  ![Screenshot 2025-03-20 113938](https://github.com/user-attachments/assets/f17ca1d6-abcd-4969-aaf1-6ab38ea63a03)


- Autopsy Interface
  ![Screenshot 2025-03-19 222716](https://github.com/user-attachments/assets/3f8dfb03-55b2-4553-8475-de3595a56ff0)

## B. Installing Sleuth Kit Separately (Optional)
Download Sleuth Kit from www.sleuthkit.org/sleuthkit/download.php.
![{FAC04ED6-02D9-4D2A-A73C-CDADA79B7939}](https://github.com/user-attachments/assets/216ff656-18eb-497f-a795-3ca4112e758c)

Extract and install it manually if needed.
Add the installation directory to the system PATH for easy command-line access.
![Screenshot 2025-03-20 115043](https://github.com/user-attachments/assets/6d1b8f6b-9719-470e-b8bb-dce3543e2ff4)
## Using Autopsy to Analyze a Disk or Folder
## 1.Launch Autopsy and Set Up a New Case:

- Run Autopsy as Administrator.

- Click Create New Case.
![Screenshot 2025-03-19 222716](https://github.com/user-attachments/assets/4028e969-add1-46c4-beb2-3f336c7dcd3d)

- Enter a case name (e.g., Autopsy1).
- Select a location for the case folder → Click Next → Finish.
  ![Screenshot 2025-03-20 101159](https://github.com/user-attachments/assets/96e4d9e3-403b-47e7-985c-48bfd5ee65e8)

- Add optional information
  ![Screenshot 2025-03-20 101237](https://github.com/user-attachments/assets/97a42cf6-4e45-4bca-9ee0-fc11c6a52b4c)

 ## 2.Add the Partition as Evidence:

- Click Add Data Source → Choose Host.
   ![Screenshot 2025-03-20 101338](https://github.com/user-attachments/assets/2cae65dd-0d06-43ef-989e-7f07dad19883)



- Select Local Disk → Click Next.
   ![Screenshot 2025-03-20 101349](https://github.com/user-attachments/assets/0eafbcca-b430-45c7-9f0c-b6c5254d799b)



- Choose Disk → Select the VHD drive (Drive1).
  ![Screenshot 2025-03-20 101605](https://github.com/user-attachments/assets/44d4a210-6c1d-463c-9e0e-fd8b2551bc7c)



- Click Next → Keep the default settings → Click Finish.
  ![Screenshot 2025-03-20 101752](https://github.com/user-attachments/assets/ced6643a-ef0b-4de8-b4b6-b9bae1e9ac44)

- Allow Autopsy to process the disk.
## C. Running the Analysis
1.Start processing the disk or folder.
2.Wait for Autopsy to generate reports.
3.Analyze deleted files, metadata, and hidden data in the results.
## Using Sleuth Kit from Command Line
### A. Checking sleuthkit version
```
sh
fls -V
```
![Screenshot 2025-03-20 115043](https://github.com/user-attachments/assets/6d1b8f6b-9719-470e-b8bb-dce3543e2ff4)

### B.  Lists partition layout
```
sh
mmls
```
![Screenshot 2025-03-20 115251](https://github.com/user-attachments/assets/ed6046f7-06dc-47b9-9f59-a16e1751f938)

### C.  Lists files and directories
```
sh
fls
```
![Screenshot 2025-03-20 115417](https://github.com/user-attachments/assets/78fc4445-76db-40d0-a64b-2af1e4ccb7ab)

## Conclusion
By following these steps, you can install Sleuth Kit & Autopsy and analyze a disk or folder from the C drive. These tools help in digital investigations, allowing forensic experts to recover and analyze digital evidence.

