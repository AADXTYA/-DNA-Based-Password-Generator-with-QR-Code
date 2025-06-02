# -DNA-Based-Password-Generator-with-QR-Code

Purpose: This Python project generates a secure password from a randomly created DNA sequence (using A, T, C, G), adds complexity by converting it to symbols, and encodes both the DNA and password into a scannable QR code.

DNA Sequence Generation: A random 40-character DNA sequence is created using random.choices() from the bases A, T, C, and G.

Symbol Mapping: Each DNA base is mapped to a special symbol (A → @, T → #, C → $, G → %) to add visual and structural complexity.

Password Creation: The symbolic DNA is combined with the first 8 characters of a SHA-256 hash of the sequence, then shuffled to enhance randomness.

QR Code Generation: The DNA sequence and generated password are embedded into a QR code using the qrcode library, saved as dna_password_qr.png, and displayed using PIL and IPython.display.

Requirements: Required libraries include biopython, qrcode, Pillow, and IPython.display. Install them using pip install biopython qrcode pillow.

Execution: The project can be run in Jupyter Notebook (QR displayed directly) or in VS Code (QR image saved). The QR code can be scanned with any QR reader to reveal the DNA and password.

Optional Extension: The project can be enhanced with GUI, encryption, web integration, or even biometrics for higher uniqueness.
