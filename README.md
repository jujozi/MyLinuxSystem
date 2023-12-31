# MyLinuxDesktop

Install Chrome
```bash
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
```

Install Signal
```bash
curl https://updates.signal.org/desktop/apt/keys.asc | sudo -H gpg --dearmor -o /etc/apt/keyrings/signal-desktop-archive.gpg
echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/signal-desktop-archive.gpg] https://updates.signal.org/desktop/apt xenial main" | sudo tee /etc/apt/sources.list.d/signal-desktop-xenial.list
sudo apt update && sudo apt install signal-desktop
```

https://looking-glass.io/

#Science

##Zotero
Find the extensions.zotero.findPDFs.resolvers , right click and select Modify 
{
    "name":"Sci-Hub",
    "method":"GET",
    "url":"https://sci-hub.se/{doi}",
    "mode":"html",
    "selector":"#pdf",
    "attribute":"src",
    "automatic":true
}
