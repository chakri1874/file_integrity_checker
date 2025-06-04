# file_integrity_checker
This is a simple web tool that helps you check if a file has been tampered with or corrupted. It calculates a unique digital fingerprint (called a 'hash') of your file and lets you compare it against a known good hash to ensure its integrity.
# 🔐 File Integrity Checker (Web-Based)

This project is a simple web-based application designed to help you verify the integrity of your files using SHA-256 cryptographic hashing. It allows you to calculate a file's hash and compare it against a previously known, trusted hash to detect any unauthorized modifications or corruption.

---

## ✨ Features

* **File Hashing:** Calculate the SHA-256 hash of any file selected from your local system.
* **Integrity Verification:** Compare the calculated hash with a "stored" (manually entered) hash to determine if the file has been altered.
* **User-Friendly Interface:** A straightforward web interface for easy interaction.

---

## 🚀 How to Use

1.  **Open the application:**
    * You can access the live version of this tool via GitHub Pages: [https://chakri1874.github.io/file_integrity_checker/integrity_checker.html](https://chakri1874.github.io/file_integrity_checker/integrity_checker.html)
        *(Note: Replace `chakri1874` with your actual GitHub username and `file_integrity_checker` with your exact repository name if it's different, or remove the path if you rename `integrity_checker.html` to `index.html` for direct root access via GitHub Pages.)*
    * Alternatively, you can download the `integrity_checker.html` file and open it directly in your web browser.

2.  **Select a File:** Click the "Choose File" button and select the file you wish to check.

3.  **Calculate Hash:** Click the "Calculate Hash" button to generate the SHA-256 hash of the selected file. The calculated hash will appear in the "Calculated Hash" field.

4.  **Enter Stored Hash (for comparison):**
    * If you have a previously known and trusted hash for this file (e.g., from a software vendor's website or a previous integrity check), paste it into the "Enter a Stored Hash for Comparison" field.
    * *(Note: For the first time, you might copy the just-calculated hash to test the comparison functionality).*

5.  **Compare Hashes:** Click the "Compare Hashes" button. The application will tell you if the file is intact or if it has been modified.

---

## 💡 Why File Integrity Matters (Cybersecurity Context)

File integrity checking is a fundamental cybersecurity practice. It helps in:

* **Detecting Tampering:** Identifying if malicious actors have modified system files, software binaries, or critical documents.
* **Verifying Downloads:** Ensuring that software you download hasn't been corrupted or altered by a third party.
* **Compliance:** Meeting regulatory requirements that demand proof of data integrity.
* **Incident Response:** Determining the scope of a breach by checking which files might have been affected.

---

## 🛠️ Technologies Used

* **HTML:** For the structure of the web page.
* **CSS:** For styling and making the interface user-friendly.
* **JavaScript:** For handling file selection, performing cryptographic hashing (using the Web Cryptography API `crypto.subtle.digest`), and managing UI updates.

---

## ⚠️ Important Notes

* This is a client-side web application. It calculates hashes directly in your browser and does not send your files or their hashes to any server.
* For comparing hashes, you must manually provide the "stored" (trusted) hash. This application does not store hashes persistently across sessions or for arbitrary local files due to browser security restrictions.
* Always ensure you are comparing against a trusted, known-good hash.

---

## License

This project is open-source. Feel free to use, modify, and distribute it.
