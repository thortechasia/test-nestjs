## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation

```bash
$ yarn
```

## Running the app

```bash
# development
$ yarn start

# watch mode
$ yarn start:dev

# production mode
$ yarn start:prod
```

## Penjelesan Test

1. buatkan 1 entitas typeorm `User` dengan attribute seperti berikut

- username: string
- password: string
- telegramUser: string

2. buatkan module untuk management user (CRUD) di dalam folder `module`, yang berisi file `controller` dan `service` dengan nama yang sama dengan nama module
3. implementasikan package `nest-router` untuk membuat prefix route `api/v1`
4. buatkan library `telegram` yang di simpan di folder `lib`
5. library telegram harus mejadi wrapper dari package `telegraf.js`
6. buat event subscriber dari entity `user` untuk melisten setiap pertambahan atau perubahan data
7. setiap perubahan data di message ke ke user yang terdaftar di `telegramUser`
