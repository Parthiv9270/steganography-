# Image Steganography with Python (OpenCV)

This project demonstrates a simple **image steganography technique** using Python and OpenCV.  
It allows you to **hide a secret message inside an image** and later retrieve it using a password.

---

##  Features
- Hide a text message inside an image.
- Retrieve the hidden message with the correct password.
- Uses basic pixel value manipulation.
- Lightweight and easy to understand.

---

##  Requirements
Make sure you have Python installed along with the required libraries:

```bash
pip install opencv-python
```

---

##  Usage

1. Place your input image in the project folder (e.g., `img1.jpeg`).
2. Run the script:

```bash
python py.py
```

3. Enter:
   - The **secret message** you want to hide.
   - A **password** for protection.

4. The program will create an encrypted image (`encryptedmsg1.jpeg`) with the hidden message.

5. To decrypt:
   - Run the same script again.
   - Enter the **same password**.
   - The hidden message will be revealed in the terminal.

---

##  File Structure
```
.
├── img1.jpeg              # Original image (input)
├── encryptedmsg1.jpeg     # Image with hidden message (output)
├── py.py                  # Main Python script
└── README.md              # Project documentation
```

---

## 📝 Example

**Encryption:**
```
Enter secret message: Hello World
Enter password: 1234
```

➡ Generates `encryptedmsg1.jpeg` with hidden message.

**Decryption:**
```
Enter passcode for Decryption: 1234
Decryption message: Hello World
```

---

##  Notes
- This is a **basic steganography method** (not secure for real-world use).
- Message length is not stored separately, so encryption and decryption must use the same image and session.
- Password is only used for verification, not actual cryptographic encryption.

---

## 🚀 Future Improvements
- Store message length inside the image.
- Apply real encryption (AES, RSA, etc.) before hiding.
- Support longer messages and multiple image formats.

---

 Developed with ❤️ using Python & OpenCV
