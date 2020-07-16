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
    |-- test
    |   |-- test1
    |-- tmp
        |-- .gitkeep
        |-- uploads
            |-- .gitkeep
