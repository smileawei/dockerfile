FROM alpine

ENV password=passwd \
    prot=8888 \
    version=v20180601

RUN wget  -P /usr/bin https://github.com/txthinking/brook/releases/download/${version}/brook && \
chmod +x /usr/bin/brook

EXPOSE ${prot}
CMD /usr/bin/brook server -l :${prot} -p ${password}
