<!-- THIS FILE IS GENERATED VIA '.template-helpers/generate-tag-details.pl' -->

# Tags of `ghost`

-	[`ghost:0.7.2`](#ghost072)
-	[`ghost:0.7`](#ghost07)
-	[`ghost:0`](#ghost0)
-	[`ghost:latest`](#ghostlatest)

## `ghost:0.7.2`

```console
$ docker pull library/ghost@sha256:4f8f2cc82f817e973faede32f717eeae9f6f7b4fcb44b69e7c4b1fccfbd9c5f5
```

-	Total Virtual Size: 356.9 MB (356915916 bytes)
-	Total v2 Content-Length: 106.8 MB (106845695 bytes)

### Layers (23)

#### `6d1ae97ee388924068b7a4797d995d57d1e6194843e7e2178e592a880bf6c7ad`

```dockerfile
ADD file:863d6edd178364362a93f49103aa75c1bd03a37e83bfe0b051a3881c9333d238 in /
```

-	Created: Fri, 04 Dec 2015 19:27:57 GMT
-	Docker Version: 1.8.3
-	Virtual Size: 125.1 MB (125115267 bytes)
-	v2 Blob: `sha256:d4bce7fd68df2e8bb04e317e7cb7899e981159a4da89339e38c8bf30e6c318f0`
-	v2 Content-Length: 51.4 MB (51354256 bytes)
-	v2 Last-Modified: Fri, 04 Dec 2015 19:45:49 GMT

#### `8b9a99209d5c8f3fc5b4c01573f0508d1ddaa01c4f83c587e03b67497566aab9`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Fri, 04 Dec 2015 19:28:00 GMT
-	Parent Layer: `6d1ae97ee388924068b7a4797d995d57d1e6194843e7e2178e592a880bf6c7ad`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `2e05a52ffd47e52854ef8b2d0989e08d41301926baf7b3aeb8d5c370e0b11566`

```dockerfile
RUN apt-get update && apt-get install -y --no-install-recommends \
		ca-certificates \
		curl \
		wget \
	&& rm -rf /var/lib/apt/lists/*
```

-	Created: Fri, 04 Dec 2015 19:32:32 GMT
-	Parent Layer: `8b9a99209d5c8f3fc5b4c01573f0508d1ddaa01c4f83c587e03b67497566aab9`
-	Docker Version: 1.8.3
-	Virtual Size: 44.3 MB (44293503 bytes)
-	v2 Blob: `sha256:816152842605fe3ede1dc7c47f33e641f74cb4ae0d5c51a6c19cc8d85da934f3`
-	v2 Content-Length: 18.5 MB (18528629 bytes)
-	v2 Last-Modified: Fri, 04 Dec 2015 19:56:45 GMT

#### `6a82f723181a4529ef74122a45c9b4706d155acf27cf59dff7e0775aaadf2fe2`

```dockerfile
RUN set -ex   && for key in\
     9554F04D7259F04124DE6B476D5A82AC7E37093B\
     94AE36675C464D64BAFA68DD7434390BDBE9B9C5\
     0034A06D9D9B0064CE8ADF6BF1747F4AD2306D93\
     FD3A5288F042B6850C66B31F09FE44734EB7990E\
     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1\
     DD8F2338BAE7501E3DD5AC78C273792F7D83545D   ; do\
     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
```

-	Created: Sat, 05 Dec 2015 19:59:03 GMT
-	Parent Layer: `2e05a52ffd47e52854ef8b2d0989e08d41301926baf7b3aeb8d5c370e0b11566`
-	Docker Version: 1.8.3
-	Virtual Size: 39.4 KB (39419 bytes)
-	v2 Blob: `sha256:f14c7fff9616a221d186260f1867ff046dcf6f2e8df81b0994b57ab42659ed6a`
-	v2 Content-Length: 19.9 KB (19855 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:54:13 GMT

#### `82179dc1bb23c4138d3e750068667642ddc6375ebee4b6327303e3d8e446ef47`

```dockerfile
ENV NPM_CONFIG_LOGLEVEL=info
```

-	Created: Sat, 05 Dec 2015 19:59:04 GMT
-	Parent Layer: `6a82f723181a4529ef74122a45c9b4706d155acf27cf59dff7e0775aaadf2fe2`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `b7fc5fc08cb963e4748fe6218f4015327deb3b90320badd289058827d24da152`

```dockerfile
ENV NODE_VERSION=4.2.3
```

-	Created: Sat, 05 Dec 2015 19:59:04 GMT
-	Parent Layer: `82179dc1bb23c4138d3e750068667642ddc6375ebee4b6327303e3d8e446ef47`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31f31f70d47ef84a32e6dbc08a1b27a4e6300ea73c9c6188cbd25be4927da9a6`

```dockerfile
RUN curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"   && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --verify SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt.asc | sha256sum -c -   && tar -xzf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1   && rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc
```

-	Created: Sat, 05 Dec 2015 19:59:08 GMT
-	Parent Layer: `b7fc5fc08cb963e4748fe6218f4015327deb3b90320badd289058827d24da152`
-	Docker Version: 1.8.3
-	Virtual Size: 35.5 MB (35484158 bytes)
-	v2 Blob: `sha256:031c9c6e663ce5109c21efcef448c141bde392845e8d9d7a932fe55606b1be72`
-	v2 Content-Length: 11.7 MB (11720692 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:54:05 GMT

#### `28f213970ef5fc7e3cc2532791ff3c62b549180fa46cc2c4b60bfc7d2831c64a`

```dockerfile
CMD ["node"]
```

-	Created: Sat, 05 Dec 2015 19:59:09 GMT
-	Parent Layer: `31f31f70d47ef84a32e6dbc08a1b27a4e6300ea73c9c6188cbd25be4927da9a6`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8cc210c96fc364b6b573cff8a99e9e38a67472d7fd344e7ee2375215aee10074`

```dockerfile
RUN groupadd user && useradd --create-home --home-dir /home/user -g user user
```

-	Created: Sun, 06 Dec 2015 00:39:38 GMT
-	Parent Layer: `28f213970ef5fc7e3cc2532791ff3c62b549180fa46cc2c4b60bfc7d2831c64a`
-	Docker Version: 1.8.3
-	Virtual Size: 335.1 KB (335105 bytes)
-	v2 Blob: `sha256:25becefe600291829afa4ad2bd3319de83604952e20a4caa0e79d0bba70d4bc4`
-	v2 Content-Length: 4.3 KB (4345 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:51 GMT

#### `e1882f2afd14a3142e42de5e3bbf4af3f708b89b8fb6a34052d8078fdc429e62`

```dockerfile
RUN set -x \
	&& apt-get update \
	&& apt-get install -y --no-install-recommends curl ca-certificates \
	&& rm -rf /var/lib/apt/lists/*
```

-	Created: Sun, 06 Dec 2015 00:40:04 GMT
-	Parent Layer: `8cc210c96fc364b6b573cff8a99e9e38a67472d7fd344e7ee2375215aee10074`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:cdb4b733578aff654928f6d598534edd52f132741bf2c1967656a81bca58cb68`
-	v2 Content-Length: 167.0 B
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:48 GMT

#### `02386dea041ad70d638f37b67aa195afd9780ca4867cb519de91bca926e23127`

```dockerfile
RUN gpg --keyserver pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4
```

-	Created: Sun, 06 Dec 2015 00:40:08 GMT
-	Parent Layer: `e1882f2afd14a3142e42de5e3bbf4af3f708b89b8fb6a34052d8078fdc429e62`
-	Docker Version: 1.8.3
-	Virtual Size: 141.7 KB (141670 bytes)
-	v2 Blob: `sha256:dbc1562da08a14fabc794ba47eb3a7f7aa335aa9ca83f12a6e04ded95fa7d4c4`
-	v2 Content-Length: 134.5 KB (134471 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:45 GMT

#### `cdb693589bee8e7feef053e37b452f245db4d3ec65749cbff820a68778093db4`

```dockerfile
RUN arch="$(dpkg --print-architecture)" \
	&& set -x \
	&& curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$arch" \
	&& curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$arch.asc" \
	&& gpg --verify /usr/local/bin/gosu.asc \
	&& rm /usr/local/bin/gosu.asc \
	&& chmod +x /usr/local/bin/gosu
```

-	Created: Sun, 06 Dec 2015 00:40:14 GMT
-	Parent Layer: `02386dea041ad70d638f37b67aa195afd9780ca4867cb519de91bca926e23127`
-	Docker Version: 1.8.3
-	Virtual Size: 2.7 MB (2698808 bytes)
-	v2 Blob: `sha256:5cd68282d1eb47c8cb66b055ceb9713b5103d95ec168a9c160a155b75d0b4957`
-	v2 Content-Length: 807.9 KB (807947 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:42 GMT

#### `6990d2324eadc05a53c7f84c92e6251d08e6253a61ca70d4b88dcbf1926ec1fa`

```dockerfile
ENV GHOST_SOURCE=/usr/src/ghost
```

-	Created: Sun, 06 Dec 2015 00:40:14 GMT
-	Parent Layer: `cdb693589bee8e7feef053e37b452f245db4d3ec65749cbff820a68778093db4`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `32fda9195a2892de33b648f1ea6cd5ffccb6ce9deb1fde9eaf590b0a10d2e682`

```dockerfile
WORKDIR /usr/src/ghost
```

-	Created: Sun, 06 Dec 2015 00:40:15 GMT
-	Parent Layer: `6990d2324eadc05a53c7f84c92e6251d08e6253a61ca70d4b88dcbf1926ec1fa`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `27f8a6a126468195c2a7727fd1634eda3db9dc7b6855f72942c04c43f8690e93`

```dockerfile
ENV GHOST_VERSION=0.7.2
```

-	Created: Sun, 06 Dec 2015 00:40:15 GMT
-	Parent Layer: `32fda9195a2892de33b648f1ea6cd5ffccb6ce9deb1fde9eaf590b0a10d2e682`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `0ab374d406c3400a5d764bcf146f8cdc00e37e48e46868968ca3abc7511893d4`

```dockerfile
RUN buildDeps=' \
		gcc \
		make \
		python \
		unzip \
	' \
	&& set -x \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -sSL "https://ghost.org/archives/ghost-${GHOST_VERSION}.zip" -o ghost.zip \
	&& unzip ghost.zip \
	&& npm install --production \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps \
	&& rm ghost.zip \
	&& npm cache clean \
	&& rm -rf /tmp/npm*
```

-	Created: Sun, 06 Dec 2015 00:41:50 GMT
-	Parent Layer: `27f8a6a126468195c2a7727fd1634eda3db9dc7b6855f72942c04c43f8690e93`
-	Docker Version: 1.8.3
-	Virtual Size: 148.8 MB (148807329 bytes)
-	v2 Blob: `sha256:a38a126b8a7d614f18a5e9a0decac5ca45d8232905881623b0c5ef24cda6717d`
-	v2 Content-Length: 24.3 MB (24274354 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:30 GMT

#### `40dfd8d7ad827cfd413ef0793540c8990e252d170c79acf6211db9cbf2b5e4d5`

```dockerfile
ENV GHOST_CONTENT=/var/lib/ghost
```

-	Created: Sun, 06 Dec 2015 00:41:54 GMT
-	Parent Layer: `0ab374d406c3400a5d764bcf146f8cdc00e37e48e46868968ca3abc7511893d4`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `ca79ad82e8f94a59bf6b48fd1ac498cd5b91d8e814d7fc08313d98dc9c8a850d`

```dockerfile
RUN mkdir -p "$GHOST_CONTENT" && chown -R user:user "$GHOST_CONTENT"
```

-	Created: Sun, 06 Dec 2015 00:41:55 GMT
-	Parent Layer: `40dfd8d7ad827cfd413ef0793540c8990e252d170c79acf6211db9cbf2b5e4d5`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a1ad5596e4b02710d44459fcb3203ecd83d52fc7fe45eea1548e8e0a8fd0390f`
-	v2 Content-Length: 139.0 B
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:03 GMT

#### `53bf636141e5146c398ee7cfb529432b26ca9726d02d67bd6122eaf2859c4626`

```dockerfile
VOLUME [/var/lib/ghost]
```

-	Created: Sun, 06 Dec 2015 00:41:56 GMT
-	Parent Layer: `ca79ad82e8f94a59bf6b48fd1ac498cd5b91d8e814d7fc08313d98dc9c8a850d`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `609bccad4687b5e2dca912b7f1c0d6e6c7f0c6911506fb57dbd30b637314b1fa`

```dockerfile
COPY file:0f74adbded832aab834ad580f6cd1b5bb1e590b8e74beb16ee810e7b358eef5a in /entrypoint.sh
```

-	Created: Sun, 06 Dec 2015 00:41:56 GMT
-	Parent Layer: `53bf636141e5146c398ee7cfb529432b26ca9726d02d67bd6122eaf2859c4626`
-	Docker Version: 1.8.3
-	Virtual Size: 657.0 B
-	v2 Blob: `sha256:2915e121ee5d487dd3045eaad9309815cd6b262f6c3412e8e8e4f75917116ccc`
-	v2 Content-Length: 456.0 B
-	v2 Last-Modified: Fri, 17 Apr 2015 03:15:47 GMT

#### `3db96466aae0e17570d935f07301c8b0369617549925994bf1087a9895c18df8`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Sun, 06 Dec 2015 00:41:57 GMT
-	Parent Layer: `609bccad4687b5e2dca912b7f1c0d6e6c7f0c6911506fb57dbd30b637314b1fa`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `3089eb6bfc827fa0331660c28d7edb7923b3d93198a6072ba1d629393aaf3f63`

```dockerfile
EXPOSE 2368/tcp
```

-	Created: Sun, 06 Dec 2015 00:41:57 GMT
-	Parent Layer: `3db96466aae0e17570d935f07301c8b0369617549925994bf1087a9895c18df8`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fe87988ffe8997c987ceb51bb9e18506c4cdcaf0e3634efa45ed99e96371a443`

```dockerfile
CMD ["npm" "start"]
```

-	Created: Sun, 06 Dec 2015 00:41:58 GMT
-	Parent Layer: `3089eb6bfc827fa0331660c28d7edb7923b3d93198a6072ba1d629393aaf3f63`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `ghost:0.7`

```console
$ docker pull library/ghost@sha256:521ccafbe9d7e693b1f866ed282b9bbcdea15239b060ab65477cce6840c7e605
```

-	Total Virtual Size: 356.9 MB (356915916 bytes)
-	Total v2 Content-Length: 106.8 MB (106845695 bytes)

### Layers (23)

#### `6d1ae97ee388924068b7a4797d995d57d1e6194843e7e2178e592a880bf6c7ad`

```dockerfile
ADD file:863d6edd178364362a93f49103aa75c1bd03a37e83bfe0b051a3881c9333d238 in /
```

-	Created: Fri, 04 Dec 2015 19:27:57 GMT
-	Docker Version: 1.8.3
-	Virtual Size: 125.1 MB (125115267 bytes)
-	v2 Blob: `sha256:d4bce7fd68df2e8bb04e317e7cb7899e981159a4da89339e38c8bf30e6c318f0`
-	v2 Content-Length: 51.4 MB (51354256 bytes)
-	v2 Last-Modified: Fri, 04 Dec 2015 19:45:49 GMT

#### `8b9a99209d5c8f3fc5b4c01573f0508d1ddaa01c4f83c587e03b67497566aab9`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Fri, 04 Dec 2015 19:28:00 GMT
-	Parent Layer: `6d1ae97ee388924068b7a4797d995d57d1e6194843e7e2178e592a880bf6c7ad`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `2e05a52ffd47e52854ef8b2d0989e08d41301926baf7b3aeb8d5c370e0b11566`

```dockerfile
RUN apt-get update && apt-get install -y --no-install-recommends \
		ca-certificates \
		curl \
		wget \
	&& rm -rf /var/lib/apt/lists/*
```

-	Created: Fri, 04 Dec 2015 19:32:32 GMT
-	Parent Layer: `8b9a99209d5c8f3fc5b4c01573f0508d1ddaa01c4f83c587e03b67497566aab9`
-	Docker Version: 1.8.3
-	Virtual Size: 44.3 MB (44293503 bytes)
-	v2 Blob: `sha256:816152842605fe3ede1dc7c47f33e641f74cb4ae0d5c51a6c19cc8d85da934f3`
-	v2 Content-Length: 18.5 MB (18528629 bytes)
-	v2 Last-Modified: Fri, 04 Dec 2015 19:56:45 GMT

#### `6a82f723181a4529ef74122a45c9b4706d155acf27cf59dff7e0775aaadf2fe2`

```dockerfile
RUN set -ex   && for key in\
     9554F04D7259F04124DE6B476D5A82AC7E37093B\
     94AE36675C464D64BAFA68DD7434390BDBE9B9C5\
     0034A06D9D9B0064CE8ADF6BF1747F4AD2306D93\
     FD3A5288F042B6850C66B31F09FE44734EB7990E\
     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1\
     DD8F2338BAE7501E3DD5AC78C273792F7D83545D   ; do\
     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
```

-	Created: Sat, 05 Dec 2015 19:59:03 GMT
-	Parent Layer: `2e05a52ffd47e52854ef8b2d0989e08d41301926baf7b3aeb8d5c370e0b11566`
-	Docker Version: 1.8.3
-	Virtual Size: 39.4 KB (39419 bytes)
-	v2 Blob: `sha256:f14c7fff9616a221d186260f1867ff046dcf6f2e8df81b0994b57ab42659ed6a`
-	v2 Content-Length: 19.9 KB (19855 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:54:13 GMT

#### `82179dc1bb23c4138d3e750068667642ddc6375ebee4b6327303e3d8e446ef47`

```dockerfile
ENV NPM_CONFIG_LOGLEVEL=info
```

-	Created: Sat, 05 Dec 2015 19:59:04 GMT
-	Parent Layer: `6a82f723181a4529ef74122a45c9b4706d155acf27cf59dff7e0775aaadf2fe2`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `b7fc5fc08cb963e4748fe6218f4015327deb3b90320badd289058827d24da152`

```dockerfile
ENV NODE_VERSION=4.2.3
```

-	Created: Sat, 05 Dec 2015 19:59:04 GMT
-	Parent Layer: `82179dc1bb23c4138d3e750068667642ddc6375ebee4b6327303e3d8e446ef47`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31f31f70d47ef84a32e6dbc08a1b27a4e6300ea73c9c6188cbd25be4927da9a6`

```dockerfile
RUN curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"   && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --verify SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt.asc | sha256sum -c -   && tar -xzf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1   && rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc
```

-	Created: Sat, 05 Dec 2015 19:59:08 GMT
-	Parent Layer: `b7fc5fc08cb963e4748fe6218f4015327deb3b90320badd289058827d24da152`
-	Docker Version: 1.8.3
-	Virtual Size: 35.5 MB (35484158 bytes)
-	v2 Blob: `sha256:031c9c6e663ce5109c21efcef448c141bde392845e8d9d7a932fe55606b1be72`
-	v2 Content-Length: 11.7 MB (11720692 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:54:05 GMT

#### `28f213970ef5fc7e3cc2532791ff3c62b549180fa46cc2c4b60bfc7d2831c64a`

```dockerfile
CMD ["node"]
```

-	Created: Sat, 05 Dec 2015 19:59:09 GMT
-	Parent Layer: `31f31f70d47ef84a32e6dbc08a1b27a4e6300ea73c9c6188cbd25be4927da9a6`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8cc210c96fc364b6b573cff8a99e9e38a67472d7fd344e7ee2375215aee10074`

```dockerfile
RUN groupadd user && useradd --create-home --home-dir /home/user -g user user
```

-	Created: Sun, 06 Dec 2015 00:39:38 GMT
-	Parent Layer: `28f213970ef5fc7e3cc2532791ff3c62b549180fa46cc2c4b60bfc7d2831c64a`
-	Docker Version: 1.8.3
-	Virtual Size: 335.1 KB (335105 bytes)
-	v2 Blob: `sha256:25becefe600291829afa4ad2bd3319de83604952e20a4caa0e79d0bba70d4bc4`
-	v2 Content-Length: 4.3 KB (4345 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:51 GMT

#### `e1882f2afd14a3142e42de5e3bbf4af3f708b89b8fb6a34052d8078fdc429e62`

```dockerfile
RUN set -x \
	&& apt-get update \
	&& apt-get install -y --no-install-recommends curl ca-certificates \
	&& rm -rf /var/lib/apt/lists/*
```

-	Created: Sun, 06 Dec 2015 00:40:04 GMT
-	Parent Layer: `8cc210c96fc364b6b573cff8a99e9e38a67472d7fd344e7ee2375215aee10074`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:cdb4b733578aff654928f6d598534edd52f132741bf2c1967656a81bca58cb68`
-	v2 Content-Length: 167.0 B
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:48 GMT

#### `02386dea041ad70d638f37b67aa195afd9780ca4867cb519de91bca926e23127`

```dockerfile
RUN gpg --keyserver pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4
```

-	Created: Sun, 06 Dec 2015 00:40:08 GMT
-	Parent Layer: `e1882f2afd14a3142e42de5e3bbf4af3f708b89b8fb6a34052d8078fdc429e62`
-	Docker Version: 1.8.3
-	Virtual Size: 141.7 KB (141670 bytes)
-	v2 Blob: `sha256:dbc1562da08a14fabc794ba47eb3a7f7aa335aa9ca83f12a6e04ded95fa7d4c4`
-	v2 Content-Length: 134.5 KB (134471 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:45 GMT

#### `cdb693589bee8e7feef053e37b452f245db4d3ec65749cbff820a68778093db4`

```dockerfile
RUN arch="$(dpkg --print-architecture)" \
	&& set -x \
	&& curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$arch" \
	&& curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$arch.asc" \
	&& gpg --verify /usr/local/bin/gosu.asc \
	&& rm /usr/local/bin/gosu.asc \
	&& chmod +x /usr/local/bin/gosu
```

-	Created: Sun, 06 Dec 2015 00:40:14 GMT
-	Parent Layer: `02386dea041ad70d638f37b67aa195afd9780ca4867cb519de91bca926e23127`
-	Docker Version: 1.8.3
-	Virtual Size: 2.7 MB (2698808 bytes)
-	v2 Blob: `sha256:5cd68282d1eb47c8cb66b055ceb9713b5103d95ec168a9c160a155b75d0b4957`
-	v2 Content-Length: 807.9 KB (807947 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:42 GMT

#### `6990d2324eadc05a53c7f84c92e6251d08e6253a61ca70d4b88dcbf1926ec1fa`

```dockerfile
ENV GHOST_SOURCE=/usr/src/ghost
```

-	Created: Sun, 06 Dec 2015 00:40:14 GMT
-	Parent Layer: `cdb693589bee8e7feef053e37b452f245db4d3ec65749cbff820a68778093db4`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `32fda9195a2892de33b648f1ea6cd5ffccb6ce9deb1fde9eaf590b0a10d2e682`

```dockerfile
WORKDIR /usr/src/ghost
```

-	Created: Sun, 06 Dec 2015 00:40:15 GMT
-	Parent Layer: `6990d2324eadc05a53c7f84c92e6251d08e6253a61ca70d4b88dcbf1926ec1fa`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `27f8a6a126468195c2a7727fd1634eda3db9dc7b6855f72942c04c43f8690e93`

```dockerfile
ENV GHOST_VERSION=0.7.2
```

-	Created: Sun, 06 Dec 2015 00:40:15 GMT
-	Parent Layer: `32fda9195a2892de33b648f1ea6cd5ffccb6ce9deb1fde9eaf590b0a10d2e682`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `0ab374d406c3400a5d764bcf146f8cdc00e37e48e46868968ca3abc7511893d4`

```dockerfile
RUN buildDeps=' \
		gcc \
		make \
		python \
		unzip \
	' \
	&& set -x \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -sSL "https://ghost.org/archives/ghost-${GHOST_VERSION}.zip" -o ghost.zip \
	&& unzip ghost.zip \
	&& npm install --production \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps \
	&& rm ghost.zip \
	&& npm cache clean \
	&& rm -rf /tmp/npm*
```

-	Created: Sun, 06 Dec 2015 00:41:50 GMT
-	Parent Layer: `27f8a6a126468195c2a7727fd1634eda3db9dc7b6855f72942c04c43f8690e93`
-	Docker Version: 1.8.3
-	Virtual Size: 148.8 MB (148807329 bytes)
-	v2 Blob: `sha256:a38a126b8a7d614f18a5e9a0decac5ca45d8232905881623b0c5ef24cda6717d`
-	v2 Content-Length: 24.3 MB (24274354 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:30 GMT

#### `40dfd8d7ad827cfd413ef0793540c8990e252d170c79acf6211db9cbf2b5e4d5`

```dockerfile
ENV GHOST_CONTENT=/var/lib/ghost
```

-	Created: Sun, 06 Dec 2015 00:41:54 GMT
-	Parent Layer: `0ab374d406c3400a5d764bcf146f8cdc00e37e48e46868968ca3abc7511893d4`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `ca79ad82e8f94a59bf6b48fd1ac498cd5b91d8e814d7fc08313d98dc9c8a850d`

```dockerfile
RUN mkdir -p "$GHOST_CONTENT" && chown -R user:user "$GHOST_CONTENT"
```

-	Created: Sun, 06 Dec 2015 00:41:55 GMT
-	Parent Layer: `40dfd8d7ad827cfd413ef0793540c8990e252d170c79acf6211db9cbf2b5e4d5`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a1ad5596e4b02710d44459fcb3203ecd83d52fc7fe45eea1548e8e0a8fd0390f`
-	v2 Content-Length: 139.0 B
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:03 GMT

#### `53bf636141e5146c398ee7cfb529432b26ca9726d02d67bd6122eaf2859c4626`

```dockerfile
VOLUME [/var/lib/ghost]
```

-	Created: Sun, 06 Dec 2015 00:41:56 GMT
-	Parent Layer: `ca79ad82e8f94a59bf6b48fd1ac498cd5b91d8e814d7fc08313d98dc9c8a850d`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `609bccad4687b5e2dca912b7f1c0d6e6c7f0c6911506fb57dbd30b637314b1fa`

```dockerfile
COPY file:0f74adbded832aab834ad580f6cd1b5bb1e590b8e74beb16ee810e7b358eef5a in /entrypoint.sh
```

-	Created: Sun, 06 Dec 2015 00:41:56 GMT
-	Parent Layer: `53bf636141e5146c398ee7cfb529432b26ca9726d02d67bd6122eaf2859c4626`
-	Docker Version: 1.8.3
-	Virtual Size: 657.0 B
-	v2 Blob: `sha256:2915e121ee5d487dd3045eaad9309815cd6b262f6c3412e8e8e4f75917116ccc`
-	v2 Content-Length: 456.0 B
-	v2 Last-Modified: Fri, 17 Apr 2015 03:15:47 GMT

#### `3db96466aae0e17570d935f07301c8b0369617549925994bf1087a9895c18df8`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Sun, 06 Dec 2015 00:41:57 GMT
-	Parent Layer: `609bccad4687b5e2dca912b7f1c0d6e6c7f0c6911506fb57dbd30b637314b1fa`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `3089eb6bfc827fa0331660c28d7edb7923b3d93198a6072ba1d629393aaf3f63`

```dockerfile
EXPOSE 2368/tcp
```

-	Created: Sun, 06 Dec 2015 00:41:57 GMT
-	Parent Layer: `3db96466aae0e17570d935f07301c8b0369617549925994bf1087a9895c18df8`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fe87988ffe8997c987ceb51bb9e18506c4cdcaf0e3634efa45ed99e96371a443`

```dockerfile
CMD ["npm" "start"]
```

-	Created: Sun, 06 Dec 2015 00:41:58 GMT
-	Parent Layer: `3089eb6bfc827fa0331660c28d7edb7923b3d93198a6072ba1d629393aaf3f63`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `ghost:0`

```console
$ docker pull library/ghost@sha256:2cf8ed23e2ef5fb78785f21cc78633aac4cd97c2ccf65e798bbb0086c28e607e
```

-	Total Virtual Size: 356.9 MB (356915916 bytes)
-	Total v2 Content-Length: 106.8 MB (106845695 bytes)

### Layers (23)

#### `6d1ae97ee388924068b7a4797d995d57d1e6194843e7e2178e592a880bf6c7ad`

```dockerfile
ADD file:863d6edd178364362a93f49103aa75c1bd03a37e83bfe0b051a3881c9333d238 in /
```

-	Created: Fri, 04 Dec 2015 19:27:57 GMT
-	Docker Version: 1.8.3
-	Virtual Size: 125.1 MB (125115267 bytes)
-	v2 Blob: `sha256:d4bce7fd68df2e8bb04e317e7cb7899e981159a4da89339e38c8bf30e6c318f0`
-	v2 Content-Length: 51.4 MB (51354256 bytes)
-	v2 Last-Modified: Fri, 04 Dec 2015 19:45:49 GMT

#### `8b9a99209d5c8f3fc5b4c01573f0508d1ddaa01c4f83c587e03b67497566aab9`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Fri, 04 Dec 2015 19:28:00 GMT
-	Parent Layer: `6d1ae97ee388924068b7a4797d995d57d1e6194843e7e2178e592a880bf6c7ad`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `2e05a52ffd47e52854ef8b2d0989e08d41301926baf7b3aeb8d5c370e0b11566`

```dockerfile
RUN apt-get update && apt-get install -y --no-install-recommends \
		ca-certificates \
		curl \
		wget \
	&& rm -rf /var/lib/apt/lists/*
```

-	Created: Fri, 04 Dec 2015 19:32:32 GMT
-	Parent Layer: `8b9a99209d5c8f3fc5b4c01573f0508d1ddaa01c4f83c587e03b67497566aab9`
-	Docker Version: 1.8.3
-	Virtual Size: 44.3 MB (44293503 bytes)
-	v2 Blob: `sha256:816152842605fe3ede1dc7c47f33e641f74cb4ae0d5c51a6c19cc8d85da934f3`
-	v2 Content-Length: 18.5 MB (18528629 bytes)
-	v2 Last-Modified: Fri, 04 Dec 2015 19:56:45 GMT

#### `6a82f723181a4529ef74122a45c9b4706d155acf27cf59dff7e0775aaadf2fe2`

```dockerfile
RUN set -ex   && for key in\
     9554F04D7259F04124DE6B476D5A82AC7E37093B\
     94AE36675C464D64BAFA68DD7434390BDBE9B9C5\
     0034A06D9D9B0064CE8ADF6BF1747F4AD2306D93\
     FD3A5288F042B6850C66B31F09FE44734EB7990E\
     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1\
     DD8F2338BAE7501E3DD5AC78C273792F7D83545D   ; do\
     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
```

-	Created: Sat, 05 Dec 2015 19:59:03 GMT
-	Parent Layer: `2e05a52ffd47e52854ef8b2d0989e08d41301926baf7b3aeb8d5c370e0b11566`
-	Docker Version: 1.8.3
-	Virtual Size: 39.4 KB (39419 bytes)
-	v2 Blob: `sha256:f14c7fff9616a221d186260f1867ff046dcf6f2e8df81b0994b57ab42659ed6a`
-	v2 Content-Length: 19.9 KB (19855 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:54:13 GMT

#### `82179dc1bb23c4138d3e750068667642ddc6375ebee4b6327303e3d8e446ef47`

```dockerfile
ENV NPM_CONFIG_LOGLEVEL=info
```

-	Created: Sat, 05 Dec 2015 19:59:04 GMT
-	Parent Layer: `6a82f723181a4529ef74122a45c9b4706d155acf27cf59dff7e0775aaadf2fe2`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `b7fc5fc08cb963e4748fe6218f4015327deb3b90320badd289058827d24da152`

```dockerfile
ENV NODE_VERSION=4.2.3
```

-	Created: Sat, 05 Dec 2015 19:59:04 GMT
-	Parent Layer: `82179dc1bb23c4138d3e750068667642ddc6375ebee4b6327303e3d8e446ef47`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31f31f70d47ef84a32e6dbc08a1b27a4e6300ea73c9c6188cbd25be4927da9a6`

```dockerfile
RUN curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"   && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --verify SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt.asc | sha256sum -c -   && tar -xzf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1   && rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc
```

-	Created: Sat, 05 Dec 2015 19:59:08 GMT
-	Parent Layer: `b7fc5fc08cb963e4748fe6218f4015327deb3b90320badd289058827d24da152`
-	Docker Version: 1.8.3
-	Virtual Size: 35.5 MB (35484158 bytes)
-	v2 Blob: `sha256:031c9c6e663ce5109c21efcef448c141bde392845e8d9d7a932fe55606b1be72`
-	v2 Content-Length: 11.7 MB (11720692 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:54:05 GMT

#### `28f213970ef5fc7e3cc2532791ff3c62b549180fa46cc2c4b60bfc7d2831c64a`

```dockerfile
CMD ["node"]
```

-	Created: Sat, 05 Dec 2015 19:59:09 GMT
-	Parent Layer: `31f31f70d47ef84a32e6dbc08a1b27a4e6300ea73c9c6188cbd25be4927da9a6`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8cc210c96fc364b6b573cff8a99e9e38a67472d7fd344e7ee2375215aee10074`

```dockerfile
RUN groupadd user && useradd --create-home --home-dir /home/user -g user user
```

-	Created: Sun, 06 Dec 2015 00:39:38 GMT
-	Parent Layer: `28f213970ef5fc7e3cc2532791ff3c62b549180fa46cc2c4b60bfc7d2831c64a`
-	Docker Version: 1.8.3
-	Virtual Size: 335.1 KB (335105 bytes)
-	v2 Blob: `sha256:25becefe600291829afa4ad2bd3319de83604952e20a4caa0e79d0bba70d4bc4`
-	v2 Content-Length: 4.3 KB (4345 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:51 GMT

#### `e1882f2afd14a3142e42de5e3bbf4af3f708b89b8fb6a34052d8078fdc429e62`

```dockerfile
RUN set -x \
	&& apt-get update \
	&& apt-get install -y --no-install-recommends curl ca-certificates \
	&& rm -rf /var/lib/apt/lists/*
```

-	Created: Sun, 06 Dec 2015 00:40:04 GMT
-	Parent Layer: `8cc210c96fc364b6b573cff8a99e9e38a67472d7fd344e7ee2375215aee10074`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:cdb4b733578aff654928f6d598534edd52f132741bf2c1967656a81bca58cb68`
-	v2 Content-Length: 167.0 B
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:48 GMT

#### `02386dea041ad70d638f37b67aa195afd9780ca4867cb519de91bca926e23127`

```dockerfile
RUN gpg --keyserver pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4
```

-	Created: Sun, 06 Dec 2015 00:40:08 GMT
-	Parent Layer: `e1882f2afd14a3142e42de5e3bbf4af3f708b89b8fb6a34052d8078fdc429e62`
-	Docker Version: 1.8.3
-	Virtual Size: 141.7 KB (141670 bytes)
-	v2 Blob: `sha256:dbc1562da08a14fabc794ba47eb3a7f7aa335aa9ca83f12a6e04ded95fa7d4c4`
-	v2 Content-Length: 134.5 KB (134471 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:45 GMT

#### `cdb693589bee8e7feef053e37b452f245db4d3ec65749cbff820a68778093db4`

```dockerfile
RUN arch="$(dpkg --print-architecture)" \
	&& set -x \
	&& curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$arch" \
	&& curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$arch.asc" \
	&& gpg --verify /usr/local/bin/gosu.asc \
	&& rm /usr/local/bin/gosu.asc \
	&& chmod +x /usr/local/bin/gosu
```

-	Created: Sun, 06 Dec 2015 00:40:14 GMT
-	Parent Layer: `02386dea041ad70d638f37b67aa195afd9780ca4867cb519de91bca926e23127`
-	Docker Version: 1.8.3
-	Virtual Size: 2.7 MB (2698808 bytes)
-	v2 Blob: `sha256:5cd68282d1eb47c8cb66b055ceb9713b5103d95ec168a9c160a155b75d0b4957`
-	v2 Content-Length: 807.9 KB (807947 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:42 GMT

#### `6990d2324eadc05a53c7f84c92e6251d08e6253a61ca70d4b88dcbf1926ec1fa`

```dockerfile
ENV GHOST_SOURCE=/usr/src/ghost
```

-	Created: Sun, 06 Dec 2015 00:40:14 GMT
-	Parent Layer: `cdb693589bee8e7feef053e37b452f245db4d3ec65749cbff820a68778093db4`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `32fda9195a2892de33b648f1ea6cd5ffccb6ce9deb1fde9eaf590b0a10d2e682`

```dockerfile
WORKDIR /usr/src/ghost
```

-	Created: Sun, 06 Dec 2015 00:40:15 GMT
-	Parent Layer: `6990d2324eadc05a53c7f84c92e6251d08e6253a61ca70d4b88dcbf1926ec1fa`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `27f8a6a126468195c2a7727fd1634eda3db9dc7b6855f72942c04c43f8690e93`

```dockerfile
ENV GHOST_VERSION=0.7.2
```

-	Created: Sun, 06 Dec 2015 00:40:15 GMT
-	Parent Layer: `32fda9195a2892de33b648f1ea6cd5ffccb6ce9deb1fde9eaf590b0a10d2e682`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `0ab374d406c3400a5d764bcf146f8cdc00e37e48e46868968ca3abc7511893d4`

```dockerfile
RUN buildDeps=' \
		gcc \
		make \
		python \
		unzip \
	' \
	&& set -x \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -sSL "https://ghost.org/archives/ghost-${GHOST_VERSION}.zip" -o ghost.zip \
	&& unzip ghost.zip \
	&& npm install --production \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps \
	&& rm ghost.zip \
	&& npm cache clean \
	&& rm -rf /tmp/npm*
```

-	Created: Sun, 06 Dec 2015 00:41:50 GMT
-	Parent Layer: `27f8a6a126468195c2a7727fd1634eda3db9dc7b6855f72942c04c43f8690e93`
-	Docker Version: 1.8.3
-	Virtual Size: 148.8 MB (148807329 bytes)
-	v2 Blob: `sha256:a38a126b8a7d614f18a5e9a0decac5ca45d8232905881623b0c5ef24cda6717d`
-	v2 Content-Length: 24.3 MB (24274354 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:30 GMT

#### `40dfd8d7ad827cfd413ef0793540c8990e252d170c79acf6211db9cbf2b5e4d5`

```dockerfile
ENV GHOST_CONTENT=/var/lib/ghost
```

-	Created: Sun, 06 Dec 2015 00:41:54 GMT
-	Parent Layer: `0ab374d406c3400a5d764bcf146f8cdc00e37e48e46868968ca3abc7511893d4`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `ca79ad82e8f94a59bf6b48fd1ac498cd5b91d8e814d7fc08313d98dc9c8a850d`

```dockerfile
RUN mkdir -p "$GHOST_CONTENT" && chown -R user:user "$GHOST_CONTENT"
```

-	Created: Sun, 06 Dec 2015 00:41:55 GMT
-	Parent Layer: `40dfd8d7ad827cfd413ef0793540c8990e252d170c79acf6211db9cbf2b5e4d5`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a1ad5596e4b02710d44459fcb3203ecd83d52fc7fe45eea1548e8e0a8fd0390f`
-	v2 Content-Length: 139.0 B
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:03 GMT

#### `53bf636141e5146c398ee7cfb529432b26ca9726d02d67bd6122eaf2859c4626`

```dockerfile
VOLUME [/var/lib/ghost]
```

-	Created: Sun, 06 Dec 2015 00:41:56 GMT
-	Parent Layer: `ca79ad82e8f94a59bf6b48fd1ac498cd5b91d8e814d7fc08313d98dc9c8a850d`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `609bccad4687b5e2dca912b7f1c0d6e6c7f0c6911506fb57dbd30b637314b1fa`

```dockerfile
COPY file:0f74adbded832aab834ad580f6cd1b5bb1e590b8e74beb16ee810e7b358eef5a in /entrypoint.sh
```

-	Created: Sun, 06 Dec 2015 00:41:56 GMT
-	Parent Layer: `53bf636141e5146c398ee7cfb529432b26ca9726d02d67bd6122eaf2859c4626`
-	Docker Version: 1.8.3
-	Virtual Size: 657.0 B
-	v2 Blob: `sha256:2915e121ee5d487dd3045eaad9309815cd6b262f6c3412e8e8e4f75917116ccc`
-	v2 Content-Length: 456.0 B
-	v2 Last-Modified: Fri, 17 Apr 2015 03:15:47 GMT

#### `3db96466aae0e17570d935f07301c8b0369617549925994bf1087a9895c18df8`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Sun, 06 Dec 2015 00:41:57 GMT
-	Parent Layer: `609bccad4687b5e2dca912b7f1c0d6e6c7f0c6911506fb57dbd30b637314b1fa`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `3089eb6bfc827fa0331660c28d7edb7923b3d93198a6072ba1d629393aaf3f63`

```dockerfile
EXPOSE 2368/tcp
```

-	Created: Sun, 06 Dec 2015 00:41:57 GMT
-	Parent Layer: `3db96466aae0e17570d935f07301c8b0369617549925994bf1087a9895c18df8`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fe87988ffe8997c987ceb51bb9e18506c4cdcaf0e3634efa45ed99e96371a443`

```dockerfile
CMD ["npm" "start"]
```

-	Created: Sun, 06 Dec 2015 00:41:58 GMT
-	Parent Layer: `3089eb6bfc827fa0331660c28d7edb7923b3d93198a6072ba1d629393aaf3f63`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `ghost:latest`

```console
$ docker pull library/ghost@sha256:cc41e7bc3575eab6c6c86797e8fcaa39bca06ef469e5539ba1a6819e1a54dbcb
```

-	Total Virtual Size: 356.9 MB (356915916 bytes)
-	Total v2 Content-Length: 106.8 MB (106845695 bytes)

### Layers (23)

#### `6d1ae97ee388924068b7a4797d995d57d1e6194843e7e2178e592a880bf6c7ad`

```dockerfile
ADD file:863d6edd178364362a93f49103aa75c1bd03a37e83bfe0b051a3881c9333d238 in /
```

-	Created: Fri, 04 Dec 2015 19:27:57 GMT
-	Docker Version: 1.8.3
-	Virtual Size: 125.1 MB (125115267 bytes)
-	v2 Blob: `sha256:d4bce7fd68df2e8bb04e317e7cb7899e981159a4da89339e38c8bf30e6c318f0`
-	v2 Content-Length: 51.4 MB (51354256 bytes)
-	v2 Last-Modified: Fri, 04 Dec 2015 19:45:49 GMT

#### `8b9a99209d5c8f3fc5b4c01573f0508d1ddaa01c4f83c587e03b67497566aab9`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Fri, 04 Dec 2015 19:28:00 GMT
-	Parent Layer: `6d1ae97ee388924068b7a4797d995d57d1e6194843e7e2178e592a880bf6c7ad`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `2e05a52ffd47e52854ef8b2d0989e08d41301926baf7b3aeb8d5c370e0b11566`

```dockerfile
RUN apt-get update && apt-get install -y --no-install-recommends \
		ca-certificates \
		curl \
		wget \
	&& rm -rf /var/lib/apt/lists/*
```

-	Created: Fri, 04 Dec 2015 19:32:32 GMT
-	Parent Layer: `8b9a99209d5c8f3fc5b4c01573f0508d1ddaa01c4f83c587e03b67497566aab9`
-	Docker Version: 1.8.3
-	Virtual Size: 44.3 MB (44293503 bytes)
-	v2 Blob: `sha256:816152842605fe3ede1dc7c47f33e641f74cb4ae0d5c51a6c19cc8d85da934f3`
-	v2 Content-Length: 18.5 MB (18528629 bytes)
-	v2 Last-Modified: Fri, 04 Dec 2015 19:56:45 GMT

#### `6a82f723181a4529ef74122a45c9b4706d155acf27cf59dff7e0775aaadf2fe2`

```dockerfile
RUN set -ex   && for key in\
     9554F04D7259F04124DE6B476D5A82AC7E37093B\
     94AE36675C464D64BAFA68DD7434390BDBE9B9C5\
     0034A06D9D9B0064CE8ADF6BF1747F4AD2306D93\
     FD3A5288F042B6850C66B31F09FE44734EB7990E\
     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1\
     DD8F2338BAE7501E3DD5AC78C273792F7D83545D   ; do\
     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
```

-	Created: Sat, 05 Dec 2015 19:59:03 GMT
-	Parent Layer: `2e05a52ffd47e52854ef8b2d0989e08d41301926baf7b3aeb8d5c370e0b11566`
-	Docker Version: 1.8.3
-	Virtual Size: 39.4 KB (39419 bytes)
-	v2 Blob: `sha256:f14c7fff9616a221d186260f1867ff046dcf6f2e8df81b0994b57ab42659ed6a`
-	v2 Content-Length: 19.9 KB (19855 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:54:13 GMT

#### `82179dc1bb23c4138d3e750068667642ddc6375ebee4b6327303e3d8e446ef47`

```dockerfile
ENV NPM_CONFIG_LOGLEVEL=info
```

-	Created: Sat, 05 Dec 2015 19:59:04 GMT
-	Parent Layer: `6a82f723181a4529ef74122a45c9b4706d155acf27cf59dff7e0775aaadf2fe2`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `b7fc5fc08cb963e4748fe6218f4015327deb3b90320badd289058827d24da152`

```dockerfile
ENV NODE_VERSION=4.2.3
```

-	Created: Sat, 05 Dec 2015 19:59:04 GMT
-	Parent Layer: `82179dc1bb23c4138d3e750068667642ddc6375ebee4b6327303e3d8e446ef47`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31f31f70d47ef84a32e6dbc08a1b27a4e6300ea73c9c6188cbd25be4927da9a6`

```dockerfile
RUN curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"   && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --verify SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt.asc | sha256sum -c -   && tar -xzf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1   && rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc
```

-	Created: Sat, 05 Dec 2015 19:59:08 GMT
-	Parent Layer: `b7fc5fc08cb963e4748fe6218f4015327deb3b90320badd289058827d24da152`
-	Docker Version: 1.8.3
-	Virtual Size: 35.5 MB (35484158 bytes)
-	v2 Blob: `sha256:031c9c6e663ce5109c21efcef448c141bde392845e8d9d7a932fe55606b1be72`
-	v2 Content-Length: 11.7 MB (11720692 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:54:05 GMT

#### `28f213970ef5fc7e3cc2532791ff3c62b549180fa46cc2c4b60bfc7d2831c64a`

```dockerfile
CMD ["node"]
```

-	Created: Sat, 05 Dec 2015 19:59:09 GMT
-	Parent Layer: `31f31f70d47ef84a32e6dbc08a1b27a4e6300ea73c9c6188cbd25be4927da9a6`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8cc210c96fc364b6b573cff8a99e9e38a67472d7fd344e7ee2375215aee10074`

```dockerfile
RUN groupadd user && useradd --create-home --home-dir /home/user -g user user
```

-	Created: Sun, 06 Dec 2015 00:39:38 GMT
-	Parent Layer: `28f213970ef5fc7e3cc2532791ff3c62b549180fa46cc2c4b60bfc7d2831c64a`
-	Docker Version: 1.8.3
-	Virtual Size: 335.1 KB (335105 bytes)
-	v2 Blob: `sha256:25becefe600291829afa4ad2bd3319de83604952e20a4caa0e79d0bba70d4bc4`
-	v2 Content-Length: 4.3 KB (4345 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:51 GMT

#### `e1882f2afd14a3142e42de5e3bbf4af3f708b89b8fb6a34052d8078fdc429e62`

```dockerfile
RUN set -x \
	&& apt-get update \
	&& apt-get install -y --no-install-recommends curl ca-certificates \
	&& rm -rf /var/lib/apt/lists/*
```

-	Created: Sun, 06 Dec 2015 00:40:04 GMT
-	Parent Layer: `8cc210c96fc364b6b573cff8a99e9e38a67472d7fd344e7ee2375215aee10074`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:cdb4b733578aff654928f6d598534edd52f132741bf2c1967656a81bca58cb68`
-	v2 Content-Length: 167.0 B
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:48 GMT

#### `02386dea041ad70d638f37b67aa195afd9780ca4867cb519de91bca926e23127`

```dockerfile
RUN gpg --keyserver pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4
```

-	Created: Sun, 06 Dec 2015 00:40:08 GMT
-	Parent Layer: `e1882f2afd14a3142e42de5e3bbf4af3f708b89b8fb6a34052d8078fdc429e62`
-	Docker Version: 1.8.3
-	Virtual Size: 141.7 KB (141670 bytes)
-	v2 Blob: `sha256:dbc1562da08a14fabc794ba47eb3a7f7aa335aa9ca83f12a6e04ded95fa7d4c4`
-	v2 Content-Length: 134.5 KB (134471 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:45 GMT

#### `cdb693589bee8e7feef053e37b452f245db4d3ec65749cbff820a68778093db4`

```dockerfile
RUN arch="$(dpkg --print-architecture)" \
	&& set -x \
	&& curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$arch" \
	&& curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$arch.asc" \
	&& gpg --verify /usr/local/bin/gosu.asc \
	&& rm /usr/local/bin/gosu.asc \
	&& chmod +x /usr/local/bin/gosu
```

-	Created: Sun, 06 Dec 2015 00:40:14 GMT
-	Parent Layer: `02386dea041ad70d638f37b67aa195afd9780ca4867cb519de91bca926e23127`
-	Docker Version: 1.8.3
-	Virtual Size: 2.7 MB (2698808 bytes)
-	v2 Blob: `sha256:5cd68282d1eb47c8cb66b055ceb9713b5103d95ec168a9c160a155b75d0b4957`
-	v2 Content-Length: 807.9 KB (807947 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:42 GMT

#### `6990d2324eadc05a53c7f84c92e6251d08e6253a61ca70d4b88dcbf1926ec1fa`

```dockerfile
ENV GHOST_SOURCE=/usr/src/ghost
```

-	Created: Sun, 06 Dec 2015 00:40:14 GMT
-	Parent Layer: `cdb693589bee8e7feef053e37b452f245db4d3ec65749cbff820a68778093db4`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `32fda9195a2892de33b648f1ea6cd5ffccb6ce9deb1fde9eaf590b0a10d2e682`

```dockerfile
WORKDIR /usr/src/ghost
```

-	Created: Sun, 06 Dec 2015 00:40:15 GMT
-	Parent Layer: `6990d2324eadc05a53c7f84c92e6251d08e6253a61ca70d4b88dcbf1926ec1fa`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `27f8a6a126468195c2a7727fd1634eda3db9dc7b6855f72942c04c43f8690e93`

```dockerfile
ENV GHOST_VERSION=0.7.2
```

-	Created: Sun, 06 Dec 2015 00:40:15 GMT
-	Parent Layer: `32fda9195a2892de33b648f1ea6cd5ffccb6ce9deb1fde9eaf590b0a10d2e682`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `0ab374d406c3400a5d764bcf146f8cdc00e37e48e46868968ca3abc7511893d4`

```dockerfile
RUN buildDeps=' \
		gcc \
		make \
		python \
		unzip \
	' \
	&& set -x \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -sSL "https://ghost.org/archives/ghost-${GHOST_VERSION}.zip" -o ghost.zip \
	&& unzip ghost.zip \
	&& npm install --production \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps \
	&& rm ghost.zip \
	&& npm cache clean \
	&& rm -rf /tmp/npm*
```

-	Created: Sun, 06 Dec 2015 00:41:50 GMT
-	Parent Layer: `27f8a6a126468195c2a7727fd1634eda3db9dc7b6855f72942c04c43f8690e93`
-	Docker Version: 1.8.3
-	Virtual Size: 148.8 MB (148807329 bytes)
-	v2 Blob: `sha256:a38a126b8a7d614f18a5e9a0decac5ca45d8232905881623b0c5ef24cda6717d`
-	v2 Content-Length: 24.3 MB (24274354 bytes)
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:30 GMT

#### `40dfd8d7ad827cfd413ef0793540c8990e252d170c79acf6211db9cbf2b5e4d5`

```dockerfile
ENV GHOST_CONTENT=/var/lib/ghost
```

-	Created: Sun, 06 Dec 2015 00:41:54 GMT
-	Parent Layer: `0ab374d406c3400a5d764bcf146f8cdc00e37e48e46868968ca3abc7511893d4`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `ca79ad82e8f94a59bf6b48fd1ac498cd5b91d8e814d7fc08313d98dc9c8a850d`

```dockerfile
RUN mkdir -p "$GHOST_CONTENT" && chown -R user:user "$GHOST_CONTENT"
```

-	Created: Sun, 06 Dec 2015 00:41:55 GMT
-	Parent Layer: `40dfd8d7ad827cfd413ef0793540c8990e252d170c79acf6211db9cbf2b5e4d5`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a1ad5596e4b02710d44459fcb3203ecd83d52fc7fe45eea1548e8e0a8fd0390f`
-	v2 Content-Length: 139.0 B
-	v2 Last-Modified: Mon, 07 Dec 2015 22:53:03 GMT

#### `53bf636141e5146c398ee7cfb529432b26ca9726d02d67bd6122eaf2859c4626`

```dockerfile
VOLUME [/var/lib/ghost]
```

-	Created: Sun, 06 Dec 2015 00:41:56 GMT
-	Parent Layer: `ca79ad82e8f94a59bf6b48fd1ac498cd5b91d8e814d7fc08313d98dc9c8a850d`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `609bccad4687b5e2dca912b7f1c0d6e6c7f0c6911506fb57dbd30b637314b1fa`

```dockerfile
COPY file:0f74adbded832aab834ad580f6cd1b5bb1e590b8e74beb16ee810e7b358eef5a in /entrypoint.sh
```

-	Created: Sun, 06 Dec 2015 00:41:56 GMT
-	Parent Layer: `53bf636141e5146c398ee7cfb529432b26ca9726d02d67bd6122eaf2859c4626`
-	Docker Version: 1.8.3
-	Virtual Size: 657.0 B
-	v2 Blob: `sha256:2915e121ee5d487dd3045eaad9309815cd6b262f6c3412e8e8e4f75917116ccc`
-	v2 Content-Length: 456.0 B
-	v2 Last-Modified: Fri, 17 Apr 2015 03:15:47 GMT

#### `3db96466aae0e17570d935f07301c8b0369617549925994bf1087a9895c18df8`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Sun, 06 Dec 2015 00:41:57 GMT
-	Parent Layer: `609bccad4687b5e2dca912b7f1c0d6e6c7f0c6911506fb57dbd30b637314b1fa`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `3089eb6bfc827fa0331660c28d7edb7923b3d93198a6072ba1d629393aaf3f63`

```dockerfile
EXPOSE 2368/tcp
```

-	Created: Sun, 06 Dec 2015 00:41:57 GMT
-	Parent Layer: `3db96466aae0e17570d935f07301c8b0369617549925994bf1087a9895c18df8`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fe87988ffe8997c987ceb51bb9e18506c4cdcaf0e3634efa45ed99e96371a443`

```dockerfile
CMD ["npm" "start"]
```

-	Created: Sun, 06 Dec 2015 00:41:58 GMT
-	Parent Layer: `3089eb6bfc827fa0331660c28d7edb7923b3d93198a6072ba1d629393aaf3f63`
-	Docker Version: 1.8.3
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT
