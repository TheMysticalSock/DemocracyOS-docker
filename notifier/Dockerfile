FROM node:0.10

ENV GITHUB_USERNAME YourUsername
ENV GITHUB_PASSWORD YourPassword
ENV NODE_ENV production
ENV PORT 9001
ENV MONGO_URL mongodb://mongo/DemocracyOS-prod
ENV ACCESS_TOKEN YourToken
ENV MANDRILL_TOKEN YourToken
ENV MANDRILL_FROM_EMAIL some@email.com
ENV MANDRILL_FROM_NAME FromName
ENV LOCALE en

RUN mkdir /app
WORKDIR /app
ADD ./app /app

ENV NODE_PATH .

CMD make

EXPOSE 9001