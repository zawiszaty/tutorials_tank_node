# Node.js Dockerfile for Tutorials Tank
[![Build Status](https://travis-ci.com/zawiszaty/tutorials_tank_node.svg?branch=master)](https://travis-ci.com/zawiszaty/tutorials_tank_node)

### How to use it with docker-compose
```bash
  frontend:
    image: zawiszaty/tutorials_tank_node:latest
    expose:
      - 80
    ports:
      - 80:3000
    volumes:
      - ./web-app:/usr/src/app
    command: ['npm','start']
```
### But you must add this line to your package.json in scrpits
```bash
"start": "npm install; react-scripts start",
```
