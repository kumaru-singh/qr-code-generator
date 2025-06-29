# QR Code Generator CLI 🧭

A simple Node.js command-line application that uses [Inquirer.js](https://github.com/SBoudrias/Inquirer.js) and the `qr-code` package to generate QR codes from user input and save them as images.

---

## 🚀 Features

- Interactive CLI prompt for accepting **text or URL input**.
- Generate QR code using the [`qr-code`](https://www.npmjs.com/package/qr-code) package.
- Save the resulting QR code as a `.png` file with customizable name and dimensions.
- Minimal dependencies, quick setup.

---

## 📦 Installation

1. Clone this repo:
   ```bash
   git clone https://github.com/kumaru-singh/qr-code-generator.git
   cd qr-code-generator
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

---

## 🎯 How to Use

Run the CLI:
```bash
npm start
```

Follow these steps:

1. **Enter your text or URL** when prompted.
2. Choose/determine:
   - **Output file name** (e.g. `qr.png`)
   - **Image dimensions** (e.g. 200 for a 200×200 PNG)
   - Optional: **Error correction level** (Low / Medium / High) for greater scanning reliability.

The app will generate a PNG QR code in the project folder.

---

## ⚙️ Configuration Options

While the default flow is fully interactive, advanced users can customize the script:

- **Default file name**: change in source code.
- **Default size**: adjust the PNG dimensions (e.g. 256×256).
- **Error correction level**: `L`, `M`, `Q`, or `H`.

---

## 🧠 How It Works

1. Inquirer prompts the user for input and config options.
2. The **`qr-code`** package encodes the input into a QR code buffer.
3. The buffer is written to a `.png` file using Node's file system.

---

## 🧾 Example

```
? Enter text or URL: https://example.com
? Output file name: my-qr.png
? Image size in px: 300
? Error correction level? (choose M for typical use)
✔ Generated QR code saved to ./my-qr.png
```

---

## 📚 Inspiration & Context

QR codes (Quick Response codes) are 2D barcodes that store data as patterns of black and white squares. Created originally for the automotive industry in 1994, they are now widely used due to fast machine readability and high storage capacity.

---

## 🛠️ Dependencies

- **[inquirer](https://www.npmjs.com/package/inquirer)** – interactive CLI prompts.
- **[qr-code](https://www.npmjs.com/package/qr-code)** – QR code generation library.
- Built-in **`fs`** module to write image files.

---

## 🧪 Testing

- Run the app multiple times to generate different QR codes.
- Open the PNG in a browser or scan with your phone to verify accuracy.

---

## 📝 Contributing

Contributions are welcome! You can:
- Add support for different image formats (e.g., SVG).
- Add options to set foreground/background colors.
- Enable batch-generation from a CSV or text file.
- Improve error handling and UX.

---

## 📄 License

[MIT License](./LICENSE)

---

## 📬 Questions?

Feel free to open an **Issue** or submit a **PR**, or contact me via GitHub Discussions.

---

## 📖 References

- Wikipedia: "QR Code" and its evolution  
- [Inquirer.js](https://github.com/SBoudrias/Inquirer.js)  
- [QR Code Generator Libraries](https://github.com/topics/qrcode)
