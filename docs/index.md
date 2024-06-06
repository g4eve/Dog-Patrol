---
layout: page
---

# Dog Patrol Service API

The Dog Patrol is a cloud-based service that brings together dog owners who need professional caretakers and dog sitters who can walk, run, or house dogs. It's a complementary service that web and app developers can easily integrate into the existing online platforms and apply custom branding and a unique customer facing UI.

There are two resources.

**Dog Jobs** - Job postings created by the registered dog owners. The Dog Jobs resource includes endpoints to create, retrieve, update, and delete job posting information.

**Dog Sitters** - Dog sitters who have completed a user form. The Dog Sitters resource includes endpoints to create, retrieve, update, and delete their user data.

**NOTE**: The API service does not auto-match dog owners and sitters. Instead, the dog owner can search the database for possible matches based on criteria like location or availability. In turn, dog sitters can scan for relevant job postings that match their intersts.

## Quickstart

[Quickstart _(coming soon)_](#quickstart) with the Dog Patrol service to see how easy it is to use!

## Tutorials

Learn how to do common tasks with in the Dog Patrol service.

Before you get strated, complete this prerequisite tutorial to set up your development. You only have to do this one time per development system.

* [Before you start a tutorial](tutorials/before-you-start-a-tutorial)

After your system is ready, select a tutorial and learn how to perform common tasks.

### Dog Sitters
* [Enroll a new dog sitter](tutorials/enroll-a-dog-sitter.md)
* [Update a dog sitter's information _(coming soon)_](tutorials/edit-a-dog-sitter)
* [Delete a dog sitter _(coming soon)_](tutorials/delete-a-dog-sitter)
* [Find a dog sitter by a property _(coming soon)_](tutorials/get-a-dog-sitter)

### Dog Jobs
* [Create a job post _(coming soon)_](tutorials/add-a-new-job-post)
* [Edit a job post _(coming soon)_](tutorials/edit-a-job-post)
* [Delete a job post _(coming soon)_](tutorials/delete-a-job-post)
* [Find a job post by a property _(coming soon)_](tutorials/get-a-job-post)

## API reference docs

Detailed descriptions of the service's resources.

The API reference docs refer to a `{base_url}` when they
refer to the URL of a resource. The `{base_url}` value depends
on the installation of the service. When run locally for testing, the `{base_url}` is generally `http://localhost:3000`.

* [Dog Job resource](docs/api/dog-sitter.md)
* [Dog Sitter resource](api/dog-sitter.md)
