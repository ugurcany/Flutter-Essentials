---
description: How to install Flutter SDK on macOS and Windows machines
---

# Installation

{% tabs %}
{% tab title="Install on macOS" %}
**Step 0:** Make sure the following tools are already installed on your device.

* Xcode
* Git

If you are on Apple Silicon Mac, you also need to install Rosetta for some ancillary tools. You can do this by running:

```bash
sudo softwareupdate --install-rosetta --agree-to-license
```

**Step 1:** Download the latest stable Flutter SDK bundle from GitHub and unzip it in your desired directory.

<pre class="language-bash"><code class="lang-bash"><strong>cd $HOME/development
</strong>git clone https://github.com/flutter/flutter.git -b stable
</code></pre>

**Step 2:** Add the following line to the `$HOME/.bash_profile` or `$HOME/.zshrc` file, depending on which shell you use.

```
export PATH="$PATH:$HOME/development/flutter/bin"
```

Now you can use `flutter` commands via terminal.

**Step 3:** Run the following command to see all dependencies are installed and ready before starting development.

```bash
flutter doctor
```

If there are missing dependencies, follow the guidelines given in the output.
{% endtab %}

{% tab title="Install on Windows" %}
**Step 0:** Make sure the following tools are already installed on your device.

* PowerShell
* Git

**Step 1:** Download the latest stable Flutter SDK bundle from GitHub and unzip it in your desired directory.

```powershell
cd C:\development
git clone https://github.com/flutter/flutter.git -b stable
```

**Step 2:** Append the following directory to your `Path` environment variable.

```
C:\development\flutter\bin
```

Now you can use `flutter` commands via console.

**Step 3:** Run the following command to see all dependencies are installed and ready before starting development.

```powershell
flutter doctor
```

If there are missing dependencies, follow the guidelines given in the output.
{% endtab %}
{% endtabs %}
