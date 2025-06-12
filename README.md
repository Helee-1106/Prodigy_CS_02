# Prodigy_CS_02
# 🔐 Image Encryption & Decryption Tool

This is a beginner-friendly Python tool for basic image encryption and decryption using pixel-level operations. It uses a simple numeric key to modify the RGB values of an image and can restore the original using the same key.

---

## ✨ Features

- 🔢 Encrypts images by applying a numeric key to each pixel
- 🔓 Decrypts using the same key to restore the original
- 📸 Supports standard image formats (JPEG, PNG, etc.)
- 🧠 Simple logic using NumPy and Pillow (PIL)
- ✅ Fully command-line based, no GUI needed

---

## 🛠️ How It Works

1. The image is converted into a NumPy array for pixel manipulation.
2. Each RGB value is modified using:
   - Encryption: `(pixel + key) % 256`
   - Decryption: `(pixel - key) % 256`
3. The processed image is saved locally.

⚠️ **Important:** Pixel values are wrapped using modulo 256 to keep them within the valid range (0–255).

---

## 📦 Requirements

- Python 3.x
- [Pillow](https://pypi.org/project/Pillow/)
- [NumPy](https://pypi.org/project/numpy/)

Install dependencies with:

```bash
pip install pillow numpy
