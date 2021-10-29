- 👋 Hi, I’m @Sabareesvaran
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Sabareesvaran/Sabareesvaran is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->




error from chokidar angular system limit

echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p

# that modifies the file watch limit to max 524,288 which consume approx. 512MB Ram for 64bit.
# reduce that number to consume less memory.

# to see if that did it run
cat /proc/sys/fs/inotify/max_user_watches

# you should see
fs.inotify.max_user_watches=524288
