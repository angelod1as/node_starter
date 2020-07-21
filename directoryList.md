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
