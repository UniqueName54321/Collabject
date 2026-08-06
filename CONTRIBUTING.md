# Contributing to Collabject

Thanks for helping out! You can suggest a project through an issue or add its
registry file yourself. Either way, please make sure the developer is happy for
the project to be listed and give us a public link that backs up the details.

## First, a quick name check

Collabject is an external, unaffiliated website. It is **not Object Collab** and
it is **not Object Workshop**:

- Object Workshop downloads *prefabs* that use vanilla Geometry Dash objects.
- Object Collab is an API mod that lets mods add objects.
- Collabject lists downloadable mods that rely on the Object Collab API—what
  you can think of as “modded objects.”

Please describe projects with that distinction in mind. Don't say that
Collabject itself adds objects or that it is part of either mod.

## The easy route: open an issue

Open the **Issues** tab and choose **Submit an Object Collab project**. Tell us
what the project does, how it connects to Object Collab, and where we can verify
that. A maintainer will turn the submission into a registry entry.

## Adding the JSON yourself

1. Fork this repository.
2. Copy [`registry/example.json`](registry/example.json).
3. Rename the copy using the Geode mod ID, or the project name if it has no ID.
4. Swap the example data for the real project details.
5. Check that the file is valid JSON.
6. Open a pull request and include evidence of the Object Collab connection.

Keep filenames lowercase and use hyphens between words. For example:

- `lua-trigger.json`
- `developer-dialogue-objects.json`
- `object-groups.json`

## Values the registry understands

Use one of these values for `relationship`:

- `adds_objects`
- `uses_objects`
- `compatibility`
- `developer_tool`
- `experimental`

Use one of these values for `status`:

- `released`
- `public_beta`
- `work_in_progress`
- `planned`
- `discontinued`

The `objects` field is a JSON array. Leave it empty (`[]`) when individual
objects don't apply. A missing link can be `null`, just like the `website` in
the example. Please don't invent placeholder URLs in a real entry.

## A few ground rules

- Get the developer's permission before listing their project.
- Only claim support that can be checked publicly.
- Link to the Geode index, source repository, docs, release notes, or another
  useful source whenever possible.
- Keep one project in one registry file unless there is a good reason not to.
- Search the registry first so we don't end up with duplicate entries.
