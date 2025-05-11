# lungoo Personal Arch Repository

This is a custom Arch Linux repository containing personal and patched packages.

## Repository URL

    https://repo.lungoo.de/x86_64

## How to Add This Repository

1. **Import the GPG Key**

   Run the following command to import and locally sign my GPG key:

   ```sh
   sudo pacman-key --recv-keys B54DD65336CCFAA7
   sudo pacman-key --lsign-key B54DD65336CCFAA7
   ```

2. **Add the Repository to Your pacman.conf**

   Edit `/etc/pacman.conf` and add the following lines at the end:

   ```ini
   [lungoo]
   Server = https://repo.lungoo.de/x86_64
   ```

3. **Update and Install Packages**

   ```sh
   sudo pacman -Sy
   sudo pacman -S <package-name>
   ```

Replace `<package-name>` with the desired package from this repository.

---

**Note:** This repository is personal and may contain packages not suitable for production use. Use at your own risk.