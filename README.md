📌 **Project Title:** **InstaFlow — Photo & Video Organize**  
📅 **Project Timeline:** **December 2025 – Present [Active Development & Maintenance]**  
🎥 YouTube Demo: TBD  
📦 GitHub Source Code: <https://github.com/IvanSicaja/2025.12.26_RND_software_workflow--InstaFlow>  

---

📍 My Personal Profiles ⬇︎  
🎥 Video Portfolio: To be added  
📦 GitHub Profile: <https://github.com/IvanSicaja>  
👔 LinkedIn: <https://www.linkedin.com/in/ivan-si%C4%8Daja-832682222>  
🎥 YouTube: <https://www.youtube.com/@ivan_sicaja>  

---

### 💡 Core Challenge This Project Resolves:

Accelerating repetitive photo and video organization workflows by providing a keyboard-driven desktop interface for visually reviewing media and sorting files into configurable destination folders through controlled copy or move operations.

---

### 🔧 Core Skills Tree Used To Build The Project - Skills and Tech Stack:
*(Project-Specific Structured Overview)*
```
│
├── Software Engineering
│ ├── Software / Frameworks / Libraries
│ │ ├── Python
│ │ ├── PyQt6
│ │ ├── rawpy
│ │ ├── NumPy
│ │ ├── Python shutil
│ │ ├── Python threading
│ │ ├── OrderedDict
│ │ └── QSettings
│ │
│ └── Skills
│   ├── Desktop GUI application development
│   ├── Object-oriented software design
│   ├── Event-driven application architecture
│   ├── Keyboard-driven workflow design
│   ├── Background data preloading
│   ├── Thread-safe cache management
│   ├── Persistent application settings
│   ├── File-system operations
│   └── Error handling & user feedback
│
├── System Integration Engineering
│ ├── Software / Frameworks / Libraries
│ │ ├── PyQt6
│ │ ├── Native file system
│ │ ├── QSettings
│ │ ├── shutil
│ │ └── rawpy
│ │
│ └── Skills
│   ├── GUI-to-filesystem integration
│   ├── Source-to-destination folder integration
│   ├── Keyboard-to-workflow integration
│   ├── Image-decoder integration
│   ├── Persistent configuration management
│   ├── File copy & move orchestration
│   ├── Operation logging
│   └── End-to-end media sorting workflow integration
│
├── Media & File Workflow Automation
│ ├── Software / Frameworks / Libraries
│ │ ├── QPixmap / QImage
│ │ ├── rawpy
│ │ ├── NumPy
│ │ ├── shutil.copy2
│ │ └── shutil.move
│ │
│ └── Skills
│   ├── Visual media review workflows
│   ├── Recursive source-folder scanning
│   ├── Configurable destination folders
│   ├── Keyboard-based media classification
│   ├── COPY / MOVE workflow automation
│   ├── RAW image decoding
│   ├── Media preview caching
│   ├── File deletion workflow
│   └── Operation history logging
│
└── Research & Development Engineering
  ├── Software / Frameworks / Libraries
  │ └── Integrated within sections above
  │
  └── Skills
    ├── Media workflow architecture
    ├── Desktop workflow optimization
    ├── Interactive sorting workflow design
    ├── Performance-oriented preview loading
    ├── File-management automation
    ├── User interaction refinement
    └── Technical debugging & reliability improvement
```

---

### 📋 Core System Capabilities - List Only:

- **Photo & video organization workflow**
- **Recursive source-folder scanning**
- **Visual media preview**
- **Keyboard-based media navigation**
- **Keyboard-based destination sorting**
- **Configurable shortcut-to-folder mapping**
- **COPY and MOVE operation modes**
- **Source-folder or custom target-folder selection**
- **Dynamic destination-folder management**
- **Existing subfolder loading**
- **Automatic destination-folder creation**
- **RAW image decoding**
- **Background preview preloading**
- **Thread-safe image cache**
- **Current and neighboring media previews**
- **Permanent file deletion with confirmation**
- **Operation logging**
- **Duplicate destination-file validation**
- **Persistent source and target settings**...

