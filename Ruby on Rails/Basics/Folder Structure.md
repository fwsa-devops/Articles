# Rails Directory Structure Guide

There is a default directory structure that __Ruby on Rails__ comes with. The Rails guides go in depth in explaining the folder structure, but does not talk about the extra folders that commonly get added in Rails Apps.

The goal of this guide is to be a central place to learn about __ALL__ the folders that are used in Rails apps, _not just the ones that come by default (Marked with asterisk)_. 

We will also go over explaining __RSpec__ folder structure and any additional folders.

## Directory Structure

- [app](#app)
	- [assets](#app_assets)
	- [channels](#app_channels)
	- [controllers](#app_controllers)
	- [helpers](#app_helpers)
	- [jobs](#app_jobs)
	- [mailers](#app_mailers)
	- [models](#app_models)
	- [views](#app_views)
- [bin](#bin)
- [config](#config)
	- [environments](#config_environments)
	- [initializers](#config_initializers)
	- [locales](#config_locales)
- [db](#db)
	- [migrate](#db_migrate)
- [lib](#lib)
	- [assets](#lib_assets)
	- [tasks](#lib_tasks)
- [log](#log)
- [public](#public)
- [test](#test)
	- [controllers](#test_controllers)
	- [fixtures](#test_fixtures)
	- [helpers](#test_helpers)
	- [integration](#test_integration)
	- [mailers](#test_mailers)
	- [models](#test_models)
- [tmp](#tmp)
- [vendor](#vendor)

---

### <a name="app"></a> app

It organizes your application components. It's got subdirectories that hold the views, controllers, models, and more that handle business logic.

### <a name="app_assets"></a> app/assets

Holds the assets for your application including images, stylesheets, and javascript.

### <a name="app_channels"></a> app/channels

Contains channels used to setup connections with [ActionCable](http://guides.rubyonrails.org/action_cable_overview.html#channels).

### <a name="app_controllers"></a> app/controllers

Contains app [controllers](http://guides.rubyonrails.org/action_controller_overview.html).

### <a name="app_helpers"></a> app/helpers

Contains app [helpers](http://guides.rubyonrails.org/action_view_overview.html#overview-of-helpers-provided-by-action-view).

### <a name="app_inputs"></a> *app/inputs

Simple form allows you to create custom input components and you can place them here.

- [github](https://github.com/plataformatec/simple_form) simple form gem.
- [github](https://github.com/plataformatec/simple_form/wiki/Adding-custom-input-components) create custom input component.

### <a name="app_jobs"></a> app/jobs

Contains app [jobs](http://guides.rubyonrails.org/v4.2/active_job_basics.html).

### <a name="app_mailers"></a> app/mailers

Contains app [mailers](http://guides.rubyonrails.org/action_mailer_basics.html).

### <a name="app_models"></a> app/models

Contains app [models](http://guides.rubyonrails.org/active_record_basics.html).

### <a name="app_views"></a> app/views

Contains app [views](http://guides.rubyonrails.org/layouts_and_rendering.html).

---

### <a name="bin"></a> bin

Contains the rails script that starts your app and can contain other scripts you use to setup, update, deploy or run your application.

---

### <a name="config"></a> config

Configure your application's routes, database, and more. This is covered in more detail in [Configuring Rails Applications](http://guides.rubyonrails.org/configuring.html).

---

### <a name="db"></a> db

Contains your current database schema, as well as the database migrations.

---

### <a name="lib"></a> lib

Extended modules for your application.

---

### <a name="log"></a> log

Application log files.

---

### <a name="public"></a> public

The only folder seen by the world as-is. Contains static files and compiled assets.

---

### <a name="test"></a> test

Unit tests, fixtures, and other test apparatus. These are covered in [Testing Rails Applications](http://guides.rubyonrails.org/testing.html).

---

### <a name="tmp"></a> tmp

Temporary files (like cache and pid files).

---

### <a name="vendor"></a> vendor

A place for all third-party code. In a typical Rails application this includes vendored gems.
