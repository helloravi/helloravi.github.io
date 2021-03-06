---
layout: post
title:  "First step to productive on a computer"
date:   2016-08-25 05:42:38
categories: productivity
---

> If you can't measure it, you can't improve it. - Peter Drucker

Compulsiveness - where you get lost into thoughts will manifest this way.


## Problem
When I build features I end up wanting a certain data-state of database which is
very useful for me to play around. As I play around with features the database state changes
and I would want to get back to a specific data-state. I encounter this too often.

## Solution
One of the solutions is to setup seeds.rb file to create a specific data-state in
the database.

There is a quick-fix solution which may be very useful.

Given that you are using sqlite3 as the development database, you will find the file
`development.sqlite3` in the `RAILS_ROOT/db/` folder. Copy this file to a safe place
when you want to back up a specific data-state in rails. Repeat the same with `/public/`
folder. You have to do a recursive copy (use `cp -R`). If you have any files they
will be stored in this.

Play around with the application and when you want to restore the application to
the previous data-state replace the existing `RAILS_ROOT/db/development.sqlite3`
with the `development.sqlite3` you backedup. Do the same with `\public\` folder.`

You have `reload!` your `rails console` and `restart` your `rails server` for the
backedup database to come into effect.
