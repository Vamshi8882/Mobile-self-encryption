# Mobile-self-encryption
Mobile Self Encryption is a Python Tkinter-based desktop application for secure file protection. It uses AES-256 for file encryption, RSA-2048 for key management, and SHA-256 for integrity verification. A blockchain-based log records all encryption and decryption actions locally without any cloud dependency.

The application is built using Python Tkinter, allowing users to encrypt and decrypt files easily through a simple graphical interface.

📌** Features **

🔐 AES-256 Encryption for strong file security
🔑 RSA-2048 Key Pair for secure key management
🧾 SHA-256 Hashing for data integrity verification
⛓ Blockchain Audit Log to track encryption and decryption activities
📦 Chunk-based file processing for efficient large file encryption
🖥 User-friendly Tkinter GUI with simple controls
🌐 Fully Offline Operation – no cloud or network dependency

⚙️ ** Technologies Used **
Technology	Purpose
Python	Core programming language
Tkinter	GUI development
Cryptography Library	AES and RSA encryption
hashlib	SHA-256 hashing
os & time	File handling and timestamps

🏗 ** System Architecture **
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/380617bb-98d2-40a4-ab94-c91975d19579" />

The project follows a four-layer architecture:
1️⃣ ** GUI Layer **
Built using Tkinter, providing buttons and dialogs for user interaction.                                   
2️⃣ ** Logic Layer **
Handles application logic including:
File selection
Encryption and decryption
Authentication
Blockchain transaction recording
3️⃣ ** Cryptographic Engine **
Implements:
AES-256 for encryption
RSA-2048 for key generation
SHA-256 for hashing
4️⃣ ** Storage & Audit Layer **
Stores:
RSA key files (public_key.pem, private_key.pem)
Encrypted files
Decrypted files
Blockchain transaction logs


🔄 ** Workflow **

1️⃣ User selects a file
2️⃣ RSA key pair is generated or loaded
3️⃣ AES-256 key is generated using secure randomness
4️⃣ File is encrypted in 1KB chunks
5️⃣ SHA-256 hash is calculated for integrity
6️⃣ File is replaced with encrypted version
7️⃣ Transaction is recorded in the blockchain log

For decryption:
User authenticates
Private key is used
File is decrypted and saved with timestamp

🖥 ** Application Interface **

The GUI provides four main operations:
Select File – Choose a file for encryption or decryption
Encrypt and Replace – Encrypt the file using AES-256
Decrypt – Decrypt the file using RSA authentication
Show Blockchain – Display transaction history

📂 **Project Structure**
** Mobile-Self-Encryption
│
├── main.py
├── private_key.pem
├── public_key.pem
├── encrypted_files/
├── decrypted_files/
└── README.md **

🚀** How to Run the Project **
1️⃣ ** Install dependencies **
pip install cryptography
2️⃣ ** Run the application **
python main.py
The GUI window will open and you can start encrypting files.

** Output **
      <img width="212" height="483" alt="Screenshot 2026-03-13 120102" src="https://github.com/user-attachments/assets/c98e2526-1e62-4f89-a2a8-be95747a0d0f" />

🎯 ** Applications **
Personal file protection
Secure storage of sensitive documents
Healthcare data protection
Corporate confidential file management
Academic and research data security

✅ ** Advantages **
Strong encryption using modern algorithms
Efficient chunk-based file processing
Local execution without internet dependency
Tamper-evident blockchain logging
Simple graphical user interface

📜 ** License **
    This project is developed for educational and research purposes.

👨‍💻 ** Author **
      G. Vamshi
