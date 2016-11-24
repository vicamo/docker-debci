FROM debian:jessie

MAINTAINER You-Sheng Yang <vicamo@gmail.com> (@vicamo)

RUN apt-get update \
	&& apt-get install -y --no-install-recommends \
		debci \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*_dists_*

RUN wget -O /usr/local/bin/dumb-init \
		https://github.com/Yelp/dumb-init/releases/download/v1.2.0/dumb-init_1.2.0_amd64 \
	&& chmod +x /usr/local/bin/dumb-init

# Runs "/usr/local/bin/dumb-init -- /bin/foo"
ENTRYPOINT ["/usr/local/bin/dumb-init", "--"]
