FROM node:16-alpine

# Create the directory!
RUN mkdir -p /usr/src/bot
WORKDIR /usr/src/bot

# Copy and Install our bot
COPY package.json /usr/src/bot
RUN npm install

## following 3 lines are for installing ffmepg
# RUN apk update
# RUN apk add
# RUN apk add ffmpeg

# Our precious bot
COPY . /usr/src/bot

# Start me!
CMD ["npm", "start"]