# Steganography Technique to Hide Information within an Image File

This repository contains the official research monograph, architectural layout, and comprehensive step-by-step system implementation documentation for a real-time digital asset encryption framework utilizing an optimized Least Significant Bit (LSB) embedding methodology.

---

## 📑 Core Research Asset

### 🔬 Academic Research Paper
* **Full Paper:** [Download the Complete Research PDF](./Research-Paper.pdf)
* **Presented At:** 2nd International Award Conference on Review, Research and Evaluate (Bangkok, Thailand)

### 📘 Engineering Project Report
* **Full Documentation:** [Download Full Project Report PDF](./Project-Report.pdf)
* **Cap-stone Engineering Report:** Major system design documentation and cryptographic deployment verification framework certified by AKTU University.

---

## ⚙️ Core Algorithm & Logic Breakdown

The software embeds encrypted text payload streams natively into digital display media utilizing pixel-level matrix manipulation to ensure minimal structural degradation of the cover medium.

### 🔑 Key Generation & Block Manipulation Matrix

1. **Source Parsing:** Read the cover image matrix from the source asset.
2. **Array Division:** The system segments the image frame into an array grid of independent processing blocks.
3. **Byte Distribution:** The insertion algorithm applies a custom 32-bit stego-key configured as follows:
   * **Bits 0–7:** Determine Row allocations ($R$).
   * **Bits 8–15:** Determine Column allocations ($C$).
   * **Bits 16–31:** Dictate the sequential pseudo-random pattern bits.

```text
If pattern_bit == 0 -> Adjust the 1st LSB of the target pixel channel.
If pattern_bit == 1 -> Adjust the 2nd LSB of the target pixel channel.
```
## 🗺️ System Process Flowcharts
The overall algorithmic data pipeline transitions seamlessly between standalone encryption and decryption nodes.

### Algorithmic Concept: Encryption Engine
The conceptual process mapping shows how the secret payload data stream is integrated with raw carrier pixels via the stego-key to yield an output bitmap asset.

### Algorithmic Concept: Decryption Engine
The reverse conceptual mapping demonstrates how the receiver node parses incoming pixel headers, evaluates channel bits against the shared key matrix, and isolates the intact payload file.

## 🖥️ System Architecture & UI Modules Detailed Walkthrough
The operational software was engineered across distinct execution modules to simulate real-time secure transmission over public infrastructure networks. Every interface state below corresponds to an essential transition in the data pipeline.

### 🔒 Module 1: The Encryption Encoder Pipeline

#### Step 1.1: Initialized Encoder Dashboard (01-encryption-ui-main.png)
The primary system console window upon system launch, featuring an unpopulated image viewer container, configuration options, and action fields.

#### Step 1.2: Cover File Stream Browser Node (02-select-cover-image.png)
The system triggers the operating system's native directory file browser node, allowing the system administrator to query and lock in the source cover medium asset.

#### Step 1.3: Asset Parsing Engine Dimensions Checked (03-cover-image-loaded.png)
The selected cover image is rendered into the primary application matrix container. The backend engine automatically evaluates image attributes, displaying the target pixel height and width dimensions on the configuration column.

#### Step 1.4: Selecting the Secret Document Payload (04-select-secret-file.png)
The user maps the precise secret file payload (Home.doc) containing the target information intended to be completely hidden inside the pixel blocks.

#### Step 1.5: Target Output Path Map Generation (05-encryption-processing.png)
The encoder pipeline generates a directory save prompt to define the storage path and lock in the output filename for the processed stego-medium array.

#### Step 1.6: Final Processing Matrix Confirmation (06-stego-image-saved.png)
The algorithm writes the bits into the matrix, finishes execution, and displays a verified system alert confirming that the encrypted image has been successfully created and saved to disk.

### 🔓 Module 2: The Receiver / Decoder Node

#### Step 2.1: Standalone Decoder Interface Node (07-decryption-ui-main.png)
The independent receiver workspace dashboard used to load, read, and extract information hidden inside altered images.

#### Step 2.2: Importing the Carrier Medium Array (08-decryption-load-stego.png)
The receiver application launches its file system picker tool to grab the incoming stego-image array off the shared folder directory.

#### Step 2.3: Validating Matrix Headers (09-stego-file-loaded.png)
The decoder engine accepts the input stego-bitmap, displays it inside the canvas container, and checks its array dimensions to ready the bit-extraction loops.

#### Step 2.4: Choosing Output Extraction Path (10-decryption-destination.png)
The receiver node specifies the local folder destination pathway where the restored document payload will be reconstructed.

#### Step 2.5: Complete Bitstream Reconstruction (11-decrypted-file-saved.png)
The application executes the inverse key manipulation algorithm, pulls the data from the designated LSB positions, restores the hidden text file, and pops up a successful system saving notification.

### 🔀 Multi-Instance Pipeline Profiles

#### Parallel Execution System Workspace View (12-pipeline-side-by-side.png)
An advanced runtime profile layout showing concurrent handling of file configurations, directory queries, and multiple program pipelines tracking active memory allocation modules simultaneously.

### 📊 Data Flow & Logic Modeling

**System Process Diagram: Encryption Engine (13-encryption-flowchart.jpg)**
The conceptual process mapping shows how the secret payload data stream (Information File) is integrated with raw carrier pixels (Image File) via the optimized LSB embedding methodology to yield an output bitmap asset (BMP File) without structural degradation.

**System Process Diagram: Decryption Engine (14-decryption-flowchart.jpg)**
The reverse conceptual mapping demonstrates how the receiver node parses the incoming stego-bitmap (BMP File) to extract the hidden payload data stream back into a standalone information document while preserving the original carrier image frame.

## 📁 Repository Directory Map

```text
├── images/               # Asset directory containing sequential execution screenshots and flowcharts
├── README.md             # Unbundled, step-by-step interactive portfolio documentation
├── Project-Report.pdf    # Capstone engineering system documentation and institutional thesis
└── Research-Paper.pdf    # Peer-reviewed research monograph publication
