# https://hub.docker.com/r/adguard/adguardhome
FROM --platform=linux/arm64 adguard/adguardhome:v0.107.52@sha256:88e801c6c322f3fc4aa3747eb46c8f1be45e534840b073a55f4903de9e11e048

# hadolint ignore=DL3018
RUN apk add --no-cache yq

COPY entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

ENTRYPOINT [ "/entrypoint.sh" ]
CMD [ ]
