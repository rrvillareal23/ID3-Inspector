# ID3 Inspector

A forensic-style tool for inspecting and analyzing ID3 metadata embedded in MP3 files.  
Supports ID3v2.2, ID3v2.3, and ID3v2.4 tag parsing, including image extraction and hex-level frame dumps.

## 🔍 Features

- Parses ID3v2.x headers and frame metadata
- Displays tag version, size, and flags (e.g. unsynchronization, extended headers)
- Hex + ASCII display of each frame’s content
- Extracts and counts embedded images (APIC, PIC frames)
- Detects known text, URL, and user-defined tags
- Ideal for digital forensics, data recovery, or learning about MP3 metadata internals

## 📂 Example Output

ID3 Version: 3  
Tag Size: 2586 bytes  
Flags: unsynchronization=False, extended header=False, experimental=False  

Frame: TIT2 (Title/songname/content description)  
Size: 30 bytes  
Flags: tag_alter_preservation=False, file_alter_preservation=False  
----------------------------------------  
00000000  00 54 65 73 74 20 53 6f 6e 67 20 54 69 74 6c 65   .Test Song Title  
00000010  20 45 78 61 6d 70 6c 65 00 00 00 00 00 00 00 00    Example........

## 🛠️ Usage

Run the script with the following command:

`python id3_inspector.py path/to/file.mp3`

**✅ Requires Python 3.x**

## 📥 Installation

Clone the repository:

`git clone https://github.com/yourusername/id3-inspector.git`

Navigate into the project folder:

`cd id3-inspector`

Run the script:

`python id3_inspector.py your_audio.mp3`
