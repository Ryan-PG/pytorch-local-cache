# How to Store PyTorch for Installation on Environments

If you have PyTorch installed and want to store it for future use in other environments without re-downloading, follow these steps:

### Step 1: Download PyTorch Locally
Use `pip` to download the PyTorch package and any additional dependencies to a local folder:

```bash
pip download torch torchvision torchaudio -d /path/to/your/cache_directory
```

This command downloads the specified PyTorch packages into the `cache_directory`.

### Step 2: Install PyTorch from the Local Folder
To install PyTorch from the local folder in a different environment, use the following command:

```bash
pip install --find-links=/path/to/your/cache_directory torch torchvision torchaudio
```

This tells `pip` to look for the packages in the specified directory before attempting to download them from the internet.

### Benefits
- **Offline Installation**: Once stored locally, you can install PyTorch on any environment without internet access.
- **Faster Setup**: Saves time by avoiding repeated downloads.

---
By following these steps, you can efficiently store and reuse PyTorch packages for different Python environments.

