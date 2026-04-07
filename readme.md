# Timestamp Microservice

A freeCodeCamp backend API challenge that converts dates to Unix timestamps and UTC strings.

## Features

- `GET /api/` - Returns current time
- `GET /api/:date` - Returns Unix (ms) and UTC for valid dates
- `GET /api/1451001600000` - Handles Unix timestamp input
- Returns `{ error: "Invalid Date" }` for invalid inputs

## Tech Stack

- Node.js
- Express.js
- CORS

## Local Setup

```bash
git clone https://github.com/srg2912/timestamp_microservice.git
cd timestamp-microservice
npm install
npm start
```
Visit `http://localhost:3000`

## API Examples

| Endpoint | Response |
|----------|----------|
| `/api/` | `{"unix":...,"utc":"Tue, 07 Apr 2026..."}` |
| `/api/2015-12-25` | `{"unix":1451001600000,"utc":"Fri, 25 Dec 2015 00:00:00 GMT"}` |
| `/api/invalid` | `{"error":"Invalid Date"}` |

## License

MIT

Copyright 2026 Sergio Alfonso Omar Avalos Soria

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
