# HASITHA
HASITHA  MD

me  you tube 👇 සප්පරක්  දාන්න 

https://youtube.com/@user-md-hasitha?si=HmRs8KoTnEV3Px9x

ASITHA. MD.v3  සිසන්  ID link
👇
https://pair-production-68b5.up.railway.app

___________________________________________

Node.js. file. 👇







    name: Node.js CI

    on:
    push:
    branches:
      - main
    pull_request:
    branches:
      - main

    jobs:
    build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: npm install

    - name: Start application
      run: npm start
