---
layout: home
title: "Building a Website with Jekyll in GitHub"
lesson-example: "https://carpentries.github.io/lesson-example/"
---
<!-- the lesson-example is a local variable to refer to later in this page -->

## Description
{{ site.description }}
{% assign lead = site.team_members | where:"role", "project lead" | first %}
The project is led by {{ lead.name }}.
[See our full team](about#team)

More details about the project are available from the [About page](about).

See some [examples of our work]({{page.lesson-example}}).

Have any questions about what we do? [We'd love to hear form you!](mailto:{{ site.email }})
