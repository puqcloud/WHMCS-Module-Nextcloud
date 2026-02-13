# WHMCS setup (install/update)

### Nextcloud module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-nextcloud.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Nextcloud/) | [FAQ](https://faq.puqcloud.com/)

## System requirements

| Requirement | Minimum version |
|-------------|-----------------|
| **PHP** | 8.2 or higher |
| **WHMCS** | 9.x or higher |
| **ionCube Loader** | v13 or newer (v14, v15) |

> **Note:** The module uses ionCube encoding. Make sure ionCube Loader is installed and active on your server.

---

## Download

The module can be ordered and downloaded from PUQ Cloud:

- **Order / Download:** [https://puqcloud.com/whmcs-module-nextcloud.php](https://puqcloud.com/whmcs-module-nextcloud.php)
- **FAQ:** [https://faq.puqcloud.com/](https://faq.puqcloud.com/)
- **Direct download link for the latest version:**

```
wget https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Nextcloud/php82/PUQ_WHMCS-Nextcloud-latest.zip
```

> Older module versions for WHMCS 8 are available in PHP-specific directories:
> - PHP 7.4: [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Nextcloud/php74/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Nextcloud/php74/)
> - PHP 8.1: [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Nextcloud/php81/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-Nextcloud/php81/)

After downloading, extract the archive:

```
unzip PUQ_WHMCS-Nextcloud-latest.zip
```

---

## Installation

### Step 1: Upload files

Extract the module archive and copy the `puqNextcloud` directory to the WHMCS servers module directory:

```
WHMCS_WEB_DIR/modules/servers/puqNextcloud
```

### Step 2: Add server

Navigate to **System Settings** → **Servers** → **Add New Server**:

1. Enter the correct **Name** and **Hostname**
2. In Server Details, select the **PUQ Nextcloud** module
3. Enter valid Nextcloud web interface credentials (username and password)
4. Click **Test connection** to verify

### Step 3: Create product

Navigate to **System Settings** → **Products/Services** → **Create a New Product**:

1. Select the **PUQ Nextcloud** module in the Module settings section
2. Configure the product parameters

---

## Update

### Step 1: Backup

Before updating, it is recommended to back up:
- WHMCS database
- Module files in `modules/servers/puqNextcloud/`

### Step 2: Upload new files

Download and extract the new version, then overwrite all files in:

```
WHMCS_WEB_DIR/modules/servers/puqNextcloud/
```

### Step 3: Verification

1. Log in to the WHMCS admin panel
2. Check the module is functioning correctly
3. Verify product settings

> **Important (v3.0):** Product reconfiguration is required after updating to version 3.0.
