# tophackr status

## How to modify files to your own status

In config ([_config.yml]) you need to change this line to your own.
```
title: example status
description: example description to site
baseurl: '/status' # if you want to connect your own domain to the status of the quotation marks leave blank or remove this line.
url: 'https://example.com'
repository: 'https://example.github.com/example-name/example-project'
email: admin@example.com
twitter: examplestatus
```

and you need to change `zone` to your timezone, and `timezone`. A list of all available values can be found [here](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
```
zone: 'UTC+3' # example
timezone: Europe/Moscow # example
```

## How to create incident

There are 3 types of incident [danger], [warning], [success].  
You can use these drafts as you want, just note that the history displays danger incident.  
Posts need to be created in the folder [_posts]

## How to create a status level at the top

When you create an incident, there is a `category` in the incident. When you write a category, such as example or 'example.com', a new status is created at the top. And depending on the last status of the post (danger, warning, success) of this category, there will be the color of the status at the top.

## If you have a problem

Check [repository page][repository] or [status page][status]

[_config.yml]: _config.yml
[danger]: _drafts/danger.md
[warning]: _drafts/warning.md
[success]: _drafts/success.md
[_posts]: _posts/
[repository]: https://github.com/tophackr/status-other
[status]: https://tophackr.github.io/status-other
