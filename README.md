# SECURE DATA HIDING IN IMAGES USING STEGANOGRAPHY

This project provides a simple implementation of **image-based steganography**, where secret messages are hidden within an image and later retrieved using a decryption script. The encryption and decryption processes involve modifying the pixel values of an image to store message bytes.


## Requirements

```sh
pip install opencv-python
```

## Usage

### 1. Encrypting a Message

To hide a secret message in an image:

```sh
python encryption.py
```

#### Steps:

1. The script will ask for the image file (`img.jpg`).
2. Enter the secret message you want to hide.
3. Provide a password for security.
4. The encrypted image is saved as `encryptedImage.png`.
5. The password is stored in `key.txt`.

### 2. Decrypting a Message

To retrieve the hidden message from the encrypted image:

```sh
python decryption.py
```

#### Steps:

1. The script reads `encryptedImage.png`.
2. You must enter the correct password.
3. If the password matches, the hidden message is displayed.
4. If the password is incorrect, access is denied.

## File Descriptions

- **encrypt.py** - Script to embed a secret message into an image.
- **decrypt.py** - Script to extract the secret message from the image.
- **encryptedImage.png** - Image containing the hidden message.
- **key.txt** - Stores the password required for decryption.
- **mypic.jpg** - Original image used for encryption.

## Example

### Encrypting:

```sh
Enter secret message: Important Message
Enter a passcode: secretpass
Encryption done. Saved as 'encryptedImage.png'.
```

![image](https://github.com/user-attachments/assets/16885841-995b-4a72-b3c9-f1c0e6859039)


### Decrypting:

```sh
Enter password: secretpass
Secret message: Important Message
```

![image](https://github.com/user-attachments/assets/8adf06db-ecd2-4207-b2d1-e83bac6f13da)
