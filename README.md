---

# Vigenère Cipher Encryption and Decryption

This project demonstrates the implementation of the **Vigenère Cipher** algorithm, a classical encryption method used for encrypting and decrypting messages. The algorithm was implemented as part of a learning project on **freeCodeCamp**.

### Features:
- **Encrypt** a message using a custom key.
- **Decrypt** a message using the same key.
- Handles both lowercase and uppercase letters, while ignoring non-alphabet characters.
  
### How it works:
The Vigenère Cipher works by shifting each letter in the message based on the corresponding letter in the key. The key is repeated as many times as needed to match the length of the message. The shift is calculated by finding the position of the key letter in the alphabet, and then shifting the message letter by that amount.

For encryption, each letter is shifted forward by the position of the corresponding key letter in the alphabet. For decryption, each letter is shifted backward.

### Example:

- **Encrypted Text:** `Oabbtiz Vq Pruhdq`
- **Key:** `zambak`
- **Decrypted Text:** `this is secret`

### Getting Started

1. **Clone the repository:**

```bash
git clone https://github.com/FihriSina/vigenere-cipher.git
```

2. **Navigate to the project directory:**

```bash
cd vigenere-cipher
```

3. **Run the script:**
   - The Python script can be run as is.
   - Modify the `text` and `custom_key` variables to encrypt or decrypt different messages.

### Code Overview:

- **vigenere(message, key, direction=1)**: This function takes a message, a key, and a direction (`1` for encryption, `-1` for decryption). It processes each letter in the message and applies the Vigenère Cipher accordingly.
  
- **encrypt(message, key)**: Calls the `vigenere()` function with the direction set to `1`, returning the encrypted message.

- **decrypt(message, key)**: Calls the `vigenere()` function with the direction set to `-1`, returning the decrypted message.

### Example Code:
```python
text = 'Oabbtiz Vq Pruhdq'
custom_key = 'zambak'

decryption = decrypt(text, custom_key)
print(f'Encrypted text: {text}')
print(f'Decrypted text: {decryption}')
```

### Requirements:
- Python 3.x

### License:
This project is open-source under the MIT license. Feel free to modify and contribute!

Tabii, işte Türkçe olarak güncellenmiş `README.md` dosyası:

---

# Vigenère Şifreleme ve Çözme

Bu proje, mesajları şifrelemek ve çözmek için kullanılan klasik bir şifreleme yöntemi olan **Vigenère Şifreleme** algoritmasının uygulanmasını göstermektedir. Bu algoritma, **freeCodeCamp** üzerinde yapılan bir öğrenme projesi olarak geliştirilmiştir.

### Özellikler:
- Kendi anahtarınızı kullanarak bir mesajı **şifreleme**.
- Aynı anahtarı kullanarak bir mesajı **çözme**.
- Küçük ve büyük harflerle çalışır, harf olmayan karakterleri göz ardı eder.

### Nasıl Çalışır:
Vigenère Şifreleme, her harfi mesajdaki karşılık gelen anahtar harfine göre kaydırarak çalışır. Anahtar, mesajın uzunluğuna ulaşana kadar tekrar edilir. Anahtar harfinin alfabetedeki pozisyonu kullanılarak, mesajdaki harfe kaydırma yapılır.

Şifreleme için, her harf, karşılık gelen anahtar harfinin pozisyonu kadar ileri kaydırılır. Çözme işlemi ise, her harfi anahtar harfinin pozisyonu kadar geri kaydırır.

### Örnek:

- **Şifreli Metin:** `Oabbtiz Vq Pruhdq`
- **Anahtar:** `zambak`
- **Çözülmüş Metin:** `this is secret`

### Başlarken

1. **Depoyu klonlayın:**

```bash
git clone https://github.com/FihriSina/vigenere-cipher.git
```

2. **Proje dizinine gidin:**

```bash
cd vigenere-cipher
```

3. **Script'i çalıştırın:**
   - Python script'i olduğu gibi çalıştırabilirsiniz.
   - Farklı mesajları şifrelemek veya çözmek için `text` ve `custom_key` değişkenlerini değiştirebilirsiniz.

### Kod Özeti:

- **vigenere(message, key, direction=1)**: Bu fonksiyon bir mesaj, bir anahtar ve bir yön (`1` şifreleme, `-1` çözme) alır. Mesajdaki her harfi işler ve Vigenère şifresini uygular.
  
- **encrypt(message, key)**: `vigenere()` fonksiyonunu `1` yönüyle çağırarak şifreli mesajı döndürür.

- **decrypt(message, key)**: `vigenere()` fonksiyonunu `-1` yönüyle çağırarak çözülmüş mesajı döndürür.

### Örnek Kod:
```python
text = 'Oabbtiz Vq Pruhdq'
custom_key = 'zambak'

decryption = decrypt(text, custom_key)
print(f'Encrypted text: {text}')
print(f'Decrypted text: {decryption}')
```

### Gereksinimler:
- Python 3.x

### Lisans:
Bu proje MIT lisansı altında açık kaynaklıdır. Değiştirebilir ve katkıda bulunabilirsiniz!

---
