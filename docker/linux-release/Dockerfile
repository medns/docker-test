FROM debian

ENV PATH="/opt/depot_tools:${PATH}"

RUN \
apt-get update && apt-get -y install curl git git-lfs libc6-i386 lib32atomic1 lib32stdc++6 && apt-get clean && \
git clone https://chromium.googlesource.com/chromium/tools/depot_tools.git /opt/depot_tools && gclient && \
echo 22444