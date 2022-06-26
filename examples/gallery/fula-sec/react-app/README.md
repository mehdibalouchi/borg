# Gallery in react

It's a React web app that you can play with and learn:
- How Use @functionland/fula-sec, for create and importing DIDs.
- How to encrypt data and store it in Box with DID. 
- How to retrieve data and decrypt it in Client with DID.

## Installation
Clone the repository and change to project directory
```bash
cd ./examples/gallery/fula-sec/react-app
npm install
```

## Usage

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

## Deploy

To deploy this application, you need to create a production build first:
```bash
npm run build
```

The above command will create a `build` directory containing everything a web server needs to serve the application. Bring up a `nginx` web server using docker:
```bash
docker build -t web-gallery .
docker run -p 80:80 web-gallery
```

now open [http://localhost](http://localhost) to use the web gallery production version.

