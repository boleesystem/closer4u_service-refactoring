1. npm 설치
npm init -y
npm i bcrypt cookie-parser dotenv ejs express jsonwebtoken mysql2 sequelize
npm i jest nodemon prettier sequelize-cli supertest -save-dev

2. package.json 설정 - nodemon, jest(테스트코드)
"start": "nodemon app.js",
    "test:unit": "jest __test__/unit/* --forceExit",
    "test:unit:silent": "jest __test__/unit/* --silent --forceExit",
    "test:unit:coverage": "jest __test__/unit/* --coverage --forceExit",
    "test:integration": "jest __test__/integration --forceExit",
    "test:integration:coverage": "jest __test__/integration --coverage --forceExit"

3. 서버 켜기
1) server.js에서 const app = require('../app.js');로 루트 폴더의 app.js에서 불러옴# closer4u_service-socketio-refactoring
