---
layout: home
lesson-example: "https://carpentries.github.io/lesson-example/"
---

# Building Websites in GitHub

# Description
{{ site.description}}
{% assign lead=site.team_members | where: "role","project lead"|first %}
The project is lead by {{ lead.name }}.

More details about the project are available from the [About page](about).

See some [examples of our work]({{page.lesson-example}}).

Have any questions about what we do? [We'd love to hear form you!](mailto:{{ site.email }})

## Blog Posts

{% for post in site.blogposts %}
- {{ post.date| date_to_string}}: [{{post.title }}]({{post.url|relative_url}})
{% endfor %}
