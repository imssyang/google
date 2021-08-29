# Chrome

```
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
cp google-chrome-stable_current_amd64.deb /opt/google/archive/source

apt install fonts-liberation
apt install ./google-chrome-stable_current_amd64.deb
apt purge google-chrome-stable

vim /opt/google/archive/source/google-chrome  修改启动脚本以支持root用户运行
    exec -a "$0" "$HERE/chrome" "$@" --user-data-dir --test-type --no-sandbox
```

# Chromium开发工具
[Chromium depot tools](git clone https://chromium.googlesource.com/chromium/tools/depot_tools.git)


