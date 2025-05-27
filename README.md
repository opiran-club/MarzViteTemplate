Forked version for personal use

for a better result go to the source page and install from this link

[Matin Dehghani](https://github.com/MatinDehghanian/MarzViteTemplate)

---


## Installation Steps

### For Marzban

1. **Download the Template File:**
   ```sh
   sudo wget -N -P /var/lib/marzban/templates/subscription/ https://github.com/MatinDehghanian/MarzViteTemplate/releases/download/v.1.1/index.html
   ```

2. **Execute the Following Commands in Your Server Terminal:**
   ```sh
   echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
   echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
   ```
   Or uncomment the following lines in the `.env` file located in `/opt/marzban` by removing the `#` at the beginning:
   ```sh
   CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
   SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
   ```

3. **Restart Marzban:**
   ```sh
   marzban restart
   ```
