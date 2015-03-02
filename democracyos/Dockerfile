FROM node:0.10

ENV GITHUB_USERNAME YourUsername
ENV GITHUB_PASSWORD YourPassword
ENV NODE_ENV production

RUN mkdir /app
WORKDIR /app
ADD ./app /app

RUN make packages
RUN npm install -g component@1.0.0
RUN component install
ENV NODE_PATH .
CMD node ./bin/dos-install && node ./bin/dos-config && node ./bin/dos-build && $

EXPOSE 3000