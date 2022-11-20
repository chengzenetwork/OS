FROM        ghcr.io/parkervcp/yolks:debian

LABEL       author="Manuel Dielacher" maintainer="th3dilli@gmx.at"

LABEL       org.opencontainers.image.source="https://github.com/pterodactyl/yolks"
LABEL       org.opencontainers.image.licenses=MIT

RUN			dpkg --add-architecture i386 \
			&& apt update && apt upgrade -y \
			&& apt install -y lib32gcc-s1 lib32stdc++6 libstdc++5:i386


RUN			locale-gen zh_CN.UTF-8 \
			&& dpkg-reconfigure --frontend noninteractive locales

ENV			LANG zh_CN.UTF-8
ENV			LANGUAGE zh_CN.UTF-8
ENV			LC_ALL zh_CN.UTF-8