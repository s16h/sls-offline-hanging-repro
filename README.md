# Serverless Offline `POST` Request Hanging Repro

Steps to reproduce:

1. Clone repo: `git clone git@github.com:s16h/sls-offline-hanging-repro.git`
2. Go to repo: `cd sls-offline-hanging-repro`
3. Install dependencies: `npm install`
4. Run Serverless Offline: `sls offline start`
5. Send POST request: `curl -X POST http://localhost:3000/dev/test --verbose`
6. You'll see that the request hangs.

On the other hand, if you send a GET request (`curl -X GET http://localhost:3000/dev/test --verbose`), we get a response as expected.
