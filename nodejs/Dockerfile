FROM node:lts-alpine

# Working Direct (WORKDIR)
WORKDIR /usr/app

# Copy package.json (ส่วนนี้ไม่ค่อยมีการเปลี่ยนแปลงจะดึงจาก cache ในรอบถัดไป)
COPY ./package.json .

# Run Command
RUN npm install

# Copy code from host to container
COPY . .

# Default Command
CMD [ "npm", "start" ]