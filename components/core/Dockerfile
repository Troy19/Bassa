FROM python:3

MAINTAINER SCoRe Lab Community <commuity@scorelab.org>

WORKDIR /home/Bassa

COPY setup.sh .
COPY components/core components/core

RUN apt-get update \
&& ./setup.sh \
&& python components/core/setup.py develop 

CMD [ "python", "components/core/Main.py" ]

LABEL multi.org.label-schema.name = "Bassa" \
      multi.org.label-schema.description = "Bassa provides Automated Download Queue to make the best use of Internet bandwidth" \
      multi.org.label-schema.url="https://github.com/scorelab/Bassa/wiki" \
      multi.org.label-schema.vcs-url = "https://github.com/scorelab/Bassa" \
      multi.org.label-schema.vcs-ref = "" \
      multi.org.label-schema.vendor = "Sustainable Computing Research Group" \
      multi.org.label-schema.version = "" \
      multi.org.label-schema.schema-version = "1.0"
