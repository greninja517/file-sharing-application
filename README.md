# 📁 File Sharing App
File Sharing Application along with the basic Kubernetes manifests and Helm Chart.
A simple, secure web application for sharing files using unique PINs. Upload a file, get a PIN, and share it. Others can download the file using that PIN without needing an account.

---

## ✨ Features

*   ⬆️ **File Upload**: Easily upload a single file.
*   🔑 **PIN Generation**: Automatically generates a unique, secure PIN for every upload.
*   🔒 **Secure Download**: Files are only accessible with the correct PIN.
*   👤 **No Signup Required**: Quick and anonymous file sharing.

---

## 🛠️ Technologies Used

*   **Frontend**: React, Tailwind CSS
*   **Backend**: Spring Boot, Java 17
*   **Database**: MySQL
*   **File Handling**: Axios (for Multipart upload), Local File System Storage
*   **Security**: PIN-based access control
*   **Kubernetes, HELM** For Deployment Purpose
