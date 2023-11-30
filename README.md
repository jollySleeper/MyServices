# ⚙️ MyServices

Welcome to the repository of my systemd services!
This repository contains a collection of systemd service files designed to run various scripts for automating tasks and managing services on your system.

## 📖 Table of Contents

- [✨ Features](#features)
- [🚀 Installation](#installation)
- [🛠️ Usage](#usage)
- [🗑️ Uninstall](#uninstall)
- [🐛 Bugs or Requests](#bugs-or-requests)
- [🤝 Contributing](#contributing)
- [📄 License](#license)
- [🙏 Acknowledgments](#acknowledgments)

## ✨ Features

Features provided by each service are as follows:
- **EvRemap**: Service for running custom keybinds on boot.
- **SleepFixer**: Service & Timer file for fixing your sleep.
- **ThemeChanger**: Service & Timer file for changing theme based on time.

## 🚀 Installation

- Clone this repo using:
```sh
git clone http://github.com/jollySleeper/MyServices.git ~/services && cd ~/services
```

- Install a specific service by running the following commands:
```sh
mkdir -p ~/.config/systemd/user/ 
cp <service_name>.service ~/.config/systemd/user/.
systemctl --user enable <service_name>.service
```

- If the service also has a timer file, additionally run:
```sh
systemctl --user enable <service_name>.timer
```

- To install all the services & timers repeat the last two steps.

## 🛠️ Usage

- To run the service after installation, use the following commands:
```sh
systemctl --user start <service_name>.service
```

## 🗑️ Uninstall

If you decide to uninstall, we're sorry to hear that the settings didn't meet your expectations. We appreciate your feedback. 

- For uninstalling a service, run the following commands:
```sh
systemctl --user stop <service_name>.service
systemctl --user disable <service_name>.service
```

- If the service also had a timer file, run the following commands:
```sh
systemctl --user stop <service_name>.timer
systemctl --user disable <service_name>.timer
```

- Delete the cloned folder using `rm -r services` command.

## 🐛 Bugs or Requests

**Please help me improve these scripts.** If you encounter any problem(s) feel free to open an [issue](https://github.com/jollySleeper/MyServices/issues/new).
If you feel the project is missing a feature, please raise an [issue](https://github.com/jollySleeper/MyServices/issues/new) with `FeatureRequest` as the heading.

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/jollySleeper/MyServices/blob/main/LICENSE) file for details.

## 🙏 Acknowledgments

- Thanks to the internet for helping me with services & timers.
