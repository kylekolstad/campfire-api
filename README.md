# Campfire API

Campfire API is a Java-based social platform backend built with Spring MVC, Hibernate, and Maven. It powers core social networking features such as user accounts, posts, likes, profile management, media uploads, password recovery, and session-based authentication.

This project was built as a full-stack backend demonstrating enterprise Java architecture, REST-style controllers, ORM persistence, cloud file storage, and real-world user interaction workflows.

---

## Features

### User Management
- Create user accounts
- Login / logout with session handling
- Lookup users by:
  - ID
  - Username
  - Email
- Update profile title, bio, and profile image
- Password reset with generated temporary passwords sent via email

### Social Features
- Create text/image posts
- Retrieve all posts
- Like posts
- Unlike posts
- Retrieve all likes

### Media Storage
- Upload profile images and post images to Amazon S3

### Security / Backend Concepts
- Password hashing
- Session-based authentication
- Cross-Origin support for frontend integration
- Layered MVC architecture

---

## Tech Stack

- Java 8
- Spring Framework 5
- Spring MVC
- Spring ORM
- Hibernate 5
- Maven
- Jackson JSON
- Log4j
- AWS S3 SDK
- JavaMail API
- Apache Commons FileUpload

---

## Project Structure

```text
src/main/java/com/campfire/

controllers/
  CF_UserController
  CF_PostController
  CF_LikeController

model/
  CF_User
  CF_Post
  CF_Like

repository/
  CF_UserRepo
  CF_PostRepo
  CF_LikeRepo

utilities/
  AWS
  EmailAPI
  GeneratePassword
  HashPassword

aspect/
  LoggingAspect
  SessionAspect
