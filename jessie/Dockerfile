FROM vicamo/debci-base:jessie

MAINTAINER You-Sheng Yang <vicamo@gmail.com> (@vicamo)

RUN apt-get update \
	&& apt-get install -y --no-install-recommends \
		apt-cacher-ng \
		schroot \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*_dists_*
