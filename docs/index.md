---
layout: page
---

# Dog Patrol Service API

The Dog Patrol is a cloud-based service that connects dog owners who need professional caretakers with dog sitters who can walk, run, or house dogs. It's a complementary service that web and app developers can easily integrate into existing online platforms and apply custom branding and a unique customer-facing UI.

There are two resources.

**Dog Jobs** - Job postings created by registered dog owners. The Dog Jobs resource includes endpoints to create, retrieve, update, and delete job posting information.

**Dog Sitters** - Dog sitters who have completed a user form. The Dog Sitters resource includes endpoints to create, retrieve, update, and delete their user data.

**NOTE**: The API service does not auto-match dog owners and sitters. Instead, the dog owner can search the database for possible matches based on criteria like location or availability. In turn, dog sitters can scan for relevant job postings that match their interests.

## Quickstart

[Quickstart](../docs/api/quickstart.md) with the Dog Patrol service to see how easy it is to use!
[Quickstart](/docs/api/quickstart.md) with the Dog Patrol service to see how easy it is to use!
[Quickstart](/api/quickstart.md) with the Dog Patrol service to see how easy it is to use!
[Quickstart](../api/quickstart.md) with the Dog Patrol service to see how easy it is to use!

## Tutorials

Before you get started, complete this prerequisite tutorial to set up your development. You only have to do this one time per development system.

* [Before you start a tutorial](tutorials/before-you-start-a-tutorial)

After your system is ready, try the following tutorial and learn how to perform common tasks.

* [Enroll a new dog sitter](tutorials/enroll-a-dog-sitter.md)

## API reference docs

The API reference docs refer to a `{server_url}` when they
refer to the URL of a resource. The `{server_url}` value depends
on the installation of the service. When run locally for testing, the `{_url}` is generally `http://localhost:3000`.

* [Dog Jobs resource](api/dogjobs.md)
* [Dog Sitter resource](api/dogsitter.md)
