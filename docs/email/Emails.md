---
tags: [email]
---

# Emails

Neo web services sends emails to users on various occasion and for various purposes. Some emails act as notifications or reminder, while some others are an integral part of an operation flow. This page list all the emails that can be sent to users and what type of information they should deliver to the user.

## neo-auth

### Two Factor Authentication
Sent on successful login by a user.

**Content:** Two factor authentication token

ClassName | Emitter | Test Suite |
----------|---------|------------|
`TwoFactorTokenEmail` | `TwoFactorToken@onCreation` | `TwoFactorAuthTest` 

### Password Recovery
Sent when a user asks to recover its password

**Content:** Link with token for password reset 

ClassName | Emitter | Test Suite |
----------|---------|------------|
`RecoverPasswordEmail` | `RecoveryToken@onCreation`| `PasswordLostTest`

## neo-users

### Welcome
Sent when a user is created

**Content:** Link with token for password setup

ClassName | Emitter | Test Suite |
----------|---------|------------|
`WelcomeEmail` | `User@onCreation` | `UserCreationTest`