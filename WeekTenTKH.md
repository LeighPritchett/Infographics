## **Source – Week 10 Overview (Digital Forensics & Evidence Recovery)**  
**Focus:** Disk Imaging, Inode Analysis & Forensic Data Recovery

Week 10 shifted the focus from incident detection to evidence handling. The core theme was understanding how data actually lives on a disk — not as files and folders, but as inodes, metadata structures, and raw sectors. The week emphasized how forensic analysts reconstruct events by examining what the operating system leaves behind, even after deletion.

Key ideas included how file systems track metadata, how inodes reveal the history and state of a file, and why deleted data may or may not be recoverable depending on allocation status. The mindset: **forensics is about proving what happened, not just finding artifacts.**

---

## **Source – Disk Imaging & Evidence Integrity**  
**Key Concepts & Skills:**  
**Forensic Imaging:** Creating a bit‑for‑bit copy of a drive to preserve original evidence.  
**Hashing for Chain of Custody:** Using SHA256 to verify that the evidence image has not been altered.  
**Read‑Only Analysis:** Ensuring all investigation happens on the image, never the original disk.

These principles reinforce the legal and procedural side of digital forensics — accuracy, repeatability, and defensibility.

---

## **Source – Inode Structures & File System Metadata**  
**Key Concepts & Skills:**  
**Inode Analysis:** Understanding how file metadata persists even after deletion.  
**Allocated vs. Unallocated:** How the OS marks data blocks as free without actually wiping them.  
**Metadata‑Driven Investigation:** Using inode information to determine file history, size, timestamps, and block locations.

This source taught me that even when a file is gone, the inode often tells the story of what it used to be.

---

## **Source – Sleuth Kit Tools (`fls`, `istat`, `icat`)**  
**Key Concepts & Skills:**  
**`fls`:** Enumerate files, including deleted ones, by scanning the file system structure.  
**`istat`:** Inspect inode metadata to determine file status and block locations.  
**`icat`:** Attempt file extraction directly from inode references.

These tools showed how forensic analysts move beyond the GUI and interact directly with the file system’s internal structures.

---

## **Source – Sector‑Level Carving & Data Recovery Limits**  
**Key Concepts & Skills:**  
**Block‑Level Carving:** Using `dd` to extract raw sectors when file‑level recovery fails.  
**Hex Analysis:** Interpreting raw bytes to determine whether meaningful data remains.  
**Overwritten Data:** Understanding that once a block is overwritten, recovery is impossible — and documenting that outcome is still valid forensic work.

This reinforced that forensics isn’t always about “finding the smoking gun.” Sometimes the value is in proving that the data is gone and showing the steps taken to reach that conclusion.

---

## **Overall Learning Mindset – Week 10**  
Digital forensics requires precision, patience, and a deep understanding of how data is stored at the lowest levels. This week taught me how to think like an analyst: follow the metadata, validate every step, and document the process even when the evidence is incomplete. The goal is not just recovery — it’s building a defensible narrative of what happened on the system.
