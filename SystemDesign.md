Problem Statement
“The problem is to develop a secure and scalable system for protecting sensitive medical images from unauthorized access, tampering, and future quantum computing threats by utilizing quantum cryptography, and quantum-resistant encryption algorithms, while ensuring compliance with healthcare privacy regulations.”
PROPOSED DESIGN:
Workflow Summary: 
-Image Acquisition → Compression → Encryption (Quantum + Classical) → Secure Transmission.
-The encrypted data is securely transmitted to a cloud database and stored.
-Decryption (Quantum + Classical) → Error Detection → Image Reconstruction completes the process on the receiving end.
The process for securing medical images using quantum cryptography begins with image processing. Initially, the medical image is captured through an imaging device such as an X-ray, MRI, or CT scanner. To make the image more efficient for transmission, it undergoes image compression, reducing the data size without significant loss of quality. Once the image is transmitted, it is then reconstructed back to its original form, allowing healthcare providers to use the image for diagnosis and medical analysis.
1.Login: The system prompts the user to "ENTER USERNAME AND PASSWORD."
2.Authentication: The entered credentials are checked against the system's database.
-If the username and password are valid: The system proceeds to the "ADMIN PAGE" node, signifying successful authentication.
-If the username and password are invalid: The user is directed to the "INVALID USERNAME OR PASSWORD? TRY AGAIN" node, prompting them to re-enter their credentials.
3.Admin Page: The user accesses the admin page, which offers the following functionalities:
4.Encrypt Image: This option allows the administrator to encrypt an image.
5.Decrypt Image: This option enables the administrator to decrypt an image.
6.Change Password: This option allows the administrator to modify the system password.
7.Successful Operation: After performing any of the admin functions, the system asks if the operation was "SUCCESSFUL?"
-If yes: The system proceeds to the "STOP" node, indicating successful execution.
-If no: The system does not progress further, implying an error or unsuccessful operation.
In essence, this flowchart illustrates a basic administrative system that authenticates user access, provides administrative functionalities, and handles both successful and unsuccessful scenarios.

 Components of System Design: 

Component|Description
Medical Image Acquisition:Captures medical image data.
Image Compression: Compresses image for efficient storage/transmission.
Quantum Key Generation (QKG):	Creates quantum key for encryption.
Classical Encryption:	Adds an extra encryption layer (e.g., AES/RSA).
Quantum Encryption (QSDC):	Encrypts image with the quantum key.
Secure Transmission:	Ensures secure transmission of data.
Cloud Database:	Stores data securely in the cloud.
Quantum Decryption:	Decrypts data using the quantum key.
Classical Decryption:	Removes classical encryption layer.
Image Reconstruction:	Reconstructs the image after decryption.
Error Detection Module:	Detects transmission errors and initiates retransmission.
