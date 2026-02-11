# Sayonara - Tony's Adventure
### Web Systems and Technologies - Laboratory 1
**Universidad del Valle de Guatemala | Semester 5, 2026**

---

## About This Laboratory

This project is the first laboratory for the Web Systems and Technologies course at Universidad del Valle de Guatemala. The goal of the lab is to build an interactive Choose Your Own Adventure (COYA) story using only HTML, and to deploy it on a local NGINX web server so it can be accessed through a browser.

A COYA is an interactive narrative format where the reader is presented with decisions at different points in the story. Each decision leads to a different path, ultimately resulting in one of several possible endings. This format was originally popularized in books during the 1980s and 1990s and has since been adapted into video games and interactive software.


## About the Story

The story follows Tony, a human with supernatural strength who travels the universe with his AI-powered ship SITA and his alien companion KAWA. After a meteor shower forces an emergency crash landing on an unmapped swamp planet, Tony must make a series of decisions that will determine his fate. At the heart of the story is the Golden Gun, a weapon forged from pure hatred that slowly corrupts whoever uses it, and Tony's unresolved grief over losing Elvira, the person he sacrificed everything to protect.

The narrative is inspired by the album Sayonara by Alvaro Diaz. The story contains three distinct endings: a good ending in which Tony finds peace and moves forward, a neutral ending in which he survives alone but carries his pain, and a bad ending in which he surrenders entirely to darkness.


## How It Works

The project is built with 11 HTML files organized across three folders. The inicio folder contains the entry point of the story. The desarrollo folder contains the intermediate scenes where the player makes decisions. The finales folder contains the three possible endings. Navigation between pages is handled exclusively through HTML anchor tags. No JavaScript or CSS was used in this project.


## How to Run It

To run this project locally you will need NGINX installed on your machine. On Mac, NGINX can be installed using Homebrew. On Windows, it is recommended to use WSL with a Debian or Ubuntu distribution.

First, clone the repository to your local machine.

```
git clone https://github.com/YOUR_USERNAME/WEB_laboratorio1.git
```

Then create the directory where NGINX will serve the files. On Mac the path is /opt/homebrew/var/www and on Linux or WSL it is /var/www/html.

```
sudo mkdir -p /opt/homebrew/var/www/adventure
```

Copy the project files into that directory.

```
sudo cp -r ~/WEB_laboratorio1/* /opt/homebrew/var/www/adventure/
```

Set the appropriate read permissions.

```
sudo chmod -R 755 /opt/homebrew/var/www/adventure
```

Start or restart NGINX.

```
brew services restart nginx
```

Finally, open your browser and navigate to the following address. The port may vary depending on your NGINX configuration.

```
http://localhost:8080/adventure/inicio/index.html
```

---

*Laboratory 1 - Web Systems and Technologies | UVG 2026*