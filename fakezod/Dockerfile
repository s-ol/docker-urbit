FROM paulbellamy/urbit

RUN git init /arvo \
  && cd /arvo \
  && git remote add origin https://github.com/urbit/arvo \
  && git fetch origin maint-20160818 \
  && git checkout -b stable origin/maint-20160818

ENTRYPOINT ["urbit", "-F", "-I", "zod"]
