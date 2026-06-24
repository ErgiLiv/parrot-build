# parrot-build

My fixed fork of IppSec's `parrot-build`.

## Instructions

Start with a fresh Parrot OS HTB Edition VM.

Install Ansible:

```bash
python3 -m pip install --user ansible
```

Make sure Ansible is in your PATH:

```bash
export PATH="$HOME/.local/bin:$PATH"
```

Clone this repo:

```bash
git clone https://github.com/ErgiLiv/parrot-build.git
cd parrot-build
```

Install the required Ansible roles:

```bash
ansible-galaxy install -r requirements.yml
```

Run the playbook:

```bash
ansible-playbook main.yml -K
```

Enter your normal user password when asked for the `BECOME password`.

After it finishes, open a new terminal.
