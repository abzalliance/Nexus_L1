# The CLI is temporarily not working.

# Nexus Prover Node Guide  

Earn **NEX Points** by contributing computational power and engaging with the **Nexus ecosystem**.  

---

## 🚀 Contribute via Web Browser  

1. **Log in** to the [Nexus Dashboard](https://app.nexus.xyz/).  
2. Click the button to start your **prover node**.  

💡 **You can run nodes on multiple devices simultaneously**, including browser tabs, desktops, laptops, and mobile phones.  
![image](https://i.postimg.cc/c1vLvyhR/Screenshot-1.png)

📌 **All devices** can be linked and managed under a single Nexus account.  
🎯 **More computations = More NEX Points**  

---

## 🖥️ Contribute via CLI  

### 1️⃣ Install Dependencies  
Run the following commands to update your system and install required packages:  

```sh
sudo apt update && sudo apt upgrade -y
sudo apt install screen curl libssl-dev pkg-config build-essential git-all protobuf-compiler -y
sudo apt update
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
```

### 2️⃣ Run Prover
Start a screen session to keep the process running in the background:
```sh
screen -S nexus
```
Install and launch the prover:
```sh
curl https://cli.nexus.xyz/ | sh
```
Manage screen session:
Minimize: `CTRL+A+D`
Reattach: `screen -r nexus`
Terminate: `screen -XS nexus quit`

Go to `/root/.nexus`, open the `prover-id` file, and insert your prover-id from Phase 1. If you did not participate in Phase 1, create a new account on the website.
Also, don't forget to log in to the website using the same email you used to participate in Phase 1.

💡 Tip: Use Mobaxterm or Termius to easily access files on your VPS.

