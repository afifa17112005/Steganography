# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1: 
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROGRAM:
StegExpose and File Signature Analysis Commands

## OUTPUT:
- **1.Install and Set Up StegExpose**
• Download the StegExpose .jar file from the official repository.
• Ensure Java Runtime Environment (JRE) is installed.
• Run the tool on an image or a folder of images:\

• The output will list detection scores and a "suspect" verdict if steganography
is found.

- **2.Scan Individual Files**
• Run StegExpose on a single image:

The tool uses statistical analysis methods like RS analysis, Sample Pair
analysis, and Chi-square attack to detect hidden content.

- **3.Analyze File Signatures**
• Use Linux commands to verify the file's true format:

Every file type has a magic number (e.g., JPEG files start with FFD8). Comparing
the actual signature with the file extension helps identify mismatches or embedded
file tricks.

- **4. Cross-Check File Behavior**
• Rename the file (e.g., mv suspicious.jpg suspicious.zip) and try extracting it:

o Sometimes, files are disguised (e.g., a ZIP file hidden as a JPG), and this
trick helps uncover such embedded archives.

- **5.Optional: Use Other Tools**

o Tools like binwalk, stegsolve, or zsteg can be used for deeper analysis,
especially for PNG files or binary dumps.

![image](https://github.com/user-attachments/assets/035e8786-9c28-4fea-ab5c-d8043da8a4fd)

![image](https://github.com/user-attachments/assets/1a6903cd-cfa0-4fa7-837f-a34efa0a809c)

![image](https://github.com/user-attachments/assets/89fdac1b-baf2-4600-9490-f9eb4dd4eee1)


![image](https://github.com/user-attachments/assets/0f694699-9645-4aac-a938-8962943a920c)

![image](https://github.com/user-attachments/assets/1482628d-4f2c-4a26-bfb1-62edd5b5efe1)


![image](https://github.com/user-attachments/assets/4400dbfd-0fc9-4233-a6f3-9261bb569eca)



## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