---

### 🧠️ How It Works - Core System Capabilities Workflow:

The project combines different software-engineering areas (**desktop GUI development, media organization, filesystem automation, keyboard-driven interaction, file copy / move operations, RAW image decoding, multithreading, caching, persistent configuration, logging...**)  
The core of the application is **Python**, **PyQt6**, **rawpy**, **NumPy**, and native filesystem operations. The supplied implementation explicitly supports a broad range of standard and RAW image formats and uses dedicated RAW decoding for camera formats.

The application is also equipped with:

- **Visual media review**
- **Keyboard-driven sorting**
- **Configurable destination folders**
- **COPY / MOVE modes**
- **Background media preloading**
- **Operation logging**...

**Source-folder loading:**  
InstaFlow loads supported media from a selected source directory and recursively searches its subfolders. The resulting file paths are sorted and stored relative to the selected root folder, preserving information about their original subfolder location.

**Media preview:**  
The active media item is displayed in a large central preview together with neighboring preview items for faster visual navigation. Standard image formats are loaded through Qt, while supported camera RAW formats are decoded using **rawpy** and converted into Qt-compatible image data.

**Background preloading:**  
A dedicated background thread preloads media around the currently selected item. An in-memory **OrderedDict** cache retains recently used pixmaps and removes older entries when the configured cache capacity is exceeded, reducing repeated decoding during navigation.

**Keyboard navigation:**  
The left and right arrow keys move backward or forward through the loaded media collection. Whenever the active index changes, the main preview and neighboring previews are refreshed and the background cache begins preloading around the new position.

**Destination-folder configuration:**  
Users can sort media either into subfolders of the current source folder or into a separately selected target directory. Existing destination subfolders can be loaded automatically, while additional folder names can be configured and created directly from the application.

**Configurable sorting shortcuts:**  
Each destination folder can be associated with a keyboard shortcut. Numeric keys and configurable letter keys allow the currently selected media item to be routed directly into the corresponding destination folder without requiring repeated mouse-based file operations.

**COPY / MOVE workflow:**  
InstaFlow supports two file-management modes. **COPY** duplicates the current file into the selected destination while retaining the source file. **MOVE** transfers the file into the destination and removes it from the active source sequence. Existing destination files are checked before an operation is executed.

**Operation logging:**  
COPY, MOVE, and DELETE operations are written to an `instaflow_log.txt` file together with timestamps and relevant source / destination information. The log keeps a limited recent history of operations.

**Media deletion:**  
The currently selected file can be permanently deleted through the interface or its keyboard shortcut. Deletion requires explicit confirmation, updates the active media collection, records the operation in the log, and advances the preview to the next available item.

**Persistent configuration:**  
Qt **QSettings** stores selected source and target-folder information so frequently used locations can be restored between application sessions.

---

### ⚠️ Note:

The provided project scope identifies InstaFlow as a **photo and video organization** application. However, the supplied source-code version explicitly lists and previews image and RAW-image formats; dedicated video-format extensions or video playback logic are not present in the provided implementation. Video-specific handling should therefore not be interpreted as verified from this source version.

---

### 📸 Project Snapshots:

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

---

### 🎥 Video Demonstration:

<p align="center">
TBD
</p>

---

### 📣 Hashtags Section:

**#InstaFlow #PhotoOrganizer #VideoOrganizer #MediaOrganizer #MediaWorkflow #Python #PyQt6 #RAWPhotography #RawPy #NumPy #DesktopApplication #FileSystemAutomation #WorkflowAutomation #SystemIntegration #SoftwareEngineering #MediaManagement #FileManagement #Multithreading #Caching #ResearchAndDevelopment**

<!-- README requirements and required project input: -->