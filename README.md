# Node Starter

A Node server folder structure.

## Folder structure

(File tree generated by [mddir](https://www.npmjs.com/package/mddir))

```
|-- personal
    |-- .DS_Store
    |-- .env
    |-- .env.example
    |-- .eslintignore
    |-- .eslintrc.json
    |-- .gitignore
    |-- README.md
    |-- babel.config.js
    |-- directoryList.md
    |-- jest.config.js
    |-- mddir.js
    |-- ormconfig.example.json
    |-- ormconfig.json
    |-- package.json
    |-- prettier.config.js
    |-- tsconfig.json
    |-- yarn.lock
    |-- src
    |   |-- @types
    |   |   |-- express.d.ts
    |   |-- config
    |   |   |-- auth.ts
    |   |   |-- cache.ts
    |   |   |-- mail.ts
    |   |   |-- upload.ts
    |   |-- modules
    |   |   |-- users
    |   |       |-- dtos
    |   |       |   |-- ICreateUserDTO.ts
    |   |       |   |-- IFindAllProvidersDTO.ts
    |   |       |-- infra
    |   |       |   |-- http
    |   |       |   |   |-- controllers
    |   |       |   |   |   |-- ForgotPasswordController.ts
    |   |       |   |   |   |-- ProfileController.ts
    |   |       |   |   |   |-- ResetPasswordController.ts
    |   |       |   |   |   |-- SessionsControllers.ts
    |   |       |   |   |   |-- UserAvatarController.ts
    |   |       |   |   |   |-- UsersControllers.ts
    |   |       |   |   |-- middlewares
    |   |       |   |   |   |-- ensureAuthenticated.ts
    |   |       |   |   |-- routes
    |   |       |   |       |-- password.routes.ts
    |   |       |   |       |-- profile.routes.ts
    |   |       |   |       |-- sessions.routes.ts
    |   |       |   |       |-- users.routes.ts
    |   |       |   |-- typeorm
    |   |       |       |-- entities
    |   |       |       |   |-- User.ts
    |   |       |       |   |-- UserToken.ts
    |   |       |       |-- repositories
    |   |       |           |-- UserTokensRepository.ts
    |   |       |           |-- UsersRepository.ts
    |   |       |-- providers
    |   |       |   |-- index.ts
    |   |       |   |-- HashProvider
    |   |       |       |-- fakes
    |   |       |       |   |-- FakeHashProvider.ts
    |   |       |       |-- implementations
    |   |       |       |   |-- BCryptHashProvider.ts
    |   |       |       |-- models
    |   |       |           |-- IHashProvider.ts
    |   |       |-- repositories
    |   |       |   |-- IUserTokensRepository.ts
    |   |       |   |-- IUsersRepository.ts
    |   |       |   |-- fakes
    |   |       |       |-- FakeUserTokensRepository.ts
    |   |       |       |-- FakeUsersRepository.ts
    |   |       |-- services
    |   |       |   |-- AuthenticateUserService.spec.ts
    |   |       |   |-- AuthenticateUserService.ts
    |   |       |   |-- CreateUserService.spec.ts
    |   |       |   |-- CreateUserService.ts
    |   |       |   |-- ResetPasswordService.spec.ts
    |   |       |   |-- ResetPasswordService.ts
    |   |       |   |-- SendForgotPasswordEmailService.spec.ts
    |   |       |   |-- SendForgotPasswordEmailService.ts
    |   |       |   |-- ShowProfileService.spec.ts
    |   |       |   |-- ShowProfileService.ts
    |   |       |   |-- UpdateProfileService.spec.ts
    |   |       |   |-- UpdateProfileService.ts
    |   |       |   |-- UpdateUserAvatarService.spec.ts
    |   |       |   |-- UpdateUserAvatarService.ts
    |   |       |-- views
    |   |           |-- forgot_password.hbs
    |   |-- shared
    |       |-- container
    |       |   |-- index.ts
    |       |   |-- providers
    |       |       |-- index.ts
    |       |       |-- CacheProvider
    |       |       |   |-- index.ts
    |       |       |   |-- dtos
    |       |       |   |-- fakes
    |       |       |   |   |-- FakeCacheProvider.ts
    |       |       |   |-- implementations
    |       |       |   |   |-- RedisCacheProvider.ts
    |       |       |   |-- models
    |       |       |       |-- ICacheProvider.ts
    |       |       |-- MailProvider
    |       |       |   |-- index.ts
    |       |       |   |-- dtos
    |       |       |   |   |-- ISendMailDTO.ts
    |       |       |   |-- fakes
    |       |       |   |   |-- FakeMailProvider.ts
    |       |       |   |-- implementations
    |       |       |   |   |-- EtherealMailProvider.ts
    |       |       |   |   |-- SESMailProvider.ts
    |       |       |   |-- models
    |       |       |       |-- IMailProvider.ts
    |       |       |-- MailTemplateProvider
    |       |       |   |-- index.ts
    |       |       |   |-- dtos
    |       |       |   |   |-- IParseMailTemplateDTO.ts
    |       |       |   |-- fakes
    |       |       |   |   |-- FakeMailTemplateProvider.ts
    |       |       |   |-- implementations
    |       |       |   |   |-- HandlebarsMailTemplateProvider.ts
    |       |       |   |-- models
    |       |       |       |-- IMailTemplateProviders.ts
    |       |       |-- StorageProvider
    |       |           |-- index.ts
    |       |           |-- fakes
    |       |           |   |-- FakeStorageProvider.ts
    |       |           |-- implementations
    |       |           |   |-- DiskStorageProvider.ts
    |       |           |   |-- S3StorageProvider.ts
    |       |           |-- models
    |       |               |-- IStorageProvider.ts
    |       |-- errors
    |       |   |-- AppError.ts
    |       |-- infra
    |           |-- http
    |           |   |-- server.ts
    |           |   |-- middlewares
    |           |   |   |-- RateLimiter.ts
    |           |   |-- routes
    |           |       |-- index.ts
    |           |-- typeorm
    |               |-- index.ts
    |               |-- migrations
    |                   |-- .gitkeep
    |                   |-- 1586866908707-CreateAppointments.ts
    |                   |-- 1586876010061-CreateUsers.ts
    |                   |-- 1586877157192-AlterProviderFieldToProviderId.ts
    |                   |-- 1587126753091-AddAvatarFieldToUsers.ts
    |                   |-- 1589050488229-CreateUserTokens.ts
    |                   |-- 1589288323532-AddUserIdAppointments.ts
    |-- tmp
        |-- .gitkeep
        |-- uploads
            |-- .gitkeep
```

See detailed information below.

The list is ordered by folder complexity: from least complex to "absolute mess".

- **📁 tmp/**

  **Do not delete the temp folder**. It's used by upload services. It doesn't have `.gitkeep` files by mistake.

  You can delete files commited by mistake but not the folders inside it.

- **📁 src/**

  Where all code is located

  - **📁 @types/**

    Custom types for typescript. Name template: `_filename_.d.ts` (the `d` stands for `definition`).

  - **📁 config/**

      Add here default configuration for the whole project. All of the files are filled through `.env`.

    - **✏️ auth.ts**

      JWT secret and expiration date

    - **✏️ cache.ts**

      Cache configuration. In this file, Redis (but I might change)

    - **✏️ mail.ts**

      E-mail provider configuration, defauts to Ethereal.

    - **✏️ upload.ts**

      Configs upload folder with `multer` and AWS bucket

  - **📁 shared/**

    Files shared by whole project, without specific use or componentization.

    - **📁 infra/**

      These files open the server to the web. They're about infrastructure, like server:database communication (using `typeorm`) and routes & middlewares. It's here that the main `server.ts` file is located.

      - **📁 typeorm/**

        - **✏️ index.ts**

          Only opens connections with `typeorm`. Feeds on `ormconfig.json` from `root`.

        - **📁 migrations/**

          Every new change in database should be made using migrations to keep database integrity.

          To create a new migration, run `yarn typeorm migration:create -n name`, then edit file created inside this folder. The `name` has to be TitleCase and __very__ descriptive. Eg: `ChangeProviderFieldToProviderId`

          To run migrations and consolidate in server, run `yarn typeorm migration:run`

          To revert a migration, `yarn typeorm migration:revert`

    - **📁 errors/**

      - **✏️ AppError.ts**

        Handles errors through application instead of native JS error handler, making possible better error description.

    - **📁 container/**

      - **✏️ index.ts**

        Connects providers repositories with ORM using `tsyringe`.

      - **📁 providers/**

        Contains folders for providers. Important: the folders must be generic and not specific for service. Eg: instead of `Gmail Provider`, write a "Mail Provider` folder with the specific implementation (see below)

        - **✏️ index.ts**

          A simple file importing the providers.
      
        - **📁 <i>ServiceName</i>Provider/**

          This folder contains all information of the provider. This is an example for a fake service. For actual folders in this project, see next section.

          - **📁 dtos/**

            - **🛠 I<i>DoSomething</i>DTO.ts**

              Stores typescript Data Transfer Objects.

          - **📁 fakes/**

            - **🧪 Fake<i>ServiceName</i>Provider.ts**

              A copy of the provider with fake data for testing. Can't rely on other components (as testing good practices)

          - **📁 implementations/**

              Stores all possible implementations of provider. Eg: `EtherealMail` and `SES`, or `Disk Storage` vs `S3`. Useful when changing provider or while developing locally.

              - **✏️ <i>ImplementationName</i>Provider.ts**

                Interacts with database (CRUD or other)

          - **📁 models/**

            - **🛠 I<i>ModelName</i>Provider.ts**

              Store models and schemas for provider usage

          - **✏️ index.ts**

            Imports and connects providers with `tsyringe`

  - **📁 modules/**

    Here are the folders/files os specific relationships with the database. Repositories and Services should talk to the *📁 Providers* in *📁 Shared* folder.

    - **📁 _ModuleName_**

      The folder should have the associated module as its name. Eg: `users`, `notifications` or `appointments`.

      - **📁 dtos**

        - **🛠 I<i>DoSomething</i>DTO.ts**

          Stores typescript Data Transfer Objects.

      - **📁 infra**

          Files related to module infrastructure

        - **📁 http**

          Code accessible by external sources, like API calls.

          - **📁 controllers**

            Controllers that interact with services.

            - **✏️ <i>ControllerName</i>Controller.ts**

              Each file has a class with limited functions. They never manipulate database directly, just call the associated services.

          - **📁 middlewares**

            Express middlewares for this specific module.

            - **✏️ <i>MiddlewareName</i>.ts**

              File that interacts with Express as a middleware, eg: ensureAuthenticate.ts

          - **📁 routes**

            Exposes routes to HTTP.

              - **✈️ <i>filename</i>.routes.ts**

                Uses Express to expose routes and work with middlewares.

        - **📁 typeorm**

          Stores files that interact with database
          
          - **📁 entities**

            These files are schemas or models using TypeScript @descriptors.

            - **✏️ <i>Filename</i>.ts**

          - **📁 repositories**

            Stores repositories that execute database queries and actions

            - **✏️ <i>FileName</i>Repository.ts**

              Find, create, update and delete from database
      
      - **📁 providers**

        Specific module providers

        - **📁 providers/**

          Different from the aforementioned `provider` folder, this one interacts directly with the module and needs it's existance to survive.

          - **✏️ index.ts**

            Imports and connects providers with `tsyringe`
        
          - **📁 <i>ServiceName</i>Provider/**

            Contains all information of the provider.

            - **📁 dtos/**

              - **🛠 I<i>DoSomething</i>DTO.ts**

                Stores typescript Data Transfer Objects.

            - **📁 fakes/**

              - **🧪 Fake<i>ServiceName</i>Provider.ts**

                A copy of the provider with fake data for testing. Can't rely on other components (as testing good practices)

            - **📁 implementations/**

                Stores all possible implementations of provider. Eg: `BCryptHashProvider`.

                - **✏️ <i>ImplementationName</i>Provider.ts**

                  Interacts with database or service

            - **📁 models/**

              - **🛠 I<i>ModelName</i>Provider.ts**

                Store models and schemas for provider usage
      
      - **📁 repositories**
        
        Stores fake and repository interface

        - **📁 fakes**

          Has fake repository for testing

          - **🧪 Fake<i>FileName</i>Repository.ts**

            Find, create, update and delete from local array, for testing purposes.

        - **🛠 I<i>FileName</i>Repository.ts**

          Repository interface, typing all it's properties.

      - **📁 services**

        Stores services used by repositories, following Single Responsability Principle. Every file **has** to have it's test counterpart.

        - **✏️ <i>FileName</i>Service.ts**

          Has single property: `execute()`. It interacts with the request, formats and parses data, then responses accordingly.

        - **🧪 <i>FileName</i>Service.spec.ts**

          Tests service functionality using `jest`. Uses fake repositories and providers.
      
      - **📁 views**

        Stores possible views for module, like the handlebars file below for email-templating.

        - **✏️ <i>file_name</i>.hbs**

          Example file. This one is a handlebars file that serves as a template for the Mail service.

## Implementations

In this template, there are a few pre-made implementations.

- A Redis-based cache provider
- Two e-mail providers: Ethereal (development) and Amazon SES
- A e-mail template provider using handlebars
- Two storage providers: disk (dev and temporary storage) and Amazon S3

You can add/remove any of them knowing that you'll need to change other files, mainly those that connect the providers with the rest of the server... but that's easy if your IDE shows those kinds of "missing file" errors.

## Modules

In this template, there is a `user` module already implemented with the following services:

- Authenticate user (via JWT)
- Create user
- Reset password
- Send "forgot password" e-mail
- Show profile
- Update profile
- Update user avatar

## Root files walkthrough

- .gitignore: Ignores files and folders from git
- .env: It's imperative to have a `.env` file following `.env.example`. Fill the missing information before running server.
- .eslintignore: Ignores files and folders from eslint
- .eslintrc.json: Eslint configuration file
- babel.config.js: Babel configuration file
- jest.config.js: Jest configuration file
- ormconfig.json: Server Usage configuration file. Follow `ormconfig.example.json`.
- prettier.config.js: Prettier configuration file
- tsconfig.json: Typescript configuration file
- package.json: see below

## Package.json walkthrough

### Scripts

- `build`: parses typescript into `dist` folder
- `dev:server`: development server
- `start`: runs server
- `test`: runs `jest` tests
- `typeorm`: runs `typeorm` commands, like creating and running migrations

### Dependencies

- dotenv: loads `.env` files
- express: makes all the server _magic_ happen
- express-async-errors: async/await in express
- rate-limiter-flexible: protects the server from DDoS and brute force
- typeorm: ORM (object-relational mapping): language agnostic server communication
- uuidv4: generates unique ids

### Dev Dependencies

#### Babel & Typescript

- typescript: types!
- @babel/cli, core, env & node: Needed package for Babel transpile.
- @babel/preset-typescript: Preset for typescript usage
- @babel/plugin-proposal-class-decorators: Allows Typescript @decorators
- babel-plugin-transform-typescript-metadata: usage with decorators
- @babel/plugin-proposal-class-properties: Transforms static class properties as well as properties declared with the property initializer syntax. [Source](https://www.npmjs.com/package/@babel/plugin-proposal-class-properties)
- babel-plugin-module-resolver: best pathing, see [source](https://github.com/tleunen/babel-plugin-module-resolver)


#### Eslint

All below: configuration for `eslint` and `typescript`, using `airbnb` as base.

- eslint
- eslint-config-airbnb-base
- eslint-plugin-import
- eslint-import-resolver-typescript
- @typescript-eslint/eslint-plugin
- @typescript-eslint/parser

Working alongside `eslint` is `prettier`:

- prettier
- eslint-plugin-prettier
- eslint-config-prettier

#### Others

- jest: testing tool
- ts-jest: `jest` with `typescript`
- ts-node-dev: like `nodemon` but for `typescript` and `node`
- tsconfig-paths: best pathing (`paths` in `tsconfig`), eg `@module/file.ts` instead of `src/path/to/file/file.ts`

## SOLID

I've built this based on code from code [Rocketseat](https://rocketseat.com.br/) bootcamp. I try the most to follow the [SOLID](https://khalilstemmler.com/articles/solid-principles/solid-typescript/) principles.

