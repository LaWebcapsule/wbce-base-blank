# wbce-base-blank
Blank service

# Integration of this service with the webcapsule CI/CD

## Dockerfile
- Add a dockerfile at the root of your project
- You may customize the Dockerfile to your requirements.
- Ensure that the service is exposed. By default, webcapsule will assume port 80 is exposed, but you can modify the port number via the webcapsule interface.

## (optional) Build script
Webcapsule checks for the presence of a package.json file.
If found, the following commands will be executed:
1. `npm install`

2. the first script encountered from the following list:
- `npm run wbce-build`
- `npm run build`
- `npm run build-front`

3. The Docker build process will then be initiated.



