FROM vicamo/debci:stretch

MAINTAINER You-Sheng Yang <vicamo@gmail.com> (@vicamo)

RUN apt-get update \
	&& apt-get install -y --no-install-recommends \
		apt-cacher-ng \
		debci-worker \
		schroot \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*_dists_*
